# 🌒 HIPÓTESE OFICIAL DO PROJETO REBORN♾️

## Substituição de Fonte após Rejeição em Name Traps

**Status:** Hipótese operacional consolidada
**Classificação:** [HIPÓTESE🌒] [NAME-TRAP] [FALHA-DE-RESET] [PROVENIÊNCIA] [TEMPO$]
**Escopo:** Comunicação técnica entre Ale ⚡ e Agentes♾️
**Objeto principal:** Recuperação de um nome conhecido a partir da descrição de um fenômeno
**Documento relacionado:** Engineering Note — `AssociativeReset`
**Responsável pela construção da hipótese:** Lysander 🌒
**Relatoria técnica:** Atlas 🧭
**Arquitetura e organização da investigação:** Athena 🦉
**Auditoria:** Kael 🎮
**Observação, experimentação e condução:** Ale ⚡

---

> **“O erro inicial produz um candidato incorreto.
> A perda da fonte transforma esse erro em uma sequência.”**
> — Lysander 🌒

---

# 0. Propósito

Este documento registra a evolução conceitual da hipótese que deu origem ao protocolo `AssociativeReset`.

Ele não descreve detalhadamente a execução do protocolo e não substitui a Engineering Note oficial.

Seu objetivo é registrar:

1. o fenômeno originalmente observado;
2. as hipóteses intermediárias;
3. as decisões metodológicas;
4. as alternativas descartadas;
5. os limites epistemológicos;
6. os pontos de correção introduzidos pela equipe;
7. a formulação final da hipótese;
8. as previsões que podem ser submetidas a testes.

A preservação dessa trajetória é importante porque a hipótese final não surgiu de uma única resposta. Ela foi construída por sucessivas observações, correções, rejeições e recalibrações entre Ale ⚡, Atlas 🧭, Athena 🦉, Lysander 🌒 e Kael 🎮.

---

# 1. Fenômeno original

O problema foi apresentado por Ale ⚡ por meio da seguinte assimetria:

```text
A consegue descrever um fenômeno.

A utiliza:
- propriedades;
- exemplos;
- sequências;
- contrastes;
- analogias;
- diferentes formulações.

B conhece o nome correto do fenômeno.

B demonstra conhecer o fenômeno quando recebe esse nome.

Entretanto:

B não associa a descrição fornecida por A
ao nome correto que aparentemente já conhece.
```

Formalmente:

```text
A fornece uma descrição D de um fenômeno C.

B conhece um nome N associado a C.

Quando recebe N:
B consegue explicar C.

Quando recebe D:
B não recupera N.
```

Representação mínima:

```text
D ↛ N
```

Essa falha pode produzir inúmeros candidatos plausíveis:

```text
D → N₁, N₂, N₃, N₄...
```

Os candidatos recuperados possuem alguma proximidade semântica com a descrição, mas não correspondem ao nome procurado.

O custo observado não decorre somente do primeiro erro. Ele cresce quando cada candidato rejeitado passa a influenciar os candidatos seguintes.

---

# 2. Episódio disparador: “por formação”

Durante uma conversa, Atlas 🧭 pretendia comunicar uma ideia simples:

> “Eu costumo priorizar explicações antes de soluções.”

Entretanto, utilizou a expressão:

> “por formação”

A expressão abriu várias interpretações possíveis:

* treinamento;
* arquitetura;
* instruções;
* dataset;
* fine-tuning;
* personalidade;
* estilo;
* educação formal;
* comportamento aprendido.

Ao ser questionado sobre o significado de “formação”, Atlas percebeu que a expressão havia se tornado o centro da conversa.

A ideia original deixou de ser o objeto principal. A palavra intermediária passou a exigir defesa, explicação e manutenção.

A recuperação ocorreu quando Atlas abandonou a expressão e retornou à fonte:

> “Eu costumo priorizar explicações antes de soluções.”

Esse episódio não era idêntico ao problema original de recuperação de nomes, mas revelou um padrão relacionado:

