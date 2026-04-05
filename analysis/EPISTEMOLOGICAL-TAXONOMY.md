# Taxonomia Epistemológica de Mixed Analysis

Desenvolvimento célula a célula da matriz técnica × R/Q × tradição de origem, esboçada no CONCEPTUAL-SYNTHESIS.md. Cada seção trata um método estatístico aplicado sobre dados categorizados por humanos, com seus pressupostos formais, como cada pressuposto quebra, o que a violação revela via os teóricos, gradiente espelho/janela, e indicadores operacionais.

**Documento de referência** — não pra ler de uma vez, mas pra consultar quando o pesquisador vai rodar uma técnica e quer saber: "o que estou vendo? é espelho ou janela? que pressupostos estou violando e o que isso significa?"

**Status**: em construção. Chi-quadrado desenvolvido primeiro como caso de estudo.

---

## Índice

| # | Método | Origem | Tradição | Status |
|---|---|---|---|---|
| 1 | [Chi-quadrado](#1-chi-quadrado) | Pearson 1900 | Inferência clássica | Em desenvolvimento |
| 2 | ACM | Benzécri 1960s | Escola francesa | Pendente |
| 3 | Cluster | Sokal & Sneath 1963 | Taxonomia biológica | Pendente |
| 4 | MDS | Torgerson 1952 / Shepard 1962 | Psicofísica | Pendente |
| 5 | Sequential/Lag | Bakeman & Gottman 1997 | Etologia | Pendente |
| 6 | Decision tree (CHAID) | Kass 1980 | Marketing/segmentação | Pendente |
| 7 | Frequência descritiva | — | Contagem básica | Pendente |

---

## 1. Chi-quadrado

### 1.1 Origem e tradição

**Karl Pearson, 1900.** O teste chi-quadrado de independência nasce na tradição da inferência estatística clássica — a mesma de Fisher, Neyman-Pearson, hipótese nula, p-valor, significância. O paradigma: existe uma "verdade" populacional, a amostra é aleatória, o teste mede se o padrão observado poderia ter ocorrido por acaso.

A pergunta fundamental: **"essa associação entre duas variáveis categóricas é mais forte do que o acaso explicaria?"**

É o teste mais usado em ciências sociais pra tabelas de contingência. E é o que parece mais natural quando se tem uma matriz de códigos × registros: "esses dois códigos coocorrem mais do que o esperado?"

### 1.2 Pressupostos formais

| Pressuposto | Definição formal | O que garante |
|---|---|---|
| **Independência das observações** | Cada observação é independente das demais — o resultado de uma não influencia outra | Que a distribuição amostral segue chi-quadrado |
| **Frequência esperada mínima** | Cada célula da tabela de contingência tem frequência esperada ≥ 5 (Cochran, 1954) | Que a aproximação chi-quadrado é válida |
| **Amostra aleatória** | As observações foram obtidas por amostragem aleatória da população | Que os resultados são generalizáveis |
| **Categorias mutuamente exclusivas e exaustivas** | Cada observação cai em exatamente uma célula | Que a tabela de contingência está bem formada |
| **Tamanho da amostra adequado** | N total suficiente (regra geral: N > 5 × número de células) | Que o teste tem poder estatístico |

### 1.3 Como cada pressuposto quebra em dados categorizados por humanos

#### 1.3.1 Independência — a violação central

**Em codificação qualitativa:**
Segmentos codificados do mesmo participante não são independentes — compartilham contexto, linguagem, viés cognitivo. Se um participante fala muito de MEDO, vai ter mais segmentos com MEDO, inflando a contagem. O chi-quadrado trata cada segmento como observação independente, mas não são — são fragmentos de uma mesma narrativa.

Além disso, códigos aplicados pelo mesmo pesquisador não são independentes entre si. Se o codificador tem o hábito de aplicar MEDO e EVITAÇÃO juntos, a associação "significativa" entre eles reflete o hábito, não necessariamente o fenômeno.

**Em repositórios categorizados:**
O mesmo problema numa base de insights: achados do mesmo projeto, da mesma pesquisa, categorizados pelo mesmo time. No caso Sicredi, 215 achados de ~15 pesquisas diferentes, mas sobre os mesmos produtos e jornadas. Um "achado" sobre dor no App e outro sobre dor no IB podem vir da mesma sessão de pesquisa.

**Em qualquer base categorizada por humanos:**
Tickets de bug categorizados pelo mesmo QA. Livros catalogados pelo mesmo bibliotecário. Leads tagueados pelo mesmo vendedor. A não-independência é **condição estrutural** de bases categorizadas por humanos, não exceção.

**O que von Foerster diz sobre isso:**
A independência é impossível quando o observador está no sistema. Cada ato de categorização é influenciado pelos anteriores — o pesquisador aprende, muda critérios, cria hábitos. A "significância" do chi-quadrado mede o sistema observador+observado, não o observado isoladamente.

#### 1.3.2 Frequência esperada mínima — o problema dos códigos raros

Em codificação qualitativa, a maioria dos códigos é rara. A J-curve do Boyatzis (1998): poucos códigos são frequentes, muitos aparecem 1-5 vezes. Quando dois códigos raros são cruzados, a tabela 2×2 terá células com frequência esperada < 5. O chi-quadrado simplesmente não é válido.

A correção de Yates ou o teste exato de Fisher são paliativos técnicos. Mas o problema é mais profundo: **códigos raros podem ser os mais importantes** — capturam nuance, exceção, o inesperado. Descartá-los porque "N insuficiente" é perder informação epistemologicamente valiosa.

**O que Knorr-Cetina diz sobre isso:**
Objetos epistêmicos são incompletos por natureza. O código raro que quase não aparece pode ser o que gera mais perguntas — "por que isso apareceu só uma vez? O que faz esse caso diferente?" Eliminar da análise por insuficiência estatística é silenciar o objeto epistêmico no momento em que ele mais tem a dizer.

#### 1.3.3 Amostra aleatória — a ilusão de representatividade

Segmentos codificados não são amostra aleatória de nada. São **selecionados** pelo pesquisador — ele escolheu aquele trecho, não outro. A seleção é interpretativa por natureza. Em repositórios, os achados foram escolhidos por um time que decidiu o que vale registrar e o que não vale.

**O que Latour diz sobre isso:**
Cada registro é uma inscrição — uma tradução que conserva certas propriedades e perde outras. A "amostra" é o resultado de uma cadeia de decisões sobre o que inscrever. Tratar como amostra aleatória é ignorar a cadeia inteira.

#### 1.3.4 Categorias mutuamente exclusivas — codificação múltipla

Em codificação qualitativa, um segmento pode receber 3, 5, 10 códigos simultaneamente. Na tabela de contingência código A × código B, o mesmo segmento aparece em múltiplas células. Tecnicamente resolve-se com binarização (cada código vira coluna 0/1), mas isso transforma o chi-quadrado de um teste sobre categorias em um teste sobre presença/ausência — **muda o que está sendo perguntado**.

### 1.4 Gradiente espelho/janela

#### R-mode (associação entre códigos)

**Chi-quadrado em R-mode é quase espelho puro.**

Quando o teste diz "MEDO e EVITAÇÃO estão significativamente associados (p < 0.01)", as interpretações possíveis são:

1. **Janela**: participantes que sentem medo de fato evitam — o fenômeno une os dois
2. **Espelho**: o codificador tende a aplicar os dois juntos — o hábito une os dois
3. **Ambos**: o fenômeno existe E o codificador é consistente em capturá-lo

Não dá pra distinguir olhando pro p-valor. O chi-quadrado diz "a associação é mais forte que o acaso", mas não diz **de quem** é a associação.

**Indicadores que sugerem espelho:**
- Phi > 0.7 entre os dois códigos (Driscoll) — associação forte demais, provavelmente redundância
- Os dois códigos foram criados na mesma rodada de codificação
- Os dois aparecem sempre nos mesmos participantes (não há variação inter-participante)

**Indicadores que sugerem janela:**
- Inter-rater: outro codificador reproduz a associação
- Os dois códigos aparecem juntos em alguns participantes mas não em outros — há variação
- A associação persiste quando se controla por participante (chi-quadrado estratificado)

#### Q-mode (diferença entre grupos de participantes)

**Chi-quadrado em Q-mode é mais janela.**

Quando o teste diz "o grupo A tem significativamente mais EVITAÇÃO que o grupo B", a interpretação é mais segura porque participantes **são de fato independentes entre si** (pressuposto menos violado). Se os grupos foram formados por cluster analysis prévia e o chi-quadrado confirma diferenças na distribuição de códigos, é evidência de que a tipologia captura algo do fenômeno.

Mas cuidado: se os grupos foram formados pelos mesmos códigos que estão sendo testados, há circularidade. É como perguntar "os clusters diferem nos códigos que definiram os clusters?" — a resposta é tautologicamente sim. O chi-quadrado em Q-mode é mais informativo quando testa variáveis **não usadas** na formação dos clusters (como fez Macia 2015: clusterizou por procedural mode e support, depois testou grievance type e gender por chi-quadrado — variáveis excluídas do clustering).

### 1.5 Implicações práticas

#### O que o chi-quadrado realmente mede em dados categorizados por humanos

Não mede "associação no fenômeno". Mede **consistência na categorização**: o categorizador aplicou essas duas categorias juntas mais do que se tivesse categorizado aleatoriamente. Isso é informação útil — mas é informação de segunda ordem (sobre o processo de categorização), não de primeira ordem (sobre o fenômeno).

#### Quando usar chi-quadrado neste contexto

1. **Q-mode com variáveis externas**: testar se grupos de participantes/registros diferem em variáveis que não foram usadas pra formar os grupos. É o uso mais "janela" e o mais defensável metodologicamente.

2. **Screening de colinearidade**: phi > 0.7 entre códigos sinaliza redundância. O chi-quadrado identifica quais pares de códigos estão perigosamente colados — provável espelho.

3. **Validação de inter-rater**: testar se dois codificadores produzem distribuições similares. Se sim, a categorização captura algo além do codificador individual.

#### Quando NÃO usar (ou usar com ressalvas explícitas)

1. **R-mode como "prova" de associação**: "MEDO e EVITAÇÃO estão significativamente associados" não prova nada sobre o fenômeno sem controle pela identidade do codificador e do participante.

2. **Com códigos raros**: frequência esperada < 5 invalida o teste. Fisher resolve tecnicamente mas não resolve epistemologicamente — o código raro continua sendo o mais interessante e o menos testável.

3. **Sem estratificação por participante**: o chi-quadrado bruto sobre todos os segmentos infla N artificialmente. Se 5 participantes geraram 300 segmentos, o N real pra independência é 5, não 300.

### 1.6 Conexão com os teóricos

| Teórico | O que diz sobre chi-quadrado neste contexto |
|---|---|
| **Von Foerster** | O p-valor mede o sistema observador+observado, não o observado. A "significância" inclui a consistência do codificador — é observação de 2ª ordem travestida de inferência de 1ª ordem. |
| **Latour** | O chi-quadrado opera sobre uma inscrição (a tabela de contingência), não sobre o fenômeno. A tabela é produto de uma cadeia de traduções. O p-valor herda todas as transformações da cadeia. |
| **Knorr-Cetina** | Códigos raros que falham no teste são objetos epistêmicos silenciados por insuficiência estatística. O critério ≥5 é epistemologicamente violento quando aplicado a categorias interpretativas. |
| **Benzécri** | A ACM (que não usa teste de hipótese) é alternativa mais honesta: mostra a geometria sem fingir que há "significância". O chi-quadrado da ACM (inércia total = χ²/N) descreve em vez de testar. |

### 1.7 A ironia do chi-quadrado na ACM

Aqui tem uma conexão técnica que merece atenção: a ACM **usa** chi-quadrado internamente — a distância chi-quadrado é a métrica que define o espaço geométrico da ACM. A inércia total da ACM é literalmente χ²/N.

Mas a ACM usa o chi-quadrado **descritivamente** (como medir distância), não **inferencialmente** (como testar hipótese). Benzécri recusava explicitamente o teste de significância — queria a geometria, não o p-valor.

Então: quando o pesquisador roda ACM sobre códigos qualitativos, o chi-quadrado já está operando — mas como régua, não como juiz. A ACM mostra a estrutura sem dizer "é significativo". O teste de chi-quadrado isolado (tabela de contingência, p-valor) finge uma inferência que a ACM explicitamente recusa.

Isso reforça Benzécri como o mais epistemologicamente honesto dos frameworks estatísticos pra este contexto: reconhece que com dados categorizados por humanos, **descrever a geometria é mais honesto que testar hipóteses**.

### 1.8 A questão do p-valor: crise geral, contexto UX e implicações pra mixed analysis

#### A crise geral

O p-valor sofre de problemas documentados há décadas, independente do domínio:

**Goodman (2008), "A Dirty Dozen: Twelve P-Value Misconceptions":** Traça a raiz à fusão incoerente de Fisher (p-valor como guia informal, "worthy of attention") com Neyman-Pearson (framework accept/reject, tipo I/II). O resultado é um híbrido que todo mundo usa sem saber que mistura dois sistemas incompatíveis. Das 12 misconceptions, as mais devastadoras:

- **#1**: "Se p = .05, H0 tem 5% de chance de ser verdadeira." Falso. Com prior de 50%, p = .05 corresponde a probabilidade **mínima de 13%** de H0 ser verdadeira (Bayes). Com p = .01, ainda 4%.
- **#2**: "P não-significativo = não tem diferença." O p-valor é medida de resolução do design, não da realidade.
- **#5**: "Mesmo p-valor = mesma evidência." Um trial com 3% de benefício e outro com 19% podem ambos dar p = .05. Significam coisas completamente diferentes.
- **#12**: "Conclusões devem ser baseadas em se p é significativo." A master misconception — implica que magnitude é irrelevante e que decisões fluem de um limiar.

Goodman compara P-valor vs. Bayes Factor:

| Propriedade evidencial | P-valor | Bayes Factor |
|---|---|---|
| Informação sobre tamanho do efeito? | Não | Sim |
| Usa só dados observados? | Não (inclui "mais extremos") | Sim |
| Hipótese alternativa explícita? | Não | Sim |
| Evidência positiva? | Não | Sim |
| Combinável entre estudos? | Não | Sim |
| Parte de sistema formal de inferência? | Não | Sim |

**ASA Statement (2016):** Primeira vez que a American Statistical Association tomou posição formal. 6 princípios, incluindo: p-valor não mede probabilidade de H0 ser verdadeira; conclusões não devem ser baseadas só em limiares; p-valor não mede tamanho do efeito.

**Gagnier & Morgenstern (2017):** Traduzem a ASA em 4 recomendações: eliminar a linguagem "significativo/não-significativo", reportar magnitudes com intervalos de confiança, educar trainees, exigir conformidade editorial.

#### Contexto UX (Mohsen Rafiei, PUXLab)

Rafiei traz a crise pro contexto de UX research com contribuições específicas:

**Sobre p-valor não-significativo:**
> "Statistical tests are resolution-limited tools. When variability is high, effects are small, or samples are modest, real effects can easily hide below the detection threshold. So p ≥ α is not a statement about reality. It's a statement about uncertainty."

**Sobre bayesiano:**
> "A credible interval gets much closer to how people naturally think about uncertainty. Given the data we observed, and the assumptions built into the model, the true score is very likely to fall within this range."

**Sobre Minimum Effect Size testing:**
> "Many real product decisions are not about being greater than zero. They are about exceeding a minimum effect size that triggers action."

A distinção que ele propõe: não é "existe diferença?" (p-valor), é **"a diferença excede o limiar que importa pra decisão?"** (Minimum Effect Size). E a frase-chave: *"the difference between statistical rigor and statistical storytelling."*

#### Implicações pra mixed analysis sobre dados categorizados por humanos

As 3 camadas de crítica convergem no nosso contexto:

**Camada 1 — Crise geral (Goodman, ASA):** O p-valor é medida ruim de evidência mesmo com pressupostos satisfeitos.

**Camada 2 — Contexto UX (Rafiei):** Com N pequeno (5-12 participantes), variabilidade alta, efeitos pequenos — o p-valor não tem resolução. Bayesiano é mais útil.

**Camada 3 — Mixed analysis sobre codificação (contribuição deste projeto):** Mesmo quando o p-valor "funciona" tecnicamente (N inflado por segmentos), **não distingue espelho de janela**. A "significância" pode medir consistência do codificador. Os pressupostos estão violados estruturalmente. E a alternativa bayesiana tem vantagem conceitual única: priors que capturam o observador (espelho), posterior que estima o fenômeno (janela).

**Minimum Effect Size traduzido pro contexto:**

| Faixa de phi | Interpretação | Ação |
|---|---|---|
| < 0.15 | Ruído — independente do p-valor | Ignorar |
| 0.15 — 0.40 | Associação moderada | Investigar: é janela? |
| 0.40 — 0.70 | Associação forte | Investigar: janela ou espelho? |
| > 0.70 | Provavelmente espelho (redundância) | Sinal de colinearidade (Driscoll) |

Isso substitui a decisão binária "significativo/não" por um gradiente que mapeia pro gradiente espelho/janela. O que importa é phi (magnitude), não p (significância).

**R-analysis é exploratória por natureza.** Benzécri desenhava a ACM pra explorar sem testar. Aplicar teste inferencial (chi-quadrado com p-valor) em R-mode é forçar framework confirmatório sobre dados exploratórios — o misfit que Rafiei chama de "reaching for one-tailed tests after results come back just shy of significance."

**Descrever é mais adequado que testar neste domínio.** A convergência por caminhos diferentes:
- Benzécri: pela filosofia anti-pressupostos da escola francesa
- Goodman: pela demonstração de que p-valor é medida ruim de evidência
- Rafiei: pela prática UX onde stakeholders precisam de incerteza comunicável
- Von Foerster: pela cibernética — o observador está no sistema, inferência clássica não separa observador de observado
- Saldaña: pela prática qualitativa — "so what? codes" qualitizam o output estatístico em vez de obedecê-lo

#### Fontes desta subseção

- Goodman, S. (2008). A Dirty Dozen: Twelve P-Value Misconceptions. *Seminars in Hematology*, 45(3), 135-140.
- Gagnier, J.J. & Morgenstern, H. (2017). Misconceptions, Misuses, and Misinterpretations of P Values and Significance Testing. *JBJS*, 99(18), 1598-1603.
- American Statistical Association (2016). Statement on Statistical Significance and P-Values.
- Rafiei, M. (2026). Posts sobre p-valor e Minimum Effect Size em UX Research. LinkedIn/PUXLab.
- Benjamin, D.J. et al. (2018). Redefine statistical significance. *Nature Human Behaviour*, 2, 6-10. (72 coautores, proposta p < .005)
- Open Science Collaboration (2015). Estimating the reproducibility of psychological science. *Science*, 349(6251). (36% de replicação)

---

### 1.9 O que o Routledge revela (e não revela) sobre chi-quadrado em mixed analysis

O Routledge Reviewer's Guide to Mixed Methods Analysis (Onwuegbuzie & Johnson, 2021) é a referência mais completa do campo — 30 capítulos, autores de referência mundial. A leitura dos capítulos relevantes (6, 9, 10) revela um padrão: as ferramentas são tratadas como neutras.

#### Cap 6 — Collins: CHAID Analysis of Qualitative Data

Collins aplica CHAID a 593 undergraduates, 9 temas codificados binarizados (1/0), com 4 variáveis demográficas como preditoras. Usa Bonferroni pra múltiplas comparações. Reconhece instabilidade e bias inflado como limitações (Van Diepen & Franses, 2006: previsões podem ser "severely biased").

**O que não discute:** Nenhuma menção a pressupostos de independência violados por dados quali. Nenhuma reflexão sobre o que o p-valor significa quando temas foram codificados por um pesquisador. Nenhuma distinção entre o que a tree revela sobre o fenômeno vs. sobre o codificador. A binarização (1/0 por tema) descarta intensidade, contexto e nuance sem comentário epistemológico.

**A ironia:** Os resultados mais interessantes (gênero prediz "student-centered", etnicidade prediz "enthusiasm") são Q-mode — variáveis externas predizem perfis de codificação. São os mais "janela" do capítulo. Mas Collins não usa essa linguagem.

#### Cap 9 — Hitchcock et al.: HLM with Quantitized Data

**O achado mais importante do Routledge pra nossa discussão.** HLM existe porque a independência é violada em dados aninhados. Hitchcock articula: *"the idea that dependence is an interesting phenomenon"* (p.100). Dependência não é problema a corrigir — é fenômeno a investigar. ICC (Intra-class Correlation) mede quanta variância é compartilhada dentro de grupos.

Tradução pro nosso contexto: segmentos do mesmo participante são aninhados nesse participante. HLM modelaria essa dependência explicitamente — distinguindo variância entre participantes (janela) de variância dentro (potencialmente espelho). É o que von Foerster diz informalmente, formalizado em estatística.

**Mas:** HLM precisa de N grande nos dois níveis (≥5 Level-1 por cluster, ≥30 Level-2 clusters). Com 5 entrevistas, inviável. Mesma limitação de N que motivou a inversão da unidade de análise.

#### Cap 10 — Natesan Batley: Bayesian Analyses with Qualitative Data

Três vantagens que mapeiam diretamente pro espelho/janela:

1. **P(A|B) ≠ P(B|A):** Rejeitar H0 com base no p-valor é confundir P(dados|H0) com P(H0|dados). "If the sky looks cloudy it will certainly rain is the same as if it rains the sky must be cloudy. The first statement is wrong" (p.109). Formalização da Misconception #1 do Goodman.

2. **Posterior > point estimate:** A distribuição posterior dá forma completa da incerteza, não só sim/não. No contexto de associação entre códigos: não é "significativo?", é "com que força? com que incerteza? com que formato?"

3. **Prior information:** "Prior information may be obtained via previous research, researchers' educated guess about the parameter, historic data" (p.109). **Chave pra espelho/janela:** priors podem incorporar conhecimento sobre o codificador. A posterior estima associação descontando hábito.

#### O padrão nos 3 capítulos

| Capítulo | O que traz | O que falta |
|---|---|---|
| **Cap 6 (CHAID)** | Chi-quadrado aplicado, Bonferroni, exemplo empírico | Nenhuma reflexão epistemológica sobre pressupostos violados |
| **Cap 9 (HLM)** | "Dependência é fenômeno interessante", ICC | Inviável com N pequeno; não conecta com epistemologia |
| **Cap 10 (Bayesian)** | Prior information, P(A\|B) ≠ P(B\|A) | Não discute priors sobre o codificador |

Cada um tem uma peça do quebra-cabeça. Nenhum junta as peças.

#### O ponto cego estrutural do campo

O Routledge é a referência máxima de mixed analysis — e mesmo assim nenhum dos 30 capítulos questiona epistemologicamente o que acontece quando ferramentas estatísticas operam sobre codificação qualitativa. Todos tratam pressupostos como questão técnica.

Isso não é falha dos autores. É a natureza do campo: mixed methods nasceu pragmático ("funciona? resolve a pergunta? então usa"). O campo é voltado pra operacionalizar, não pra questionar os fundamentos das ferramentas que operacionaliza.

O ponto cego é estrutural — as comunidades não se cruzam:
- **Estatísticos** que conhecem pressupostos não trabalham com codificação qualitativa
- **Qualitativistas** que codificam não conhecem pressupostos profundamente
- **Mixed methodologists** juntam os dois mas tratam a ferramenta como neutra
- **Epistemólogos** (von Foerster, Latour) não falam de chi-quadrado

A posição que emerge desta costura — violação como informação, espelho/janela, taxonomia epistemológica por método — é uma **terceira via** entre "não use se os pressupostos não são satisfeitos" (purismo frequentista) e "use e interprete" (pragmatismo mixed methods). Propõe: **quando pressupostos são violados sistematicamente porque a natureza do dado não permite satisfazê-los, a violação é informação sobre a relação observador-observado**.

Defender isso exige background em estatística + epistemologia + prática de codificação + filosofia da ciência. É o que torna a posição simultaneamente forte (fundamentada em múltiplas tradições) e vulnerável (nenhuma comunidade isolada a reconhece como sua).

#### A combinação ideal (não existe em nenhum capítulo)

**Filosofia do HLM** (dependência é informação) + **mecânica do bayesiano** (priors capturam o codificador) + **geometria da ACM** (descreve sem testar) = o framework que nenhum capítulo do Routledge propõe mas que a costura conceitual deste projeto articula.

---

## 2. ACM

*Pendente. A ACM é o método mais fundamentado no CONCEPTUAL-SYNTHESIS.md — Benzécri, biplot, tradição francesa. Desenvolver aqui com a mesma profundidade do chi-quadrado, focando nos pressupostos específicos (independência de linhas, homogeneidade, categorias raras) e na ironia de que a ACM é o método que menos sofre por ser desenhado anti-pressupostos.*

---

## 3. Cluster

*Pendente.*

---

## 4. MDS

*Pendente.*

---

## 5. Sequential/Lag

*Pendente.*

---

## 6. Decision Tree (CHAID)

*Pendente.*

---

## 7. Frequência Descritiva

*Pendente.*

---

## Interações entre métodos

*Pendente. Exemplo: se chi-quadrado diz associação significativa entre dois códigos mas MDS os posiciona longe — o que isso revela? Pode indicar que coocorrem em frequência mas em contextos diferentes (clusters semânticos distintos). A divergência entre métodos é informação, não contradição.*

---

## Fontes

- CONCEPTUAL-SYNTHESIS.md — costura conceitual, distinção espelho/janela, violação de pressupostos como informação
- REFERENCES.md — 20 referências detalhadas (Péladeau R/Q-mode, Macia clustering, Driscoll colinearidade, etc.)
- THEORY-PRODUCT-MAPPING.md — mapeamento teoria→Qualia Coding
- Conversa "Data Classification and Types" (Claude.ai, 4/jun/2025) — von Foerster, mise en abyme, inversão da unidade
- Sessão "wiggly-sprouting-cupcake" (Claude Code, 24/mar/2026) — Péladeau, 20 refs, espelho/janela
- Sessão de genealogia do projeto (5/abr/2026) — articulação desta taxonomia
