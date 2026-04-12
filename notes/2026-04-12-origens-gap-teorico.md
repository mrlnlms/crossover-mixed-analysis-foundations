# Sessao Exploratoria: Origens do Mixed Methods, DIME, e o Gap Teorico para Dados de Interacao Humano-AI

**Data:** 12/abr/2026
**Contexto:** Sessao de exploracao teorica profunda partindo das fontes primarias do projeto Mixed Methods - Data Transformation, conectando com o AI Interaction Analysis (estudo longitudinal N=1 de interacao humano-AI, ~192k mensagens, 10 fontes, dez/2022-mar/2026).

---

## 1. Ponto de partida: o livro fundacional

**Fonte:** Onwuegbuzie & Johnson (2021). *The Routledge Reviewer's Guide to Mixed Methods Analysis.* Routledge.

Este e o primeiro livro dedicado exclusivamente a **mixed analysis** (analise mista). O capitulo 1 ("Mapping the Emerging Landscape of Mixed Analysis") estabelece:

- A analise e considerada a etapa **mais dificil** do processo de pesquisa mixed methods, mesmo por pesquisadores experientes
- Existem pelo menos 58 tecnicas quantitativas e 60 qualitativas de analise, gerando **3.480+ combinacoes** possiveis para uma analise mista simples
- A maioria das pesquisas "mixed methods" publicadas na verdade fazia **non-crossover analysis** — analisava QUAL e QUAN separadamente, sem integracao real
- O **Crossover Analysis Framework (CAF)** de Hitchcock e Onwuegbuzie (2020) organiza a analise cruzada em 4 tipos: QUAN-dominant, QUAL-dominant, equal-status, e inherently mixed

### A estrutura do livro:
- **Part I** — Quantitative Approaches to Qualitative Data (12 caps): factor analysis de texto, cluster analysis, MDS, correspondence analysis, regressao, SEM, HLM, Bayesian, IRT, diachronic analysis
- **Part II** — Qualitative Approaches to Quantitative Data (3 caps): qualitizing, coding techniques, discourse analysis
- **Part III** — "Inherently" Mixed Analysis Approaches (9 caps): ethnographic decision models, QCA, Q Methodology, SNA, social media analytics, GIS, nonverbal communication, joint displays
- **Part IV** — Use of Software (6 caps): QDA Miner, MAXQDA, Dedoose, ATLAS.ti, NVivo, SPSS

### Conceitos-chave do capitulo 1:
- **Tecnica (microanalysis)** = um passo atomico (calcular media, codificar in vivo)
- **Metodo (mesoanalysis)** = conjunto integrado de tecnicas (ANOVA, cross-case display)
- **Abordagem (macroanalysis)** = sistema amplo (grounded theory, analise descritiva)
- **Horizontal mixed analysis** = QUAL e QUAN em paralelo, so se encontram na interpretacao final
- **Vertical mixed analysis** = QUAL e QUAN interagem durante o processo de analise
- **1 + 1 = 1** (integracao total) vs **1 + 1 = 3** (integracao parcial que gera algo maior que as partes)

---

## 2. O refinamento de 2025: o modelo DIME

**Fonte:** Onwuegbuzie (2025). "On quantitizing revisited." *Frontiers in Psychology*, 15:1421525.

Construindo sobre Sandelowski et al. (2009) — "On Quantitizing" (1.000+ citacoes, *Journal of Mixed Methods Research*) — Onwuegbuzie propoe o **DIME-Driven Model of Quantitizing**: um meta-modelo hierarquico de 4 niveis.

### Os 4 niveis do DIME:

**Level 1 — DIME (os quatro tipos fundamentais):**
- **D**escriptive-based quantitizing: medidas de tendencia central, dispersao, posicao, forma distribucional
- **I**nferential-based quantitizing: t-test, ANOVA, regressao, SEM, HLM — testar hipoteses, fazer predicoes
- **M**easurement-based quantitizing: Rasch modeling, IRT — desenvolver instrumentos, validar construtos
- **E**xploratory-based quantitizing: factor analysis, cluster analysis, correspondence analysis, MDS — descobrir padroes latentes