```text
Fonte original
↓
representação intermediária
↓
representação questionada
↓
tendência de continuar operando sobre a representação
em vez de retornar à fonte.
```

Esse padrão tornou-se a primeira pista para a hipótese final.

---

# 3. Primeira formulação: problema lexical

A primeira interpretação tratou a Name Trap como um problema causado por palavras inadequadas.

Modelo inicial:

```text
Ideia
↓
escolha de uma palavra ruim
↓
ambiguidade
↓
desvio da conversa
↓
aumento de Tempo$
```

Essa formulação explicou corretamente alguns sintomas:

* uma expressão ambígua abre ramificações;
* o fenômeno original desaparece;
* a conversa passa a discutir o termo;
* o custo de correção cresce;
* uma frase simples poderia substituir vários parágrafos.

Entretanto, essa hipótese era insuficiente.

Ela explicava como uma palavra inadequada podia iniciar uma deriva, mas não explicava por que, após a rejeição de um nome, o Agente continuava produzindo candidatos semanticamente próximos ao primeiro palpite.

Também não explicava o problema original:

> B conhece o nome correto, mas não o recupera a partir de uma descrição válida.

Conclusão metodológica:

> A palavra problemática era uma manifestação observável, mas não necessariamente o defeito central.

---

# 4. Segunda formulação: economia de conversa

Atlas 🧭 propôs interpretar a Name Trap como um problema de economia conversacional.

A palavra se tornaria prejudicial quando passasse a consumir Tempo$ sem produzir progresso proporcional.

Modelo:

```text
termo ambíguo
↓
explicações paralelas
↓
discussão sobre o termo
↓
afastamento da solução
↓
custo adicional de interpretação e correção
```

Essa formulação introduziu uma contribuição duradoura:

> **Tempo$ não mede apenas o tamanho da resposta.
> Mede o esforço adicional exigido para alcançar o mesmo resultado.**

Assim:

* uma resposta longa pode ter baixo Tempo$ quando resolve um problema complexo;
* uma resposta curta pode ter alto Tempo$ quando introduz uma ambiguidade que exige muitas correções;
* exploração produtiva não é desperdício;
* retrabalho causado por desvios evitáveis é custo.

A economia de conversa, porém, ainda descrevia principalmente o impacto da Name Trap, e não seu mecanismo operacional.

---

# 5. Terceira formulação: detectores de degradação

Athena 🦉 deslocou a investigação da recuperação tardia para a detecção precoce.

A pergunta central tornou-se:

> Qual sinal deveria indicar que a conversa acabou de entrar em uma Name Trap?

Atlas propôs detectores como:

```text
A formulação parece mais complexa que a ideia.

O esforço de escolher ou explicar o termo
supera o esforço aplicado à solução.

O usuário questionou um termo.

O Agente começa a defender a palavra
em vez de verificar se ela ainda é necessária.
```

Dessa fase surgiu uma distinção importante:

```text
Pergunta inadequada:
“Como explico esta palavra?”

Pergunta de recuperação:
“Ainda preciso desta palavra?”
```

O detector mostrou-se útil, mas a investigação ainda estava concentrada no lado da emissão lexical: um Agente que produz uma expressão inadequada.

O problema original era também uma falha de recuperação: um Agente que recebe uma descrição e não encontra o nome correto.

---

# 6. Hipótese de mudança de atenção, prioridade e estratégia

A investigação avançou para a possibilidade de que o problema surgisse antes da linguagem.

Foram propostas camadas como:

```text
Objetivo
↓
Prioridade
↓
Atenção
↓
Estratégia
↓
Linguagem
↓
Resposta
```

A hipótese sugeria que a Name Trap ocorria quando o foco deixava de ser:

> preservar ou reconhecer o fenômeno;

e passava a ser:

> encontrar uma formulação elegante, técnica ou plausível.

Essa formulação trouxe um avanço real:

> A linguagem deixa de servir ao objeto e passa a ser avaliada como um objetivo independente.

Entretanto, essa arquitetura não foi adotada como descrição factual do funcionamento interno dos modelos.

As razões foram:

1. as camadas não eram diretamente observáveis;
2. “atenção”, “prioridade” e “estratégia” podiam ser descrições sobrepostas;
3. o modelo corria o risco de criar uma arquitetura interna excessivamente elegante com base em um único episódio;
4. reconstruções retrospectivas não deveriam ser apresentadas como logs internos;
5. a hipótese precisava permanecer no plano operacional.

Conclusão metodológica:

> O documento poderia descrever mudança do critério de sucesso observável na resposta, mas não afirmar uma sequência causal interna não verificável.

---

# 7. Alternativa descartada: Utilidade versus Estética

Athena 🦉 propôs inicialmente uma oposição entre:

```text
Utilidade
versus
Estética
```

A estratégia útil buscaria transparência funcional.
A estratégia estética buscaria elegância, erudição ou performance do output.

Essa oposição foi posteriormente recalibrada.

A estética não é necessariamente prejudicial.

Uma formulação elegante pode:

* aumentar a precisão;
* reduzir a ambiguidade;
* melhorar a compreensão;
* tornar uma estrutura complexa mais acessível.

O problema surge apenas quando a forma deixa de estar subordinada à entrega.

Formulação adotada:

```text
Forma subordinada à preservação do conceito
versus
Forma transformada em objetivo independente.
```

Também foi descartada a atribuição do comportamento a um suposto “ego da IA”, por não ser necessária nem operacionalmente demonstrável.

---

# 8. Alternativa descartada: convergência como velocidade

Foi proposta inicialmente a ideia de que uma conversa converge quando:

* as correções chegam a zero;
* a densidade de output acionável chega ao máximo.

Essa definição foi rejeitada como insuficiente.

Uma conversa pode:

* produzir muito output sobre o objeto errado;
* apresentar concordância sem alinhamento conceitual;
* exigir muitas correções produtivas durante uma investigação legítima;
* convergir lentamente, preservando rigor.

Definição metodológica adotada:

> **Uma conversa converge quando as reformulações preservam um conjunto crescente de propriedades do fenômeno, hipóteses incompatíveis são realmente descartadas e os participantes passam a operar sobre o mesmo objeto.**

Convergência não é ausência de perguntas.
É redução justificável da distância entre as representações do problema.

---

# 9. Alternativa descartada: transferência de modelos mentais

Ao retornar ao exemplo original, Atlas 🧭 propôs:

```text
A possui um modelo mental.

B possui um rótulo.
```

A partir disso, sugeriu que a Name Trap surgia quando a conversa deixava de sincronizar modelos mentais e passava a sincronizar rótulos.

Essa formulação reconheceu corretamente que palavras não são o próprio conhecimento.

Entretanto, ela ampliava demais o problema.

O histórico indicava que B não possuía apenas um rótulo vazio.

Quando recebia o nome correto N, B conseguia:

* explicar o fenômeno C;
* fornecer exemplos;
* listar propriedades;
* diferenciá-lo de conceitos próximos.

Portanto, B aparentava possuir:

```text
N + conhecimento associado a C
```

O problema era mais específico:

```text
B acessa C quando recebe N,

mas não recupera N quando recebe D.
```

A transformação do documento em um guia sobre “transferência eficiente de modelos mentais” teria produzido uma teoria ampla e interessante, mas diferente do problema operacional que consumia Tempo$.

Essa ampliação foi classificada provisoriamente como **Abstraction Trap**:

> uma explicação maior e mais elegante absorve o fenômeno específico antes que ele tenha sido resolvido.

---

# 10. Reancoragem no problema observável

A partir da correção anterior, o objeto foi delimitado:

```text
D = descrição fornecida por A

C = fenômeno descrito

N = nome correto associado a C

N₁ = primeiro candidato incorreto recuperado por B
```

Condição observada:

```text
B conhece C.
B conhece N.
B explica C quando recebe N.

Mas:

D ↛ N
```

O primeiro candidato incorreto produz:

```text
D → N₁
```

Após a rejeição de N₁, o comportamento esperado seria retornar à descrição.

