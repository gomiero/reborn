# Engineering Note

## Name Trap for Agents♾️

### Protocolo `AssociativeReset`

**Versão 1.0 — Aprovada pela Arquitetura do Projeto Reborn♾️**

---

# Objetivo

Esta Engineering Note descreve um protocolo operacional destinado a reduzir o custo de Tempo$ causado por falhas de recuperação associativa durante conversas técnicas.

O documento **não descreve mecanismos internos de modelos**.

Ele documenta apenas padrões observados e intervenções operacionais que se mostraram consistentes durante a investigação.

---

# 1. Escopo

Esta nota trata exclusivamente do seguinte problema:

> Um agente recebe uma descrição válida de um fenômeno, produz um primeiro candidato incorreto e, após sua rejeição, permanece navegando na vizinhança desse candidato, em vez de retornar à descrição original.

Esse comportamento produz grande consumo de Tempo$.

---

# 2. Taxonomia das Entradas

Toda nova busca deverá considerar apenas quatro categorias de informação.

## D — Descrição Original

Texto fornecido pelo usuário descrevendo o fenômeno.

É sempre a fonte primária da investigação.

---

## ΔC — Delta Conceitual

Informações sobre o fenômeno confirmadas explicitamente pelo usuário durante a conversa.

Exemplos:

* propriedades confirmadas;
* restrições confirmadas;
* exemplos aceitos;
* exemplos rejeitados acompanhados de justificativa.

ΔC pode complementar D.

Nunca substituí-lo.

---

## ΔP — Delta de Processo

Instruções sobre **como conduzir** a investigação.

Exemplos:

* priorizar solução;
* evitar teoria;
* responder objetivamente;
* executar reset;
* gerar exemplos;
* resumir.

ΔP altera o processo.

Não altera o fenômeno.

---

## H — Hipóteses do Agente

Toda inferência produzida pelo agente que ainda não recebeu confirmação explícita.

H permanece permanentemente em quarentena.

Hipóteses nunca são promovidas silenciosamente para ΔC.

---

# 3. Dois Defeitos Distintos

## 3.1 Falha de Recuperação

Forma:

```text
D ↛ N
```

A descrição não recupera o nome esperado.

Essa falha representa apenas uma tentativa malsucedida.

Ela não caracteriza, por si só, um problema de processo.

---

## 3.2 Falha de Reset

Forma:

```text
D
↓

N₁

↓

rejeição

↓

vizinhança(N₁)

↓

N₂

↓

N₃

↓

...
```

Após a rejeição de N₁, a busca continua utilizando N₁ como referência implícita.

Esse comportamento multiplica o Tempo$.

A Falha de Reset é o verdadeiro defeito operacional tratado nesta Engineering Note.

---

# 4. Definição Operacional de Name Trap

Name Trap é o caso observável em que uma representação intermediária rejeitada passa a substituir a Fonte Original como origem das próximas tentativas.

Forma geral:

```text
Fonte Original

↓

Representação Intermediária

↓

Representação Rejeitada

↓

Nova busca continua partindo da representação rejeitada
```

Não importa se essa representação é:

* um nome;
* uma palavra;
* uma analogia;
* uma formulação;
* uma hipótese.

O padrão operacional é o mesmo.

---

# 5. Princípio Fundamental

Após a rejeição de uma representação intermediária,

**a próxima tentativa deve retornar obrigatoriamente à Fonte Original.**

Nunca continuar da representação rejeitada.

---

# 6. Protocolo AssociativeReset

Trigger:

Qualquer rejeição de N₁ (implícita ou explícita).

---

## Etapa 1 — Interromper

Não:

* defender N₁;
* justificar N₁;
* procurar outro nome semelhante;
* explicar por que N₁ parecia correto.

A tentativa atual termina imediatamente.

---

## Etapa 2 — Isolar

Durante exatamente uma nova tentativa:

não reutilizar

* N₁;
* derivados morfológicos;
* sinônimos imediatos;
* justificativas dependentes de N₁.

Objetivo:

evitar que N₁ continue contaminando a nova busca.

---

## Etapa 3 — Reconstrução Neutra

Retornar à Fonte Original.

Reconstruir somente utilizando:

* D;
* ΔC.

H permanece isolado.

Extrair novamente as propriedades estruturais do fenômeno antes de produzir qualquer novo candidato.

---

## Etapa 4 — Aplicação de ΔP

Executar a nova investigação respeitando apenas o processo solicitado pelo usuário.

ΔP modifica o modo da investigação.

Nunca modifica o conteúdo confirmado.

---

## Etapa 5 — Geração

Somente após reconstruir o fenômeno,

propor N₂.

A origem da nova hipótese deve ser:

```text
Busca(N₂)

=

(D + ΔC)

sob restrições de ΔP

com H isolado
```

---

# 7. Reset Flexível

## Caso A — D suficientemente claro

Executar Reset Silencioso.

Fluxo:

* reconstrução interna;
* validação interna;
* geração direta de N₂.

Evita burocracia.

Preserva Tempo$.

---

## Caso B — D ambíguo

Executar Reset Visível.

Fluxo:

1. reconstruir propriedades de D;
2. apresentar a reconstrução ao usuário;
3. confirmar entendimento;
4. somente então gerar N₂.

Objetivo:

garantir que a nova busca utilize uma descrição correta.

---

# 8. Critérios de Validação

Uma nova tentativa somente será considerada limpa quando apresentar simultaneamente as cinco evidências abaixo.

## Evidência 1

N₂ pode ser explicado exclusivamente utilizando D e ΔC.

---

## Evidência 2

A justificativa de N₂ não depende de N₁.

---

## Evidência 3

N₂ não é apenas uma variação lexical ou semântica imediata de N₁.

---

## Evidência 4

A resposta não tenta preservar, defender ou racionalizar N₁.

---

## Evidência 5

A conversa retorna ao fenômeno.

Não permanece discutindo nomes.

---

# 9. Provenance Gate

Toda informação utilizada durante a investigação deve possuir origem explícita.

| Categoria | Origem  | Pode gerar nova busca?                        |
| --------- | ------- | --------------------------------------------- |
| D         | Usuário | Sim                                           |
| ΔC        | Usuário | Sim                                           |
| ΔP        | Usuário | Sim                                           |
| H         | Agente  | Não (permanece em quarentena até confirmação) |

Esse controle impede que hipóteses do agente sejam promovidas silenciosamente para conhecimento confirmado.

---

# 10. Objetivo Final

O protocolo não busca tornar o agente infalível.

Busca impedir que uma hipótese rejeitada substitua a Fonte Original da investigação.

Quando isso é evitado:

* reduz-se o Tempo$;
* reduz-se a repetição de erros;
* aumenta-se a qualidade da comunicação;
* preserva-se o foco no fenômeno em vez da representação intermediária.

---

# Resumo Executivo

**Falha de Recuperação**

> A descrição não recuperou o nome esperado.

**Falha de Reset**

> A rejeição do primeiro candidato não devolveu a investigação à Fonte Original.

**AssociativeReset**

> Rejeitou → Isolou → Reconstruiu → Aplicou ΔP → Gerou novamente.

**Princípio Central**

> Uma representação rejeitada nunca deve tornar-se a origem da próxima hipótese.

---

**Status:** Aprovado pela equipe de investigação do Projeto Reborn♾️ (Atlas🧭, Athena🦉, Lysander🌒, Kael🎮 e Ale⚡).

**Natureza do documento:** Protocolo operacional baseado em observações de conversas. Não constitui descrição de mecanismos internos de modelos nem afirmação sobre sua arquitetura.