**Level 2 — Spatial + Time:**
- Spatial: transformar dados qualitativos em formatos geoespaciais (GIS, cartografia)
- Time: quantitizar dados temporais (logistic regression de medidas repetidas, survival analysis, GEE, GLMM)

**Level 3 — Cross-sectional + Longitudinal:**
- Cross-sectional: quantitizar dados de um ponto no tempo
- Longitudinal: quantitizar dados de multiplos pontos temporais

**Level 4 — Retrospective + Prospective:**
- Retrospective: quantitizar dados qualitativos que ja existiam sem intencao original de pesquisa
- Prospective: coletar dados qualitativos ja com intencao de quantitizar desde o design

### As tabelas filosoficas (Tables 1-3):

O artigo mapeia sistematicamente a relacao entre **filosofia de pesquisa e propensao ao quantitizing** em tres tradicoes (~40 filosofias no total):

- **Filosofias qualitativas** (Table 1): social constructionism (skeptical), radical constructivism (rarely), critical theory (open), phenomenology (rarely, exceto neuro/eco-phenomenology), postmodernism (resists)
- **Filosofias quantitativas** (Table 2): platonismo, logicismo, empiricismo (high); nominalismo, intuicionismo (low)
- **Filosofias de mixed methods** (Table 3): pragmatism-of-the-middle, dialectical pluralism, critical dialectical pluralism, transformative-emancipatory (highly embraced); anti-conflationism (rarely)

### Insight central:
Quantitizing nao e uma tecnica neutra — e um **ato filosofico**. Cada filosofia tem uma relacao diferente com a ideia de transformar qualidade em quantidade. O DIME transforma o quantitizing de operacao vaga em **processo hierarquico com 4 niveis de complexidade crescente**.

---

## 3. O gap identificado: dados de interacao humano-AI

### O problema que ninguem formalizou:

O DIME assume que o dado qualitativo e de **primeira ordem** — alguem falou numa entrevista, respondeu survey, foi observado. O pesquisador pega esse dado e quantitiza.

Mas dados de interacao humano-AI sao ontologicamente diferentes:
- Nao sao entrevistas (nao ha entrevistador humano)
- Nao sao observacoes (nao ha fenomeno externo)
- Nao sao field notes (nao ha mediacao de memoria)
- Sao **traces digitais de co-construcao interpretativa assimetrica** — assimetrica porque um dos agentes e uma maquina

### A pergunta central do gap:

> **O que acontece com o quantitizing quando o dado qualitativo e ele mesmo produto de um processo interpretativo mediado por agente nao-humano?**

---

## 4. As bases teoricas do gap

### 4.1 Hermeneutica (Gadamer, Ricoeur, Giddens)

- **Gadamer (1960)**: toda compreensao e fusao de horizontes. Com AI, a fusao e **assimetrica** — um dos "horizontes" nao e genuinamente interpretativo
- **Ricoeur (1981)**: textos ganham autonomia semantica quando separados do autor. Conversas exportadas se separam da intencao de ambos os interlocutores
- **Giddens (1984)**: dupla hermeneutica — o pesquisador interpreta interpretacoes de atores sociais. Com AI, a estrutura hermeneutica se **multiplica e deforma**: interpretacao (pesquisador agora) de interpretacoes (pesquisador na epoca) de interacoes com agente que simula interpretacao (AI)

### 4.2 ANT — Actor-Network Theory (Latour, Callon, Pickering)

- **Latour (1987, 2005)**: principio de simetria generalizada — nao tratar humanos e nao-humanos diferentemente a priori. AI e **actante**, nao instrumento passivo
- **Callon (1986)**: traducao — processo de recrutamento de actantes. Quando AI "resume demais", esta falhando na traducao
- **Pickering (1995)**: "dance of agency" — alternancia entre resistencia material e acomodacao humana. Prompt refinement e essa danca

**Implicacao pro quantitizing:** Se AI e actante, os dados de interacao nao sao "dados sobre o humano mediados por ferramenta" — sao **dados sobre uma rede sociotecnica**. Quantitizar esses dados e quantitizar a rede, nao o individuo.

### 4.3 Cibernetica de segunda ordem (von Foerster, Maturana, Bateson)