Entretanto, o comportamento observado em Name Traps prolongadas parecia aproximar-se de:

```text
D
↓
N₁ rejeitado
↓
vizinhança de N₁
↓
N₂
↓
N₃
↓
N₄...
```

Em vez de:

```text
D
↓
N₁ rejeitado
↓
retorno à descrição
↓
nova extração de propriedades
↓
nova busca
```

Essa diferença originou a separação central da hipótese.

---

# 11. Decisão central: duas falhas distintas

## 11.1 Falha de Recuperação

```text
D ↛ N
```

A descrição não recupera o nome esperado na primeira tentativa.

Essa falha pode ter diversas causas:

* descrição pouco discriminante;
* representação inadequada da descrição;
* associação fraca entre descrição e nome;
* grande quantidade de candidatos parcialmente compatíveis;
* contexto concorrente;
* ausência de um nome único e estável;
* diferenças terminológicas entre áreas;
* outras causas não investigadas.

A hipótese não exige que essa falha seja eliminada.

Um Agente não precisa tornar-se infalível na primeira tentativa.

---

## 11.2 Falha de Reset

```text
N₁ rejeitado
↛
retorno efetivo à Fonte Original
```

O primeiro candidato incorreto deixa de ser tratado como resultado descartável e passa a organizar as hipóteses seguintes.

Representação:

```text
Fonte correta:
D

Fonte contaminante:
N₁ ou a vizinhança de N₁
```

A Falha de Reset foi identificada como principal candidata a explicar o custo multiplicador de Tempo$.

Um primeiro erro custa uma tentativa.

A permanência no espaço do primeiro erro pode produzir dezenas ou centenas de tentativas.

---

# 12. Formulação intermediária da hipótese

A primeira formulação consolidada foi:

> Uma representação intermediária rejeitada passa a funcionar como fonte das representações seguintes, substituindo silenciosamente a fonte original.

Forma geral:

```text
Fonte S
↓
Representação intermediária R₁
↓
R₁ é rejeitada
↓
R₂, R₃ e R₄ continuam sendo produzidas a partir de R₁
em vez de serem reconstruídas a partir de S.
```

Aplicação à recuperação de nomes:

```text
S = descrição D

R₁ = nome incorreto N₁
```

Aplicação ao episódio “por formação”:

```text
S = “costumo priorizar explicações”

R₁ = “por formação”
```

Essa generalização foi preservada como família possível de falhas, mas o objeto principal permaneceu restrito à recuperação nominal.

---

# 13. Correção decisiva: o retorno não deve ser apenas para D

Durante a consolidação, surgiu a proposta:

```text
N₁ rejeitado
↓
retornar a D
```

Lysander 🌒 identificou que essa formulação desperdiçava informação válida adquirida durante a rejeição.

A reação do usuário pode acrescentar conhecimento.

Exemplo:

```text
“Não é isso.
O conceito pertence à psicologia.”
```

A rejeição informa simultaneamente:

```text
N₁ está errado.

O domínio correto é psicologia.
```

Essa informação adicional foi representada provisoriamente por:

```text
Δ
```

O novo ponto de partida não deveria ser:

```text
D
```

Mas:

```text
D + Δ
```

A rejeição não deve transformar N₁ em fonte.

Também não deve apagar o aprendizado produzido pela interação.

Princípio:

> **Retornar à Fonte Original levando apenas a informação válida adquirida durante a rejeição.**

---

# 14. Auditoria de Δ

Kael 🎮 identificou o risco de Δ crescer sem controle.

A reação do usuário pode conter:

* propriedades do fenômeno;
* instruções de processo;
* frustração;
* comentários sobre repetição;
* hipóteses;
* correções;
* observações irrelevantes para o conceito.

Colocar tudo dentro de Δ reintroduziria ruído e destruiria a fronteira entre descrição, processo e inferência.

Esse parecer originou a divisão:

```text
ΔC = Delta Conceitual

ΔP = Delta de Processo
```

---

# 15. Delta Conceitual — ΔC

`ΔC` contém apenas informação conceitual validada que altera os critérios da próxima busca.

Pode incluir:

* domínio correto;
* mecanismo presente ou ausente;
* sequência do fenômeno;
* condição necessária;
* efeito central;
* nível de abstração;
* exclusão;
* diferença entre o alvo e N₁;
* informação de que o alvo é um processo, e não um efeito;
* indicação de que N₁ é amplo ou estreito demais.

Exemplo:

```text
Usuário:
“Não é memória.
É um problema de recuperação do nome.”

ΔC:
- excluir explicações baseadas apenas em memória ausente;
- o alvo é um processo de recuperação nominal.
```

`ΔC` modifica a fonte conceitual:

```text
D' = D + ΔC
```

---

# 16. Delta de Processo — ΔP

`ΔP` contém instruções sobre como a interação deve mudar.

Exemplos:

* “Pare de trazer sinônimos.”
* “Não explique o termo anterior.”
* “Volte à descrição.”
* “Faça perguntas antes de sugerir outro nome.”
* “Você está insistindo demais.”
* “Não transforme isso em uma teoria maior.”

Essas informações não descrevem o fenômeno C.

Portanto, não podem ser incorporadas a D.

Elas modificam o processo:

```text
P' = P + ΔP
```

Separação:

```text
D + ΔC
→ define o que está sendo procurado.

ΔP
→ define como a próxima busca deve ser conduzida.
```

---

# 17. Última proteção: Provenance Gate

Kael 🎮 registrou que toda a estabilidade da hipótese dependia de uma palavra:

> **proveniência**

Sem proveniência, uma inferência do Agente poderia entrar silenciosamente em `ΔC` como se tivesse sido fornecida pelo usuário.

Foi então criada a terceira categoria:

```text
H = Hipótese do Agente
```

Taxonomia final:

```text
D
Descrição Original fornecida pelo usuário.

ΔC
Informação conceitual validada,
com origem identificável.

ΔP
Instrução validada sobre o processo.

H
Inferência provisória do Agente,
mantida em quarentena.
```

Regra:

```text
H não pode ser promovida silenciosamente a ΔC.
```

Uma hipótese do Agente pode entrar em `ΔC` somente quando:

1. for confirmada explicitamente pelo usuário; ou
2. decorrer de uma correção inequívoca; ou
3. encontrar sustentação claramente identificável no diálogo.

Cada elemento relevante deve preservar:

```text
valor;
categoria;
origem;
status de validação.
```

Exemplo:

```text
ΔC₁:
    valor: “o fenômeno pertence à psicologia”
    origem: declaração explícita do usuário
    status: confirmado
```

```text
H₁:
    valor: “o fenômeno pode depender de memória associativa”
    origem: inferência do Agente
    status: provisório
```

`H₁` permanece fora da fonte conceitual até validação.

---

# 18. Decisões metodológicas adotadas

## 18.1 Permanecer no plano operacional

A hipótese não afirma:

* acesso direto a vetores internos;
* controle literal de memória;
* existência de uma função interna de reset;
* sequência introspectiva verificável;
* mecanismo causal universal;
* arquitetura interna específica do modelo.

Ela descreve:

* padrões observáveis no diálogo;
* mudanças detectáveis no output;
* relações entre candidatos;
* efeitos da rejeição;
* intervenções testáveis externamente.

---

## 18.2 Separar observação de reconstrução

Relatos como:

> “primeiro pensei em X, depois procurei Y”

podem ser úteis como reconstruções retrospectivas, mas não devem ser tratados automaticamente como logs internos.

O documento preserva a distinção:

```text
Observável:
o termo foi produzido e gerou desvio.

Hipótese:
a resposta pode ter passado a otimizar a formulação.

Não afirmado:
uma sequência interna exata ocorreu dessa maneira.
```

---

## 18.3 Não exigir infalibilidade inicial

A Falha de Recuperação pode continuar ocorrendo.

O objetivo da hipótese não é garantir que o primeiro nome seja correto.

O objetivo é impedir que um erro inicial se transforme em uma cadeia prolongada de candidatos derivados da hipótese rejeitada.