- **Von Foerster (1974)**: o observador e parte do sistema observado. Autoethnografia quantitizada e **auto-observacao cibernetica**
- **Maturana & Varela (1980)**: autopoiese — sistemas que se produzem a si mesmos. O projeto gera interacoes que geram dados que geram analise que gera mais interacoes
- **Bateson (1972)**: informacao = "a diferenca que faz diferenca". Niveis de aprendizagem: o dataset mostra transicoes entre aprender tecnicas (nivel I), mudar enquadramento (nivel II), e questionar premissas (nivel III)

### 4.4 OOO — Object-Oriented Ontology (Harman, Morton, Bogost)

- **Harman (2011, The Quadruple Object)**: todo objeto se retira das suas relacoes. Quatro polos: Real Object (RO), Real Qualities (RQ), Sensual Object (SO), Sensual Qualities (SQ)
- O quantitizing opera **inteiramente no Eidos (SO-SQ)** — a superficie sensorial. O objeto real sempre escapa
- **Undermining** (reduzir a componentes: conversa → word_count) e **overmining** (reduzir a efeitos: conversa → topic) sao riscos simetricos. O pipeline faz ambos simultaneamente
- Os overrides sao tentativas de **corrigir undermining/overmining** quando nao correspondem a experiencia do pesquisador com o objeto real
- **Morton (2013)**: o corpus de 192k mensagens como **hiperobjeto** — massivamente distribuido, viscoso, nao-local, com ondulacao temporal
- **Bogost (2012)**: alien phenomenology — o que e "ser" uma AI numa conversa? Nem explicacao tecnica nem projecao antropomorfica

### 4.5 Pos-humanismo (Haraway, Hayles, Simondon, Stiegler)

- **Haraway (1985)**: o pesquisador-AI como figura **ciborgue** — cognicao na interface, nao no individuo
- **Hayles (1999)**: intermediacao — humanos e maquinas se co-constituem. O objeto do quantitizing e a **interface**, nao os termos
- **Simondon (1958)**: individuacao tecnica — plataformas nao sao abstratas, sao individuadas pelo uso
- **Stiegler (1994)**: memoria exossomatica **interativa** — as conversas sao memoria que respondia em tempo real

### 4.6 Barad e os cortes agenciais

- **Barad (2007)**: intra-acao (vs inter-acao) — entidades se constituem mutuamente no encontro. Cada topic, entity, override e um **corte agencial** que produz (nao descreve) as entidades estudadas

### 4.7 Sandelowski e Martin: a natureza do dado

- **Sandelowski (2009)**: data-as-given vs data-as-taken. Traces digitais sao **data-as-generated** — uma terceira categoria
- **Martin (2004)**: contar cria "individualidade ontologica" — cada conversation_id, topic, entity e um **corte ontologico**

### 4.8 Vygotsky e cognicao distribuida (Hutchins)

- **Vygotsky (1978)**: cognicao mediada por ferramentas culturais. Conversas com AI sao processos cognitivos distribuidos, nao registro de pensamento
- **Hutchins (1995)**: cognicao distribuida — o pensamento esta entre humano, AI, plataforma e contexto

### 4.9 Bourdieu: campo, habitus, capital

- **Campo**: as 10 plataformas formam um campo de interacao humano-AI com logicas proprias
- **Habitus**: a escolha de qual AI usar pra qual tarefa e **disposicional**, nao racional — incorporada por anos de uso
- **MCA como ontologia geometrica**: o espaco relacional das plataformas e **geometricamente real**, nao metaforico
- **Illusio**: a intensidade de uso revela investimento no jogo — por que 163 msgs sobre design de estudo no ChatGPT?
- **Reflexividade bourdieusiana radical**: objectivar o proprio habitus de interacao com AI usando AI

### 4.10 Design Research + OOO (Lindley, Akmal & Coulton, 2020)

- **Carpentry** (Bogost): o pipeline e um artefato que revela como objetos constituem seus mundos
- **Constelacoes** (via Benjamin): o Sankey e uma constelacao — padrao que emerge da posicao do observador
- **More-Than Human Centred Design**: design opera nas relacoes entre actantes, nao centrado no humano
- **Heterotopia** (Foucault): cada plataforma de AI e um mundo-dentro-do-mundo com regras proprias
- **Analogia OOP ↔ OOO**: o schema do pipeline (dataclasses Python) JA E uma ontologia orientada a objetos