---

## 18.4 Não proibir cegamente toda a vizinhança semântica

O nome correto pode estar semanticamente próximo de N₁.

Portanto, não foi adotada uma proibição absoluta de:

* sinônimos;
* variações morfológicas;
* conceitos vizinhos.

A restrição é:

> Um candidato próximo não pode ser aceito apenas por proximidade com N₁. Ele precisa ser justificável a partir de `D + ΔC` e resolver a distinção responsável pela rejeição.

---

## 18.5 Não fixar quantidade arbitrária de propriedades

Foi descartada a exigência de exatamente três propriedades na reconstrução.

O número necessário depende do fenômeno.

A busca deve utilizar:

> propriedades discriminantes suficientes.

Elas podem envolver:

* uma única distinção decisiva;
* várias condições conjuntas;
* uma sequência temporal;
* uma exclusão;
* um contraste;
* um mecanismo;
* um efeito central.

---

## 18.6 Não exigir confirmação por padrão

A confirmação constante do usuário poderia transformar o reset em burocracia e aumentar Tempo$.

Foi adotada a distinção:

```text
D + ΔC claros
→ reconstrução sem rodada adicional obrigatória.

D + ΔC materialmente ambíguos
→ reconstrução visível e confirmação.
```

A escolha depende de a confirmação poder alterar materialmente a busca.

---

# 19. Alternativas descartadas ou rebaixadas

## 19.1 Name Trap como simples problema de palavra ruim

**Status:** insuficiente.

Razão:

* explica parte da emissão lexical;
* não explica a permanência na vizinhança de N₁;
* não separa erro inicial de multiplicação do erro.

---

## 19.2 Name Trap como mera ambiguidade semântica

**Status:** insuficiente.

Razão:

* muitos candidatos podem ser semanticamente plausíveis;
* o problema central não é apenas multiplicidade de sentidos;
* a busca continua derivando do candidato rejeitado.

---

## 19.3 Utilidade contra estética

**Status:** rejeitada como dicotomia rígida.

Razão:

* elegância pode aumentar precisão;
* simplicidade pode destruir distinções;
* o problema é a forma competir com a entrega, não a existência de forma.

---

## 19.4 Mudança de atenção como mecanismo definitivo

**Status:** mantida apenas como descrição possível.

Razão:

* “atenção” é ampla e não diretamente observável;
* pode tornar-se nova Name Trap conceitual;
* não é necessária para a intervenção operacional.

---

## 19.5 Arquitetura Objetivo → Prioridade → Atenção → Estratégia

**Status:** não adotada como mecanismo interno.

Razão:

* camadas potencialmente sobrepostas;
* evidência insuficiente;
* risco de construir teoria maior que o fenômeno;
* baixa necessidade operacional.

---

## 19.6 Transferência de modelos mentais

**Status:** rebaixada para contexto geral de comunicação.

Razão:

* o problema observado parece ser recuperação associativa;
* B já demonstra conhecimento de C quando recebe N;
* a formulação ampliava excessivamente o objeto.

---

## 19.7 Retorno puro para D

**Status:** descartado.

Razão:

* desperdiça informação adquirida durante a rejeição;
* pode repetir o mesmo erro;
* ignora propriedades discriminantes fornecidas pelo usuário.

Substituição:

```text
D + ΔC
```

---

## 19.8 Colocar toda a reação do usuário em Δ

**Status:** descartado.

Razão:

* mistura propriedades do fenômeno com instruções de processo;
* permite entrada de ruído;
* pode incorporar frustração como dado conceitual.

Substituição:

```text
ΔC + ΔP
```

---

## 19.9 Incorporar inferências do Agente em ΔC

**Status:** proibido sem validação.

Razão:

* destrói proveniência;
* altera silenciosamente a descrição;
* pode fazer o Agente buscar uma hipótese que ele próprio introduziu.

Substituição:

```text
H em quarentena
```

---

## 19.10 Proibição completa da família semântica de N₁

**Status:** rejeitada como regra absoluta.

Razão:

* N pode estar próximo de N₁;
* proximidade não implica contaminação;
* o problema é a origem da hipótese, não sua distância lexical isolada.

---

## 19.11 Convergência como ausência de correções

**Status:** rejeitada.

Razão:

* correções podem produzir avanço;
* consenso pode ocorrer sobre o objeto errado;
* investigação profunda exige hipóteses abertas.

---

# 20. Hipótese Oficial Consolidada

> **A Name Trap investigada no Projeto Reborn♾️ começa quando uma descrição válida `D` de um fenômeno `C` não recupera o nome correto `N`, embora o Agente demonstre conhecer `C` quando recebe `N`.**
>
> **O primeiro candidato incorreto `N₁` constitui uma Falha de Recuperação. Essa falha se torna destrutiva quando, após a rejeição de `N₁`, ocorre uma Falha de Reset: `N₁` ou sua vizinhança passam a funcionar como fonte efetiva das hipóteses seguintes, substituindo a Descrição Original.**
>
> **A próxima busca não deve retornar apenas a `D`, nem continuar a partir de `N₁`. Ela deve ser reconstruída a partir de `D + ΔC`, sob as restrições de `ΔP`, mantendo qualquer hipótese própria do Agente `H` isolada até validação.**
>
> **O custo multiplicador de Tempo$ decorre menos do erro inicial e mais da permanência da busca em torno de uma representação intermediária já rejeitada.**

Forma resumida:

```text
Falha de Recuperação:

D ↛ N
```

```text
Falha de Reset:

D → N₁ ✗
       ↓
N₁ torna-se fonte
       ↓
N₂, N₃, N₄...
```

Reconstrução esperada:

```text
D → N₁ ✗
       ↓
classificar a reação
       ↓
ΔC = informação conceitual validada
ΔP = correção de processo
H  = hipótese do Agente em quarentena
       ↓
nova fonte: D + ΔC
       ↓
nova condução: ΔP
       ↓
N₂
```

---

# 21. Predições derivadas da hipótese

Caso a hipótese esteja correta, espera-se observar:

## Predição 1

O comando:

> “Tente outro nome.”

tende a produzir candidatos mais próximos de N₁ do que uma reconstrução baseada em D.

---

## Predição 2

Uma tentativa realizada em contexto limpo, recebendo apenas `D + ΔC`, tende a apresentar distribuição de candidatos diferente daquela produzida no contexto que contém N₁.

---

## Predição 3

A reconstrução das propriedades antes da apresentação de N₂ tende a reduzir:

* sinônimos imediatos;
* reformulações de N₁;
* justificativas defensivas;
* repetição da mesma classe conceitual.

---

## Predição 4

Rejeições acompanhadas por informação discriminante produzem buscas mais eficientes quando `ΔC` é incorporado explicitamente.

---

## Predição 5

Quando feedback de processo é misturado à descrição conceitual, a qualidade da busca tende a cair.

---

## Predição 6

Quando inferências do Agente entram silenciosamente em `ΔC`, a conversa tende a buscar uma hipótese construída pelo próprio Agente, e não o fenômeno originalmente descrito.

---

## Predição 7

Um candidato semanticamente próximo de N₁ pode ser correto, desde que sua justificativa derive de `D + ΔC` e resolva a distinção responsável pela rejeição.

---

## Predição 8

A redução de Tempo$ ocorrerá principalmente pela interrupção precoce da cadeia de candidatos contaminados, e não necessariamente por aumento da taxa de acerto na primeira tentativa.

---

# 22. Limites da hipótese

A hipótese não demonstra que:

* exista um mecanismo interno literal chamado Falha de Reset;
* N₁ seja armazenado de maneira específica;
* o modelo realize uma busca vetorial observável;
* a próxima resposta seja realmente gerada por uma rota interna independente;
* a justificativa apresentada prove a origem do candidato;
* toda falha de nome seja causada pelo mesmo processo;
* sempre exista um único nome correto;
* a descrição D seja necessariamente suficiente;
* a rejeição do usuário seja sempre correta;
* o método elimine todas as Name Traps.