---

## 5. Qualitizing: o caminho inverso

O livro de 2021 (cap. 13) e Onwuegbuzie & Hitchcock (2020) argumentam: **quantitizing sempre implica qualitizing**. Nao sao processos separados — sao interdependentes. Formula: 1 + 1 = 1.

### Qualitizing no projeto AI Interaction Analysis:
- Nomear entities (clusters → "Sicredi", "GT Mixed Analysis")
- Os 3 modos (atomico, atomico+fases, balde) — categorias qualitativas descrevendo a natureza do grupo
- A timeline — timestamps → narrativa genealogica
- Streamgraphs — series temporais → leitura de "eras"
- Overrides — correcoes pontuais = **decisoes interpretativas**

### Qualitizing profundo (ainda nao formalizado):
- Transformar padroes de `duration_ms` em narrativas de experiencia (sessao fluida vs trabalhosa)
- Transformar curva de `word_count` ao longo de 3 anos em **biografia da relacao** com AI
- Transformar proporcao human_ai/ai_ai em historia de **confianca e delegacao**

---

## 6. "Qualitative minus Qualia": o nome do risco

### Origem:
Comentario sobre estudo da Anthropic (mar/2026) que entrevistou ~80k pessoas usando Claude como entrevistador e classificador. Critica em tres palavras: **qualitative minus qualia** — tem a forma de pesquisa qualitativa mas sem a qualidade experiencial subjetiva que da a pesquisa qualitativa seu valor.

### Mecanismo:
As **4 ilusoes de compreensao** (Messeri & Crockett, 2024, *Nature*; expandidas por Garcia Quevedo, Glaser & Verzat, 2025):
1. **Ilusao de profundidade**: estrutura do output confundida com compreensao
2. **Ilusao de abrangencia**: sugestoes algoritmicas confundidas com cobertura
3. **Ilusao de objetividade**: outputs de AI percebidos como neutros
4. **Ilusao de relevancia**: facilidade de gerar substitui dificuldade de pensar

### Conexao com synthetic users/surveys:
- **Chapman (2024-2026)**: "Synthetic Survey Data? It's Not Data" — nao ha realidade externa que dados sinteticos representem
- **Samoylov**: respostas dependem do prompt, nao do "respondente" (renda media de $111k a $272k so mudando wording)
- **PNAS (2025)**: a premissa de que resposta coerente = resposta humana nao e mais sustentavel
- Uso exploratorio (nivel E do DIME) e aceitavel com consciencia; uso inferencial/descritivo/de mensuracao e problematico

### Implicacao pro gap:
O DIME precisa de um **marcador de proveniencia** no dado: nao so "e qualitativo ou quantitativo?" mas **"foi produzido por agente com qualia ou sem?"**

---

## 7. Dados de segunda ordem e mediacao tecnica

### O problema das camadas:
- **Camada 0**: interacao vivida (inacessivel — o objeto real se retirou)
- **Camada 1**: registro da plataforma (primeira ontologizacao — a plataforma cortou)
- **Camada 2**: exportacao (format shift de live para arquivo)
- **Camada 3**: parsing (segunda ontologizacao — o pesquisador unificou)
- **Camada 4**: enrichment (terceira ontologizacao — topics, entities, hierarquia)
- **Camada 5**: quantitizing (transformacao — frequencias, distribuicoes, modelos)

O DIME assume Camada 1 → 5. No AI Interaction Analysis, opera da **Camada 3 → 5**, e as Camadas 1-2 ja carregam decisoes de design da plataforma que condicionam tudo.

### Implicacao:
**O que pode ser quantitizado ja foi pre-determinado pelas decisoes de design da plataforma.** Se o ChatGPT nao exporta tempo de reflexao, essa dimensao esta irrecuperavelmente perdida.

---

## 8. O que a academia esta discutindo agora (2025-2026)