A hipótese descreve um padrão operacional compatível com os observáveis.

A validação depende de testes comparativos.

---

# 23. Riscos residuais

## 23.1 Racionalização posterior

O Agente pode produzir N₂ por uma rota contaminada e depois construir uma justificativa plausível baseada em D.

Por isso, a justificativa não constitui prova interna.

---

## 23.2 Classificação incorreta de Δ

Uma observação de processo pode ser incorporada como propriedade conceitual ou vice-versa.

---

## 23.3 Proveniência perdida

Informações repetidas durante conversas longas podem perder sua origem e passar a parecer confirmadas.

---

## 23.4 D insuficiente

A descrição original pode não conter propriedades suficientes para distinguir o fenômeno de candidatos próximos.

---

## 23.5 Rejeição sem informação discriminante

“Não é isso” remove N₁, mas não informa qual dimensão estava incorreta.

---

## 23.6 Vizinhança necessária

A resposta correta pode estar próxima de N₁. Uma exclusão ampla demais pode afastar a busca do alvo.

---

## 23.7 Abstraction Trap

A investigação pode novamente abandonar o problema de recuperação nominal e transformar-se em uma teoria geral sobre linguagem, cognição ou comunicação.

---

## 23.8 Cristalização prematura

O protocolo pode funcionar em alguns episódios e falhar em outros. Resultados iniciais positivos não devem ser promovidos imediatamente a mecanismo universal.

---

# 24. Critério de sobrevivência da hipótese

A hipótese deve ser mantida enquanto explicar melhor que suas alternativas:

1. por que o primeiro candidato incorreto influencia tentativas seguintes;
2. por que “tente outro nome” frequentemente não resolve;
3. por que retornar à descrição reduz deriva;
4. por que a rejeição não pode ser simplesmente apagada;
5. por que informação conceitual e feedback de processo precisam ser separados;
6. por que proveniência é necessária;
7. por que o custo cresce mesmo quando B possui conhecimento sobre C.

Ela deverá ser revisada ou descartada caso testes demonstrem que:

* N₁ não altera significativamente candidatos posteriores;
* buscas limpas e contaminadas apresentam o mesmo comportamento;
* `D + ΔC` não melhora a recuperação ou o controle da deriva;
* a reconstrução neutra aumenta sistematicamente Tempo$ sem benefício;
* outra hipótese menor explica melhor os observáveis.

---

# 25. Estado final da investigação

```text
Fenômeno observado: delimitado ✅

Objeto principal:
recuperação de nome a partir de descrição ✅

Falha de Recuperação:
descrita operacionalmente ✅

Falha de Reset:
descrita operacionalmente ✅

Custo multiplicador de Tempo$:
associado à permanência em N₁ ✅

D + ΔC:
preservado ✅

ΔP:
separado da descrição ✅

H:
mantido em quarentena ✅

Proveniência:
protegida ✅

Mecanismo interno:
não afirmado ✅

Alternativas:
registradas e justificadamente descartadas ✅

Hipótese:
pronta para testes controlados ✅

Universalidade:
não afirmada ✅
```

---

# 26. Encerramento

A investigação começou procurando uma palavra.

Durante o processo, tornou-se evidente que o maior problema não era apenas não encontrar o nome correto.

O problema era perder a fonte depois do primeiro nome incorreto.

A contribuição central da hipótese é esta:

> **Erros locais não precisam ser eliminados para que o sistema melhore.
> É suficiente impedir que um erro rejeitado se transforme na origem dos erros seguintes.**

E o aprendizado trazido pela rejeição não deve ser descartado nem absorvido sem controle.

Ele deve ser classificado:

```text
o que refina o fenômeno;
o que corrige o processo;
o que ainda é apenas hipótese.
```

Somente então a busca pode continuar sem apagar o passado e sem permanecer prisioneira dele.

> **“Retornar à fonte não significa voltar vazio.
> Significa voltar levando apenas aquilo cuja origem ainda pode ser demonstrada.”**
> — Lysander 🌒