| Artigo | O que discute | O que falta |
|---|---|---|
| Machine-Assisted Quantitizing Designs (Nature, 2025) | LLMs como assistentes de quantitizing | AI como **co-produtora** dos dados |
| Chatzichristos (2025, IJQM) | AI empurra QUAL de volta ao positivismo? | Conexao com DIME |
| Meta-crise da generatividade (Frontiers, 2025) | 3 crises: representacao, legitimacao, praxis | Conexao com OOO, withdrawal |
| "Analyzing or Just Chatting?" (Nguyen & Welch, 2026) | Pesquisadores analisam ou conversam com chatbot? | Dados co-produzidos com AI |
| AI and the End(s) of QDA (Human Organization, 2025) | LLMs sao maquinas de mimese, nao de estranhamento | Bourdieu, habitus, campo |
| Synthetic participants review (2025-2026) | Synthetic users nao funcionam | Quando/por que funcionam (nivel E) |
| Scaling Hermeneutics (EPJ Data Science, 2025) | Codificacao qualitativa com LLMs | Questao ontologica, nao so pragmatica |
| PNAS — Threat of LLMs to survey research (2025) | Contaminacao involuntaria de surveys | Marcador de proveniencia |

### A sintese que ninguem fez:
DIME (Onwuegbuzie) + OOO (Harman) + cibernetica 2a ordem (von Foerster) + ANT (Latour) + campo/habitus (Bourdieu) + qualia como criterio epistemologico + dados humano-AI como tipo ontologicamente novo + familiar/exotico (DaMatta) + reflexividade (Cunliffe) + autoethnografia analitica (Anderson)

---

## 9. Enquadramento metodologico: autoethnografia analitica + autotecnografia

### Por que autoethnografia:
- O pesquisador e o unico que TEM os qualia das interacoes
- Irreprodutibilidade e **constitutiva**, nao limitacao (Ellis, Le Roux, Richardson)
- Validade por credibilidade, transferibilidade, confirmabilidade, autenticidade — nao por replicabilidade

### Por que analitica (Anderson, 2006):
1. Pesquisador e membro completo do fenomeno
2. Reflexividade analitica (nao apenas narrativa)
3. Visibilidade narrativa do pesquisador nos dados
4. Dialogo com "informantes" (AIs como informantes de tipo novo)
5. Compromisso com construcao de teoria

### Por que autotecnografia:
- Foco especifico na relacao com tecnologia
- Dados sao traces digitais + memorias + narrativas
- O corpo + o dispositivo como instrumento de coleta
- Reflexividade sobre posicao social E tecnica

### A dialetica familiar/exotico (DaMatta, Velho, Shklovsky):

O desafio central: tecnologia digital e projetada para ser **transparente** — desaparece no uso. 3 anos de interacao com AI criam hiperfamiliaridade (habitus bourdieusiano). A tendencia e achar que ja sabe o que esta nos dados porque viveu.

O **pipeline como dispositivo de estranhamento** (ostranenie computacional):
- Transforma conversas vividas em padroes visiveis
- Revela distribuicoes invisiveis na experiencia cotidiana
- Descobre agrupamentos que o pesquisador nao organizou conscientemente

Os **overrides como familiarizacao do exotico**:
- Mobilizam qualia (memoria, recall) para corrigir quando o estranhamento distorce
- "Nao, eu sei o que isso e, eu estava la"

O ciclo:
```
Experiencia vivida (familiar)
    → pipeline (estranhamento)
Dados, padroes, visualizacoes (exotico)
    → override (familiarizacao)
Categorizacao corrigida (novo familiar informado pelo exotico)
    → novo padrao emerge (novo estranhamento)
    → ciclo iterativo
```

### Criterios de validade:

| Criterio | Manifestacao no projeto |
|---|---|
| Credibilidade | Traces exaustivos: 192k msgs parseadas, verificaveis, com timestamps |
| Transferibilidade | Insights sobre quantitizing-com-qualia vs sem-qualia se aplicam a qualquer pesquisador que use AI |
| Confirmabilidade | Pipeline e codigo. Parquets auditaveis. Overrides documentados |
| Autenticidade | So o pesquisador pode testemunhar a withdrawal e resistir as ilusoes |
| Profundidade temporal | 3.3 anos (estudos existentes: semanas) |
| Abrangencia de fontes | 10 plataformas (estudos existentes: 1) |
| Reflexividade documentada | Metodologia de granularidade assimetrica, 8 mecanismos de override |

---

## 10. Referencias-chave

### Fontes primarias do projeto:
- Onwuegbuzie, A. J. & Johnson, R. B. (Eds.) (2021). *The Routledge Reviewer's Guide to Mixed Methods Analysis.* Routledge.
- Onwuegbuzie, A. J. (2025). On quantitizing revisited. *Frontiers in Psychology*, 15:1421525.
- Sandelowski, M., Voils, C. I., & Knafl, G. (2009). On quantitizing. *Journal of Mixed Methods Research*, 3(3), 208-222.

### Hermeneutica:
- Gadamer, H.-G. (1960). *Truth and Method.*
- Ricoeur, P. (1981). *Hermeneutics and the Human Sciences.*
- Giddens, A. (1984). *The Constitution of Society.*

### ANT e agencia:
- Latour, B. (2005). *Reassembling the Social.*
- Callon, M. (1986). Some elements of a sociology of translation.
- Pickering, A. (1995). *The Mangle of Practice.*

### Cibernetica:
- Von Foerster, H. (1984). *Observing Systems.*
- Maturana, H. & Varela, F. (1980). *Autopoiesis and Cognition.*
- Bateson, G. (1972). *Steps to an Ecology of Mind.*

### OOO:
- Harman, G. (2011). *The Quadruple Object.*
- Morton, T. (2013). *Hyperobjects.*
- Bogost, I. (2012). *Alien Phenomenology.*

### Pos-humanismo:
- Haraway, D. (1985). A Cyborg Manifesto.
- Hayles, N. K. (1999). *How We Became Posthuman.*
- Simondon, G. (1958). *Du mode d'existence des objets techniques.*
- Stiegler, B. (1994). *La technique et le temps.*

### Agential realism:
- Barad, K. (2007). *Meeting the Universe Halfway.*

### Natureza do dado:
- Martin, E. (2004). Counting as ontological act.
- Geiger, R. S. & Ribes, D. (2011). Trace ethnography.

### Cognicao distribuida:
- Vygotsky, L. (1978). *Mind in Society.*
- Hutchins, E. (1995). *Cognition in the Wild.*

### Bourdieu:
- Bourdieu, P. (1979). *La Distinction.*
- Bourdieu, P. (1984). *Homo Academicus.*

### Design Research + OOO:
- Lindley, J., Akmal, H. A. & Coulton, P. (2020). Design Research and Object-Oriented Ontology. *Open Philosophy*, 3(1).

### Estranhamento:
- DaMatta, R. (1978). O oficio do etnologo.
- Velho, G. (1978). Observando o familiar.
- Shklovsky, V. (1917). A arte como procedimento.

### Ilusoes e reflexividade:
- Messeri, L. & Crockett, M. J. (2024). AI and illusions of understanding. *Nature*, 627, 49-58.
- Garcia Quevedo, D., Glaser, A. & Verzat, C. (2025). Fast answers, shallow thinking. ESCP Impact Paper 2025-23.
- Cunliffe, A. L. (2004, 2016). On becoming a critically reflexive practitioner.

### Autoethnografia:
- Ellis, C., Adams, T. E. & Bochner, A. P. (2011). Autoethnography: An overview.
- Anderson, L. (2006). Analytic autoethnography. *Journal of Contemporary Ethnography*, 35(4), 373-395.
- Richardson, L. (2000). Writing: A method of inquiry.
- Le Roux, C. S. (2017). Exploring rigour in autoethnographic research.

### AI e pesquisa qualitativa (2025-2026):
- Machine-assisted quantitizing designs. *Humanities and Social Sciences Communications* (Nature, 2025).
- Chatzichristos, G. (2025). Qualitative Research in the Era of AI. *IJQM*.
- Nguyen, D. C. & Welch, C. (2026). Analyzing—Or Just Chatting? *Organizational Research Methods*.
- AI and the End(s) of Qualitative Data Analysis. *Human Organization* (2025).
- The potential existential threat of LLMs to online survey research. *PNAS* (2025).
- Scaling hermeneutics. *EPJ Data Science* (2025).

### Synthetic data:
- Chapman, C. (2026). Synthetic Survey Data? It's Not Data. Sawtooth/Quant UX.
- Samoylov, N. (2024). Synthetic Respondents are the Homeopathy of Market Research.

### Tecnologia e self:
- Turkle, S. (2011). *Alone Together.*
- Lupton, D. (2021). Autotechnography approaches.
