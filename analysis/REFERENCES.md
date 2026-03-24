# References — Mixed Methods: Data Transformation

Referências bibliográficas do projeto, com discussão detalhada de cada leitura.

---

## 1. Macia, L. (2015). Using Clustering as a Tool: Mixed Methods in Qualitative Data Analysis

**Fonte:** The Qualitative Report, 20(7), 1083-1094.
**Arquivo:** `./GTQQ/Using Clustering as a Tool - Mixed Methods in Qualitative Data Analysis.pdf`

| | |
|---|---|
| **Autora** | Laura Macia |
| **Instituição** | University of Pittsburgh |
| **País** | EUA |
| **Ano** | 2015 |
| **Journal** | The Qualitative Report |
| **Setor/Contexto** | Antropologia / Imigração / Saúde pública — queixas de imigrantes latinos no sudoeste da Pensilvânia |
| **Tipo** | How-to prático com case study |

### Resumo
How-to prático de cluster analysis hierárquica aplicada a dados qualitativos codificados. Case study: projeto sobre queixas (grievances) de imigrantes latinos no sudoeste da Pensilvânia — 21 entrevistas em profundidade, 195 casos codificados no Atlas.ti.

### Problema
Quando o volume de dados codificados é grande demais pra análise manual confiável (195 casos × 12 variáveis), ferramentas de QDA (co-ocorrências, buscas booleanas) não dão conta sem viés do pesquisador. Cluster analysis entra como ferramenta **exploratória** pra organizar os casos em grupos e guiar o retorno aos dados qualitativos.

### Os 3 passos-chave
1. **Data transformation** — dados qualitativos nominais/ordinais viram matriz binária (0/1 por atributo). Uma variável "suporte" com 6 valores vira 6 colunas binárias. Resultado: 59 variáveis binárias + 1 escalar.
2. **Escolha de método e medida de similaridade** — clustering hierárquico aglomerativo com medida Dice (para dados assimétricos onde presenças importam mais que ausências).
3. **Seleção do número de clusters** — testou 3 a 8 clusters, escolheu 7 via análise qualitativa das soluções (sem breakpoint estatístico claro).

### Ciclo completo
Codifica no Atlas.ti → exporta pra SPSS → transforma em binário → clusteriza → cross-tabula com variáveis excluídas do clustering (tipo de queixa, gênero, outcome) → **volta pros dados qualitativos** usando cluster membership como lente.

### Ponto central
Clustering é ferramenta **exploratória**, não substitui análise qualitativa. O valor está em criar um framework estruturado pra revisitar os dados qualitativos com mais foco. A Table 7 (cluster membership → broad characteristics) é o bridge entre quanti e quali.

### Variáveis do estudo (Table 1)
A pesquisadora codificou cada caso de queixa com 12 variáveis organizadas em 4 blocos:

**Bloco 1 — Quem sofreu a queixa (Part 1 / aggrieved):**
- When: anos desde a ocorrência
- Gender: masculino/feminino
- Strata: blue-collar / spouse of American citizen / white-collar
- Legal status: US citizen, residente permanente, visto de imigrante, non-immigrant visa, visa overstay, indocumentado
- Income: 6 faixas (under $20k a over $100k)
- Education: primary a graduate degree

**Bloco 2 — Quem causou a queixa (Part 2 / grieving party):**
- Type: individual (masc/fem/unknown), instituição, governo, outro
- Nationality: americano, latino, outro, desconhecido

**Bloco 3 — A queixa em si:**
- Grievance type: debt, discrimination, domestic, law

**Bloco 4 — Como a pessoa reagiu:**
- Procedural mode: 11 opções — adjudicação, arbitragem, mediação, negociação, coerção, evitar, *lumping it* (engolir), *assumed fault*, *talk back*, outro, nenhum
- Support sought: nenhum, família, amigo, service provider, igreja, outro
- Resolution: nenhuma, favorável ao queixoso, favorável ao outro, mista, outro

**Transformação:** As variáveis nominais foram binarizadas (cada valor possível virou uma coluna 0/1). Resultado: 59 variáveis binárias + 1 escalar (tempo). Para o clustering, excluiu variáveis demográficas (determinadas pelo research design) e usou apenas: características da parte causadora, modos procedurais, fontes de suporte.

### Resultados — O que os 7 clusters revelaram

**Grupo 1 (85 casos — o maior): "Cada um por si"**
Maioria de problemas domésticos. Reação mais comum: *lumping it* (engolir) ou negociar sozinho. Quase ninguém buscou apoio. São as queixas que as pessoas acharam que não valiam o esforço, ou se sentiram impotentes pra resolver.

**Grupo 2 (38 casos): "Os devedores"**
Quase tudo dívida, especialmente contra instituições. Estratégia: negociar ou evitar. Brancos desse grupo tendiam a se sair melhor — interpretação: mais familiaridade com o sistema americano de "reclamar e negociar".

**Grupo 3 (18 casos): "Problemas com a lei"**
Maioria homens (dirigiam mais → mais multas). Resolução via adjudicação formal (tribunais) ou assumir culpa. Grupo definido pelo gênero e pela natureza legal.

**Grupo 4 (10 casos): "Os resignados"**
Problemas sérios (domésticos + discriminação), quase nenhuma ação — *lumping it*, sem negociação, sem coerção. No retorno qualitativo, dois perfis: quem achava que não valia a pena, e quem sentia que qualquer ação seria inútil (impotência).

**Grupo 5 (25 casos): "Os que lutaram de tudo quanto é jeito"**
Maior diversidade de estratégias — negociação, mediação, assumir culpa, evitar, tudo junto. Mais buscaram apoio (família, amigos, serviços). Descoberta qualitativa: eram casos onde a pessoa se importava profundamente com o relacionamento — queria resolver SEM destruir o vínculo.

**Grupo 6 (16 casos): "Os confrontadores"**
Também domésticos + discriminação (parecido com grupo 5), mas abordagem oposta: evitar, falar grosso, coerção. Ninguém assumiu culpa. Eram situações com estranhos ou relacionamentos já destruídos — não havia vínculo pra preservar. 4 dos 6 casos domésticos envolviam violência.

**Grupo 7 (3 casos): "Os inclassificáveis"**
Outliers que resistiram a ser fundidos mesmo reduzindo pra 3 clusters. Complexidade extrema e dificuldade de categorização — a pesquisadora tinha memos longos debatendo consigo mesma sobre como classificá-los.

**Insight central:** O contraste entre grupos 5 e 6 é o achado mais poderoso — mesmos tipos de queixa, perfis demográficos parecidos, mas estratégias opostas. Sem clustering, ficariam no mesmo bolo de "problemas domésticos e discriminação". O agrupamento revelou que a **relação com a outra pessoa** (não o tipo de problema) definia a resposta. O quanti organizou; o quali explicou.

### Discussão — A decisão de excluir variáveis do clustering

Das 12 variáveis originais, ela **não usou todas** pra agrupar. Separou em dois conjuntos com funções completamente diferentes:

**Usadas no clustering (variáveis de ação/resposta):**
- Quem causou a queixa (tipo + nacionalidade da parte causadora)
- Como a pessoa reagiu (modo procedural — negociou, evitou, coagiu...)
- Se buscou apoio (família, amigo, serviço, igreja...)

**Excluídas do clustering (variáveis demográficas/contextuais):**
- Gênero, renda, educação, status legal, estrato social da pessoa que sofreu
- Tipo de queixa (dívida, discriminação, doméstico, lei)
- Resultado/resolução

#### Por que essa separação?

As variáveis demográficas eram **determinadas pelo research design**. Ela recrutou por estrato (white-collar, blue-collar, spouse of American citizen). Se jogasse gênero e estrato dentro do clustering, o computador ia agrupar "todas as mulheres blue-collar" juntas simplesmente porque compartilham essas características por construção da amostra — não porque tiveram experiências parecidas. Isso inflaciona semelhanças artificiais.

Então ela fez o inverso: agrupou **só pelo que as pessoas fizeram** (como reagiram, quem procuraram, que estratégias usaram). Os clusters são grupos de **comportamento**, não de perfil demográfico.

#### E depois usou as variáveis excluídas como lente de interpretação

Com os clusters formados, ela fez cross-tabulação com as variáveis que tinha excluído. Perguntou:

- "Esse cluster que agrupa pessoas que negociam e buscam apoio... tem mais de qual gênero? De qual estrato? Que tipo de queixa predomina?"
- "Esse cluster de pessoas que engoliam e não faziam nada... o resultado era favorável ou não?"

É como se o clustering desse a **estrutura** (esses casos se parecem), e as variáveis excluídas dessem o **significado** (e essas pessoas que se parecem são principalmente mulheres blue-collar lidando com discriminação).

#### O teste estatístico de validação

Ela usou chi-quadrado (χ²) pra verificar se a distribuição das variáveis excluídas nos clusters era significativa ou aleatória:
- Tipo de queixa vs. cluster: χ² = 211.551, p = .000 — altamente significativo
- Outcome vs. cluster: χ² = 42.626, p = .011
- Gênero vs. cluster: χ² = 11.459, p = .075 (marginalmente significativo)

Ou seja, os clusters capturam diferenças reais no tipo de problema e no resultado, **mesmo sem essas variáveis terem participado do agrupamento**. Isso valida que os padrões de comportamento estão de fato associados a tipos de situação — não é acaso.

#### Por que isso importa como decisão de design (para ferramentas de análise)

Se uma ferramenta de QDA vai oferecer clustering analítico, essa lógica de **separar variáveis de agrupamento vs. variáveis de interpretação** é uma decisão que o pesquisador precisa poder fazer. Não é "jogue tudo e clusterize" — o pesquisador precisa escolher:
1. O que define semelhança entre casos (variáveis de clustering)
2. O que explica os grupos depois (variáveis de interpretação via cross-tab)

Essa separação é o que transforma clustering de uma ferramenta estatística genérica numa ferramenta de **descoberta qualitativa**. Sem ela, os clusters refletem o research design; com ela, refletem padrões emergentes nos dados.

### Qualitização implícita no estudo

A Macia não usa o termo "qualitização" em nenhum momento do paper. Mas o estudo inteiro termina com um ato de qualitização: ela pega os 7 clusters (output numérico de um processo estatístico) e transforma cada um em **retrato narrativo** — "os resignados", "os confrontadores", "os que lutaram de tudo". A Table 7 (cluster membership → broad characteristics) é literalmente uma tabela de qualitização: números de cluster viram perfis verbais com tipo de queixa predominante, modo procedural, fontes de suporte, resolução típica.

Mais ainda: a **interpretação comparativa** entre clusters 5 e 6 — "mesmos tipos de queixa, estratégias opostas, o que os diferencia é o vínculo com a outra pessoa" — é qualitização de alto nível. Ela está atribuindo significado qualitativo a uma diferença que só foi visível por meio da estrutura numérica.

Isso é comum em pesquisa aplicada (pesquisa de mercado, segmentação de consumidor, UX research com personas data-driven) — nomear clusters e criar perfis narrativos é prática disseminada, mas quase nunca chamada de "qualitização". O campo dos métodos mistos dá nome a algo que muitos pesquisadores fazem intuitivamente.

### Nota sobre a codificação

A Macia usou **as duas abordagens** de codificação juntas:
- **Dedutiva (top-down / a priori):** códigos predefinidos vindos da literatura sobre tipos de queixas e modos procedurais de resolução de conflitos
- **Indutiva (bottom-up / emergente / grounded):** códigos data-driven que surgiram das entrevistas. Na Table 1, os itens marcados com asterisco (*assumed fault*, *talk back*) não estavam no framework teórico original — emergiram dos dados

Sobre os 195 casos de 21 pessoas: cada entrevistada contou múltiplas histórias de queixas. Uma pessoa podia ter 3 casos de discriminação, 2 de dívida e 1 doméstico. A **unidade de análise é o caso de queixa, não a pessoa**. Por isso 21 entrevistas viraram 195 casos (média ~9 queixas por pessoa).

### Conexão com obsidian-qualia-coding
O plugin já implementa parte desse pipeline na seção de analytics. Este paper traz insights pra iterar e melhorar — especialmente:
- O passo de data transformation (binarização de variáveis nominais/ordinais)
- A escolha de medidas de similaridade adequadas pro tipo de dado qualitativo (Dice para dados assimétricos)
- A separação entre variáveis de agrupamento e variáveis de interpretação como feature de UX — o pesquisador precisa poder fazer essa escolha no plugin

---

## 2. Morin, A. (2006). Intensive Use of Factorial Correspondence Analysis for Text Mining: Application with Statistical Education Publications

**Fonte:** ICOTS-7 (International Conference on Teaching Statistics), 2006.
**Arquivo:** `./GTQQ/Intensive use of factorial correspondence analysis for text mining - application with statistical education publications.pdf`

| | |
|---|---|
| **Autora** | Annie Morin |
| **Instituição** | IRISA, Université de Rennes 1 |
| **País** | França |
| **Ano** | 2006 |
| **Conferência** | ICOTS-7 (International Conference on Teaching Statistics) |
| **Setor/Contexto** | Estatística / Educação — text mining de publicações acadêmicas em educação estatística |
| **Tipo** | Demonstração metodológica com dois corpora |

### Resumo
Paper da Annie Morin (IRISA, Université de Rennes 1, França) sobre usar Análise de Correspondência (AC) fatorial como ferramenta de text mining. Ela é ao mesmo tempo pesquisadora e professora do método. Aplicado em dois corpora de publicações acadêmicas de educação estatística, com um objetivo duplo: demonstrar a AC pra text mining e analisar o campo onde ela própria atua.

### Problema
Você tem centenas de documentos textuais e quer descobrir quais temas existem ali, como se agrupam, e como os documentos se relacionam entre si. Mas textos são politematicos — um artigo pode falar de 3 assuntos ao mesmo tempo. Clustering tradicional força cada documento num grupo só. A AC não: ela cria um mapa contínuo onde documentos podem estar entre temas.

### Contexto dos dados

**SERJ — Statistics Education Research Journal (144 textos, 2002-2003):**
Revista acadêmica de **pesquisa** sobre ensino de estatística. De cada edição ela pegou não só os artigos, mas também abstracts, introduções, resumos de dissertações e publicações recentes. Mix heterogêneo de tipos de texto — paper completo, nota curta de 1 parágrafo sobre uma tese, resenha. Essa heterogeneidade explica por que os temas se misturam tanto no resultado: os documentos são diversos por natureza. Após filtrar (stopwords, frequência mínima): **464 palavras**, **140 documentos**.

**JSE — Journal of Statistics Education (247 abstracts, 1993-2005):**
Revista mais focada em **prática de ensino** — relatos de experiência, atividades de sala de aula, datasets educacionais. Só abstracts (textos curtos e objetivos), de um período muito maior (12 anos vs. 2 da SERJ). Após filtrar: **576 palavras**, **224 documentos**.

A escolha desses dois corpora não é acidental — são tipos de texto fundamentalmente diferentes (papers completos heterogêneos vs. abstracts curtos e focados), e isso produz resultados radicalmente diferentes na AC, ilustrando o que o método consegue e onde ele brilha.

### Método — como funciona (pra leigo)

**A tabela de contingência léxica (o input):**
Imagina uma tabela gigante: nas linhas estão os documentos, nas colunas estão as palavras. Cada célula diz quantas vezes aquela palavra aparece naquele documento. As palavras mais frequentes são previsíveis (statistics, students, data, teaching...), mas o que importa é a **co-ocorrência** — quais palavras aparecem juntas nos mesmos documentos.

**O que a AC faz:**
Pega essa tabela e projeta tudo — documentos E palavras — num mesmo mapa 2D (ou 3D, ou quantas dimensões quiser). Nesse mapa:
- **Palavras que aparecem juntas nos mesmos documentos** ficam próximas
- **Documentos que usam vocabulário parecido** ficam próximos
- **Oposições temáticas** aparecem como polos opostos nos eixos

Tecnicamente, a AC decompõe a tabela em **eixos** ordenados por quanto da variação total explicam. O primeiro eixo captura a maior oposição temática do corpus, o segundo a segunda maior, e assim por diante. Ela manteve 30 eixos.

**O conceito de metakeys (a sacada principal):**
Cada eixo tem dois polos (positivo e negativo). As palavras com maior contribuição em cada polo formam uma **metakey** — um grupo temático emergente. Com 4 eixos, até 8 metakeys. Uma palavra pode participar de várias metakeys, e um documento pode estar entre metakeys. Não existe a forçação de "esse documento pertence a esse cluster e pronto".

A Morin vai além: depois de identificar as metakeys, faz uma **segunda AC** cruzando metakeys entre si, revelando como os temas se misturam nos documentos.

**Diferença crucial pro clustering da Macia:**
No clustering, cada caso vai pra UM grupo. Na AC, um documento fica num ponto do mapa que pode estar entre vários temas. É a diferença entre "esse artigo é sobre ensino" (cluster) e "esse artigo está 60% no tema ensino e 40% no tema tecnologia" (AC).

### Resultados

**SERJ — O corpus politematico:**
Os papers eram misturados, com sobreposição de assuntos. No mapa, 4 temas emergiram no plano principal:
- Research / Conferences / PhD
- Computer / Performance / Spreadsheet
- Literacy / Society
- Data / Reasoning / Tables / Statistics

Mas com sobreposição significativa — os documentos não se separavam limpo. É o caso típico (a Figure 2 do paper mostra a forma de funil/cone). Isso não é falha do método — é o método revelando que o corpus é genuinamente politematico.

**JSE — O corpus monotematico:**
Resultado que a própria autora chamou de "surpreendente e interessante". Os abstracts eram tão focados que formaram blocos diagonais limpos na tabela de contingência — quase clusters perfeitos, sem sobreposição:
- Eixo 1: definido por "Teaching bits" (atividades pontuais de sala de aula)
- Eixo 2: definido por dados específicos (baseball, bodyweight — datasets educacionais)
- Eixo 3: datasets em geral
- Eixo 4: educação, currículo, aprendizagem, raciocínio

A explicação: abstracts são curtos e focados, e a JSE publica muitos "teaching bits" (atividades com um dataset específico) que são naturalmente monotemáticos. Raro ver isso em dados textuais reais.

**Aplicação em doenças raras:**
A Morin também menciona uso pra selecionar bibliografia médica — pesquisadores indicam o que leem, a AC extrai o vocabulário característico do campo, e isso filtra publicações relevantes espalhadas em revistas de diversas áreas. Um caso de text mining pra curadoria bibliográfica.

### Discussão — Diferenças e complementaridade com clustering

A AC e o clustering hierárquico (Macia) atacam problemas relacionados mas com abordagens opostas:

**Natureza do input:** A Macia parte de dados **já codificados** pelo pesquisador (variáveis estruturadas com valores definidos). A Morin parte de **texto bruto** — o método descobre os temas sem codificação prévia.

**Natureza do output:** O clustering produz **grupos exclusivos** — cada caso pertence a um cluster. A AC produz um **mapa contínuo** — cada documento tem uma posição que pode estar entre múltiplos temas. A AC preserva a ambiguidade; o clustering a resolve (às vezes forçadamente).

**Quando cada um brilha:** Clustering é melhor com dados discretos bem definidos (códigos, variáveis categóricas). AC é melhor com corpus textual grande onde documentos são politematicos e você quer descobrir a estrutura temática sem impor categorias prévias.

**Limitação compartilhada:** Ambos precisam de interpretação humana. O clustering agrupa mas não explica — a Macia precisou voltar aos dados qualitativos. A AC mapeia mas não nomeia — a Morin precisou de experts do domínio pra rotular as metakeys.

**O ponto de convergência:** A AC pode ser usada **antes** da codificação (pra entender a estrutura temática do corpus e informar o codebook), e o clustering **depois** (pra agrupar os dados codificados e descobrir padrões). São pipelines complementares, não concorrentes.

### O que o resultado vira na prática

O resultado da AC **não são códigos** — é algo anterior. É uma **cartografia temática** do corpus. Concretamente, se você roda AC nos ~30 papers deste projeto, o resultado é um mapa onde papers com vocabulário parecido ficam juntos e os eixos revelam as oposições temáticas.

O valor prático é triplo:

1. **Descoberta de estrutura:** Você enxerga quais subtemas existem antes de ter lido tudo em detalhe. "Tem um cluster de papers sobre binarização, outro sobre medidas de similaridade, outro sobre visualização" — coisas que talvez não tivesse nomeado conscientemente.

2. **Identificação de lacunas:** Se o mapa mostra 4 temas e um tem só 2 papers enquanto os outros têm 6-8, sugere um gap na cobertura bibliográfica. Pode ser intencional ou não.

3. **Ponte pra codificação:** As metakeys podem **informar** códigos, mas não são códigos prontos. São categorias temáticas sugeridas pelos dados que o pesquisador pode usar pra construir ou refinar o codebook. Passo intermediário: AC mapeia o terreno → pesquisador olha → decide quais temas viram códigos → aplica nos textos.

### Qualitização implícita no estudo

A Morin também não usa o termo "qualitização". Mas o processo de **nomear metakeys** é um ato de qualitização puro: o método produz eixos numéricos com contribuições estatísticas, e a pesquisadora (junto com experts do domínio) transforma isso em rótulos temáticos — "Research/Conferences/PhD", "Computer/Performance/Spreadsheet", "Literacy/Society".

A segunda AC (cruzando metakeys entre si) é ainda mais explícita: ela pega agrupamentos estatísticos de palavras e cria **descrições verbais de como os temas se misturam nos documentos**. É transformação de output numérico em narrativa interpretativa.

O caso da aplicação em doenças raras é talvez o mais claro: pesquisadores do campo médico indicam publicações relevantes → a AC extrai vocabulário estatisticamente característico → os pesquisadores **nomeiam e validam** esses vocabulários como pertencentes ao campo. O ciclo completo: quali (seleção expert) → quanti (AC) → quali (validação e nomeação).

A diferença em relação à Macia: na Macia, a qualitização acontece **depois** do clustering, sobre grupos discretos. Na Morin, a qualitização acontece **durante** a interpretação, sobre um espaço contínuo. São dois modos distintos de qualitizar: nomeação de categorias (Macia) vs. interpretação de paisagem (Morin).

### Conexão com obsidian-qualia-coding
Para o plugin, são dois pipelines analíticos distintos:
1. **Pipeline Morin (AC):** parte do corpus bruto → descobre temas → mapa contínuo. Útil pra exploração inicial e pra informar codebook.
2. **Pipeline Macia (clustering):** parte dos códigos → agrupa casos → clusters discretos. Útil pra análise pós-codificação.

Além disso, a ideia de rodar AC sobre todo o corpus de referências deste projeto (os ~30 papers) seria uma meta-aplicação interessante — usar o método pra mapear a própria pesquisa bibliográfica.

---

## 3. Henry, D., Dymnicki, A., Mohatt, N., Allen, J., & Kelly, J. (2015). Clustering Methods with Qualitative Data: A Mixed Methods Approach for Prevention Research with Small Samples

**Fonte:** Prevention Science, 16(7), 1007-1016.
**Arquivo:** `./GTQQ/Clustering Methods with Qualitative Data - A Mixed Methods Approach for Prevention Research with Small Samples.pdf`

| | |
|---|---|
| **Autores** | David Henry, Allison B. Dymnicki, Nathaniel Mohatt, James Allen, James G. Kelly |
| **Instituições** | University of Illinois at Chicago; American Institutes for Research; University of Colorado; University of Minnesota |
| **País** | EUA |
| **Ano** | 2015 |
| **Journal** | Prevention Science |
| **Setor/Contexto** | Prevenção / Saúde comunitária — liderança comunitária em prevenção de abuso de substâncias, comunidade afro-americana em Chicago |
| **Tipo** | Validação metodológica (simulação) + aplicação real |

### Resumo
Paper com dois estudos: (1) simulação testando se clustering funciona com dados binários em amostras pequenas, e (2) aplicação real num estudo de liderança comunitária pra prevenção de abuso de substâncias em Chicago. Saído de University of Illinois at Chicago + American Institutes for Research + U. Colorado + U. Minnesota. Mais metodológico que a Macia — valida o approach e amplia o leque de métodos.

### Problema
Pesquisa qualitativa de prevenção trabalha com comunidades culturalmente distintas e amostras pequenas (20-77 pessoas). Produz dados ricos mas poucos casos. A sabedoria convencional dizia que clustering não funciona com dados binários (foi desenvolvido pra contínuos) e que LCA precisa de amostras grandes. Ninguém tinha testado sistematicamente isso com as amostras típicas de pesquisa qualitativa.

Dado relevante: uma revisão dos últimos 10 anos da *Prevention Science* encontrou **apenas 5 artigos** usando clustering — o método era subutilizado no campo.

### Contexto dos dados

**Estudo 1 (simulação):** 1000 datasets artificiais pra cada combinação de: 4 tamanhos de amostra (20, 50, 100, 500) × 3 números de clusters (2, 3, 4) × 4 probabilidades condicionais (.6, .7, .8, .9). Cada dataset com 4 variáveis binárias. Total: 48.000 simulações. Testaram 3 métodos.

**Estudo 2 (case real):** Developing Communities Project (DCP) em Greater Roseland, Chicago — organização comunitária ligada a igrejas, prevenção de abuso de substâncias. 77 líderes comunitários afro-americanos entrevistados (54.5% mulheres, 23% clérigos). Entrevistas semi-estruturadas de ~1.5h sobre apoio social, habilidades, comunicação inter-organizacional, visões pessoais.

### Método

**Estudo 1 — simulação:** Gerou dados binários com estrutura de cluster conhecida → rodou os 3 métodos → comparou acurácia usando V de Cramer (clusters encontrados vs. clusters reais conhecidos).

**Estudo 2 — aplicação real:**
1. **Codificação puramente indutiva** (grounded theory, Strauss & Corbin) — sem códigos a priori. Equipe gerou 56 códigos por consenso que se organizaram em 5 dimensões de liderança comunitária
2. **Binarização** — presença/ausência de cada código por participante (1/0)
3. **Análise descritiva pré-clustering** — média (proporção de 1s) e correlações phi entre códigos. Excluiu códigos com média muito baixa (pouco diferenciadores) e códigos muito correlacionados (redundantes)
4. **Estratégia combinada de clustering** — hierárquico primeiro pra decidir número de clusters (via dendrograma), depois K-Means pra atribuição final
5. **Interpretação colaborativa** — Executive Director + 2 membros do board + pesquisadores em múltiplas reuniões. Se não achavam interpretável, refaziam a análise

### Os 3 métodos comparados — diferenças práticas

| Método | Como funciona | Vantagem | Desvantagem | Amostra mínima |
|---|---|---|---|---|
| **Hierárquico (Ward)** | Funde casos mais parecidos passo a passo; produz dendrograma | Funciona com qualquer N; visual intuitivo | Erro no início propaga (sem correção); não tem teste de fit | ~20 |
| **K-Means** | Centros aleatórios; move casos entre clusters iterativamente | Pode corrigir atribuições; bom pra refinar | Precisa saber nº clusters antes; instável com N<50 | ~50 |
| **LCA (Latent Class Analysis)** | Modelo probabilístico com variável latente; dá probabilidades de pertença | Único com teste formal de fit; dá probabilidades | Precisa N>50 pra convergir; mais complexo | ~50 |

**Estratégia recomendada por situação:**
- **N < 50:** Só hierárquico (os outros falham)
- **N 50-100:** Hierárquico pra explorar + K-Means pra refinar (o que o Henry usou no Study 2)
- **N > 100:** LCA como principal + hierárquico como comparação

### Resultados

**Estudo 1 — simulação:**
- Os 3 métodos performaram similarmente — sem diferença significativa geral
- A acurácia **não diminui** com amostras de até 50 (contraria a crença de que precisa de N grande)
- Com N=20: só hierárquico produziu soluções usáveis
- Maior probabilidade condicional = maior acurácia (clusters mais distintos são mais fáceis)
- Mais clusters = menor acurácia
- **Validação da Macia:** confirma que clustering hierárquico com dados binários de codificação qualitativa é legítimo e preciso

**Estudo 2 — os 3 clusters de líderes comunitários:**
- **"Ganho pessoal"** — motivação: adquirir conhecimento, receber recursos, trocar informação
- **"Obrigação moral"** — motivação: dar de volta à comunidade, satisfação de ser líder
- **"Mudança sistêmica"** — motivação: criar mudança comunitária, investir na juventude, desenvolvimento econômico

A organização usou os resultados pra ajustar recrutamento e treinamento.

### Qualitização implícita no estudo

Esse paper tem uma camada de qualitização que a Macia não tinha: **interpretação colaborativa com stakeholders**. O Executive Director e board members participaram de múltiplas reuniões pra nomear e interpretar os clusters. Se não achavam interpretável, a análise era refeita. O critério de qualidade da qualitização não era estatístico (fit, p-valor) — era **interpretabilidade pelos stakeholders**. O teste de validade do quanti é quali.

Os nomes "Ganho pessoal", "Obrigação moral", "Mudança sistêmica" são produto dessa co-construção. Também usaram "five trees" — representação gráfica onde cada líder podia ver suas respostas comparadas com os valores modais do grupo. Qualitização visual + participativa.

Isso tangencia fortemente reuniões de síntese em pesquisa aplicada (UX research, design research, service design) — aquele momento onde pesquisador apresenta achados pra stakeholders e juntos constroem significado. A diferença: aqui os stakeholders interpretam **output estatístico** (gráficos de barras com médias por cluster), não post-its ou quotes.

### Relação com Macia (2015)

O Henry essencialmente **valida** o approach da Macia e vai além:
- Confirma que clustering hierárquico funciona com dados binários de codificação qualitativa
- Prova que funciona com amostras pequenas (até N=20 pro hierárquico)
- Testa e compara 3 métodos (Macia usou só hierárquico)
- Mostra que K-Means e LCA são alternativas viáveis com N>50
- Adiciona a dimensão colaborativa na interpretação

### Conexão com obsidian-qualia-coding
- O plugin deveria oferecer os 3 métodos, com recomendação baseada no N
- A estratégia combinada (hierárquico → K-Means) poderia ser um workflow guiado
- A interpretação colaborativa sugere que o output do clustering precisa ser **compartilhável** — exportável pra reunião de síntese com stakeholders

---

## 4. Boyatzis, R. E. (1998). Transforming Qualitative Information: Thematic Analysis and Code Development

**Fonte:** Sage Publications. 202 páginas.
**Arquivo:** `./GTQQ/Transforming Qualitative Information Thematic Analysis 1998.pdf`

| | |
|---|---|
| **Autor** | Richard E. Boyatzis |
| **Instituição** | Case Western Reserve University (psicologia organizacional) |
| **País** | EUA |
| **Ano** | 1998 |
| **Editora** | Sage Publications (Thousand Oaks, CA) |
| **Setor/Contexto** | Psicologia organizacional / Ciências sociais — competências gerenciais, comportamento organizacional |
| **Tipo** | Livro fundacional — análise temática como método de ponte quali↔quanti |

### Resumo
O livro que formalizou a análise temática como método autônomo (antes era tratada como "parte de" grounded theory, etnografia, etc.). Boyatzis posiciona análise temática como **tradutor** entre pesquisa qualitativa e quantitativa — a metáfora central é de duas pessoas que falam línguas diferentes e precisam de um tradutor pra se comunicar. É pragmatista declarado: "se você é qualifóbico ou quantifóbico, esse livro não é pra você. É pra quem quer expandir seu repertório."

**Crítica relevante — Kate Gerrish (Sheffield Hallam University, J. of Advanced Nursing, 1999):**
A reviewer aponta que Boyatzis carrega uma premissa não-dita: que análise temática é **O** missing link entre quali e quanti, e que traduzir achados qualitativos pro paradigma positivista é desejável. Ela argumenta que: (1) análise temática é "an important communication channel" mas "not the only or the ideal means of translation"; (2) o uso excessivo desse approach pode levar a "a diminution of the appreciation of the inherent value and richness of qualitative data"; (3) "the challenge to qualitative research must be how to interpret data without diluting its richness". Não diz que o método é errado — diz que **assumir que tradução é sempre desejável** é um pressuposto que deveria ser explicitado. É exatamente a tensão central do Foundations.md: quando a transformação é legítima? Quando dilui?

### Estrutura do livro
- **Cap 1:** "The Codable Moment" — como perceber temas (sensing), com analogia ao aprendizado de língua estrangeira
- **Cap 2:** Developing themes and codes — teoria vs. dados
- **Cap 3:** Unidades de análise e sampling — decisões que afetam tudo
- **Cap 4:** Codificação indutiva (data-driven) com Life Stories
- **Cap 5:** Codificação dedutiva (theory-driven / prior-research-driven) com Critical Incident Interview
- **Cap 6:** **Scoring, Scaling, and Clustering Themes** — o capítulo sobre transformação
- **Cap 7:** Reliability como consistência de julgamento
- **Cap 8:** Desafios pessoais e profissionais da análise temática

### O que Boyatzis chama de "análise temática"

Não é apenas codificação qualitativa — é mais amplo e mais específico:

**Mais amplo que codificação:** É "a process for encoding qualitative information" que inclui 5 passos: (1) perceber temas (sensing, o "codable moment"), (2) desenvolver os temas em códigos explícitos, (3) aplicar os códigos ao material, (4) interpretar padrões, e (5) comunicar resultados. A codificação é o passo 3 — a análise temática é o processo inteiro do 1 ao 5.

**Mais específico que "análise qualitativa":** Posicionada como método **transversal** que não pertence a nenhuma tradição — não é grounded theory (embora use codificação), não é etnografia (embora analise cultura), não é análise de conteúdo (embora conte ocorrências).

A metáfora central: é como aprender uma **língua estrangeira**. Cada método qualitativo é um idioma. A análise temática não é um idioma novo — é a habilidade de **traduzir entre idiomas**. "Thematic analysis is a translator. When people from different countries who speak different languages meet for the first time, a translator facilitates communication. Thematic analysis is a translator of those speaking the language of qualitative analysis and those speaking the language of quantitative analysis." (Prefácio, p.vii)

Pro Qualia Coding: o plugin implementa o passo 3 (codificação) e parte do 4 (interpretar padrões via analytics). Os passos 1-2 (perceber e desenvolver temas) e 5 (comunicar/qualitizar) ficam com o pesquisador.

### Cap 3 — Unidades de análise e unidades de codificação

Boyatzis distingue duas coisas que frequentemente se confundem:

- **Unidade de codificação** — o trecho onde se aplica o código (sentença, parágrafo, incidente, bloco de 5min)
- **Unidade de análise** — o nível onde se agrega pra comparar (pessoa, incidente, organização, grupo)

| Exemplo no livro | Unidade de codificação | Unidade de análise |
|---|---|---|
| Competências gerenciais (Cap 5) | Incidente crítico dentro da entrevista | O gerente (agrega incidentes) |
| Life Stories (Cap 4) | Sentença ou trecho temático | Life story inteira ou fase da vida |
| TAT (Cap 6) | História contada sobre uma imagem | O sujeito (agrega histórias) |

Essa decisão **muda a distribuição dos scores** e portanto quais análises são possíveis. Conecta diretamente com a tensão Macia (unidade=evento, N escalado, dependência) vs. Henry (unidade=pessoa, N real, independência) vs. Sicredi (unidade=insight, dependência do estudo). Boyatzis não diz qual é "certa" — diz que é decisão de pesquisa que precisa ser explicitada e justificada.

### Cap 6 — O coração do livro pra nosso projeto

Boyatzis apresenta um **continuum** de usos da análise temática: de descrição puramente qualitativa até análise estatística quantitativa. O capítulo é literalmente sobre **quantitização** — publicado no mesmo ano que Tashakkori & Teddlie (1998) cunharam o termo, mas Boyatzis não usa essa palavra. Chama de "scoring", "scaling" e "quantitative translation".

#### Os 5 tipos de scoring (Table 6.2)

| Tipo | O que faz | Exemplo | Nível de medida |
|---|---|---|---|
| **(a) Nominal** | Qual categoria se aplica | Código "gênero": masculino=1, feminino=2. O número é rótulo, não quantidade. | Nominal |
| **(b) Presença/ausência** | O tema aparece ou não (0/1) | "Essa entrevista demonstrou empatia?" → 0 ou 1. É a binarização que Macia e Henry usam. **Exemplo do livro (p.92):** Theme 4 "Sensitivity to Others" divide em 4a (no trabalho) e 4b (na família). Reconceptualização alternativa: transforma 4b em presença/ausência, calcula 4b−4a. Resultado: Managers 1-6 = -2, -1, -2, 0, +1, +1. Superiores (4,5,6) positivos ou neutros; típicos (1,2,3) negativos. O tema muda de "quanto falou" pra "a sensibilidade é mais voltada pra família do que pro trabalho?" | Nominal (mas pode virar ordinal — ver abaixo) |
| **(c) Frequência condicionada** | Conta ocorrências SÓ SE presença foi codificada | **Exemplo do livro (p.132):** TAT (Thematic Apperception Test) — pesquisador mostra imagem, codifica se a história tem "need for achievement imagery". SE sim, conta quantas das 10 subcategorias aparecem. Participante A: tem imagery? Sim → 4 de 10 subcategorias → score 4. Participante B: não tem → score 0 (nem conta). A soma parece intervalar (0-10) mas é ordinal — subcategorias não são equivalentes em peso conceitual. | Ordinal |
| **(d) Frequência livre** | Conta ocorrências sem condição prévia | **Exemplo do livro (p.132):** "empathy coding" — empatia codificada uma vez por incidente na entrevista. Se a entrevista tem 6 incidentes críticos, score pode ir de 0 a 6. Mas a distribuição é J-curve (muitos 0s e 1s, raríssimos 3+). Um discurso de 40 páginas com 520 sentenças pode ter até 200 menções de um tema — o tamanho do material infla a frequência. **Alerta:** "the length of the essay is a potential source of bias" — normalizar pelo nº de páginas/sentenças. | Ordinal a intervalar |
| **(e) Intensidade** | Grau de manifestação | **Exemplo do livro (p.133-134):** pesquisador codifica reuniões de departamento a cada 5 minutos. Tema: "orgulho/afeto positivo na organização". Cada bloco de 5min recebe score de intensidade. Resultado por reunião = quão forte o orgulho apareceu, não quantas vezes. Pode ser parte do próprio código (níveis: leve/moderado/forte). **Problema:** se material tem tamanhos diferentes (essays manuscritas vs. digitadas), a oportunidade de manifestação não é igual. | Intervalar (mas ver ressalvas) |

#### A J-curve — por que frequência ≠ importância (o guardrail)

Esse é o ponto mais importante pra ferramentas como o Qualia Coding. Boyatzis explica:

Imagina que você codificou 50 entrevistas sobre competências gerenciais. Uma das competências é "empatia". Pra cada entrevista, contou quantas vezes empatia apareceu. A distribuição típica vai ser assim:

```
Score 0: ||||||||||||||||||  (18 entrevistas — muitos zeros)
Score 1: ||||||||||||||||    (16 entrevistas — muitos uns)
Score 2: ||||||||           (8 entrevistas)
Score 3: ||||              (4 entrevistas)
Score 4: ||               (2 entrevistas)
Score 5: |                (1 entrevista)
Score 6: |                (1 entrevista — raríssimo)
```

Isso é a **J-curve invertida** (ou "sideways J tilted 90 degrees" como Boyatzis descreve). A maioria das pessoas mostra o tema 0 ou 1 vez. Poucas mostram 2. Raríssimas mostram 3+.

**Por que isso importa:**
1. **Score de frequência NÃO é intervalar** — a distância conceitual entre 0 (ausente) e 1 (presente) não é a mesma que entre 3 e 4. Mostrar empatia 4 vezes não é "uma empatia a mais" que 3. É ordinal.
2. **Média aritmética não faz sentido** — com uma J-curve, a média de empatia na amostra vai ser tipo 1.2, o que não representa ninguém (ninguém demonstrou "1.2 empatias").
3. **Transformações estatísticas são necessárias** — logarítmica, raiz quadrada — pra normalizar antes de rodar análises paramétricas. Mas Boyatzis alerta: "resulting in scores that do not make visual sense" — os números transformados perdem interpretabilidade.
4. **A frequência pode ser artefato do método, não do fenômeno** — se as entrevistas tinham durações diferentes, uma entrevista de 2h naturalmente terá mais menções que uma de 30min. Boyatzis recomenda: divida o score pelo tamanho do material (nº de páginas, nº de sentenças). Mas mesmo isso assume que oportunidade = manifestação.

**Implicação pro Qualia Coding:** Qualquer view de analytics que mostre frequência de códigos precisa de um guardrail: avisar que frequência bruta não é comparável entre documentos de tamanhos diferentes, e que a distribuição provavelmente é J-curve (não normal). Oferecer normalização por tamanho do documento como opção.

#### Presença/ausência é mais poderoso do que parece

Boyatzis faz um argumento sutil: quando um tema tem subtemas (ex: "need for achievement" tem 10 subcategorias), a presença/ausência de cada subcategoria é mais informativa que a contagem. O score final (soma de subcategorias presentes) parece intervalar (0-10) mas é ordinal — porque as subcategorias não são equivalentes em peso conceitual. Score 4 não é "uma subcategoria acima de 3" da mesma forma que 2 é "uma acima de 1".

Isso é exatamente o que Macia faz: binariza (presença/ausência) e clusteriza. Boyatzis está dizendo que essa é a forma mais robusta de quantitizar dados temáticos — não porque é a mais rica, mas porque é a que menos distorce.

#### Duas formas de formar clusters (Table 6.2)

| Tipo | Como | Vantagem | Limitação |
|---|---|---|---|
| **Conceptual** | Pesquisador agrupa temas por (a) características relacionadas, (b) constructo subjacente, ou (c) hierarquia causal | Fácil, intuitivo, conecta com teoria | Enviesado pela teoria do pesquisador; não reflete necessariamente os dados |
| **Empírico** | Análise estatística multivariada (cluster analysis, fatorial) agrupa temas que co-ocorrem | Revela padrões não visíveis; menos enviesado | Precisa de N suficiente; distribuições J-curve violam pressupostos |

O exemplo principal: competências gerenciais (Boyatzis, 1982, N=1000+). Table 6.1 mostra **conceptual vs. empirical clustering lado a lado**:

**Clusters conceituais** (organizados por teoria de competências):
- *Entrepreneurial:* Efficiency Orientation, Initiative
- *Interpersonal:* Concern With Impact, Developing Others, Use of Unilateral Power, Use of Socialized Power, Managing Group Process, Oral Presentations
- *Intellectual:* Diagnostic Use of Concepts, Logical Thought, Conceptualization
- *Socioemotional Maturity:* Stamina/Adaptability, Accurate Self-Assessment, Perceptual Objectivity, Spontaneity, Self-Control

**Clusters empíricos** (organizados por co-ocorrência nos dados):
- *Goal and Action Management:* Efficiency Orientation, Initiative (i.e. Proactivity), Diagnostic Use of Concepts, Concern With Impact
- *Directing Subordinates:* Developing Others, Use of Unilateral Power, Spontaneity
- *Human Resource Management:* Managing Group Process, Use of Socialized Power, Accurate Self-Assessment
- *Leadership:* Oral Presentations, Self-Confidence, Conceptualization, Logical Thought
- *Focus on Others:* Perceptual Objectivity (+ outros)

A reorganização empírica revelou padrões que o framework conceitual não capturava — "Developing Others" e "Use of Unilateral Power" estavam em clusters conceituais separados mas caíram juntos em "Directing Subordinates" no empírico. Faz sentido na prática gerencial: desenvolver pessoas E usar poder sobre elas co-ocorrem (é o mesmo gerente fazendo as duas coisas no mesmo contexto). O empírico captura o **comportamento real**, o conceitual captura a **teoria sobre competências**.

Boyatzis comenta (p.141): os clusters empíricos permitiram expandir a teoria apresentada no "The Competent Manager" (1982), porque revelaram que as competências se organizavam por **função gerencial** (dirigir, liderar, gerenciar RH) e não por **tipo de habilidade** (interpessoal, intelectual). A apresentação do modelo empírico "appeared to make sense to executives and human resource professionals" — qualitização colaborativa implícita: os stakeholders validaram os nomes dos clusters empíricos.

E quando Mentkowski et al. (1982) replicaram com **amostra exclusivamente feminina**, os clusters empíricos mudaram de novo — "accurate self-assessment" migrou para o cluster de goal and action management (nas mulheres, autoavaliação precisa co-ocorre com orientação a resultados; nos homens, com gestão de recursos humanos). "Positive regard" e "managing group process" se associaram com "developing others" — nas mulheres, o cuidado com o grupo é parte do desenvolvimento de pessoas. Os autores interpretaram que "the dynamics in the different empirical clusters reflected important and evident differences in the situations faced by female managers in the late 1970s and early 1980s."

Isso não apareceria no clustering conceitual — e é argumento fortíssimo pra que ferramentas de QDA ofereçam **ambos** lado a lado.

#### Scaling e o aviso sobre independência

Boyatzis alerta: "multiple regression or discriminant function analysis will be inappropriate if you do not believe or predict your themes to be mutually exclusive." Se os temas são conceitualmente relacionados (como "iniciativa" e "persuasão", ambos ligados a "need for achievement"), forçar independência estatística distorce os clusters.

Isso conecta diretamente com a discussão sobre violação de independência que fizemos com a Macia e o Sicredi — Boyatzis já avisava em 1998 que a dependência entre temas não é bug, é feature dos dados qualitativos.

### Outras seções relevantes

**Cap 3 — Unidades de análise:** Boyatzis trata da decisão que afeta tudo — o que é a "unidade de codificação" (parágrafo? sentença? incidente?) e como essa decisão muda as distribuições dos scores. Conecta com a discussão Macia (unidade=evento) vs. Henry (unidade=pessoa).

**Cap 7 — Reliability:** Boyatzis redefine confiabilidade como "consistência de julgamento" (não verificação positivista). Dois tipos: (a) entre codificadores e (b) ao longo do tempo/contextos. Posiciona reliability como o que permite a ponte: "thematic analysis with reliability as consistency of judgment provides for methodological translation and conceptual bridges between two or more approaches to discovery." É a análise temática + reliability que legitima a transformação.

### Qualitização implícita

O caso Mary Simpson (p.127) é qualitização pura sem o nome: scores de frequência em 13 competências transformados em narrativa — "she was coded for more management abilities than is typical for entering MBA students" (Perfil Normativo); "she was demonstrating analytic reasoning abilities more frequently than most" (Perfil Comparativo). O feedback pra Mary é qualitização aplicada em contexto de desenvolvimento profissional.

A Table 6.1 (conceitual vs. empírico) também é qualitização: os clusters empíricos recebem **nomes** ("Goal and Action Management", "Directing Subordinates") que são atos de interpretação qualitativa sobre output estatístico. E quando os clusters mudam com amostra feminina, os novos nomes são nova qualitização do mesmo método.

### Conexão com obsidian-qualia-coding

**Guardrails necessários no plugin:**
1. Avisar que frequência bruta de códigos segue J-curve — não é normal, não faz sentido calcular média
2. Oferecer normalização por tamanho do documento (nº de segmentos, nº de palavras)
3. Distinguir entre presença/ausência (mais robusto) e frequência (mais rico mas mais problemático)
4. Na view de clustering: mostrar claramente que é R-analysis (clusters de códigos) e não Q-analysis (clusters de casos)
5. O framework conceitual vs. empírico é exatamente o que o plugin já permite: o pesquisador cria famílias de códigos manualmente (conceitual) E o dendrograma sugere agrupamentos (empírico). Mostrar os dois lado a lado seria poderoso.

---

## 5. Jaworska, N. & Chupetlovska-Anastasova, A. (2009). A Review of Multidimensional Scaling (MDS) and its Utility in Various Psychological Domains [renumerada de #4]

**Fonte:** Tutorials in Quantitative Methods for Psychology, 5(1), 1-10.
**Arquivo:** `./GTQQ/MDS/A Review of Multidimensional Scaling (MDS) and its Utility in Various Psychological Domains p1-10.pdf`

| | |
|---|---|
| **Autoras** | Natalia Jaworska, Angelina Chupetlovska-Anastasova |
| **Instituição** | University of Ottawa, Institute of Mental Health Research |
| **País** | Canadá |
| **Ano** | 2009 |
| **Journal** | Tutorials in Quantitative Methods for Psychology |
| **Setor/Contexto** | Psicologia — review tutorial de MDS com aplicações em percepção, personalidade, aconselhamento, construção de testes |
| **Tipo** | Review tutorial (não é estudo empírico) |

### Resumo
Review não-técnico de Multidimensional Scaling voltado pra psicólogos. Apresenta o que é MDS, como funciona, tipos de dados, tipos de MDS, diagnósticos de output, e faz um tour por aplicações em psicologia (construção de testes, perfis de personalidade, percepção de odores/emoções/dor, psicologia de aconselhamento).

### Problema
Psicólogos têm dados complexos (percepções, similaridades, preferências) que frequentemente são não-lineares e multidimensionais. MDS oferece alternativa a métodos como análise fatorial — com menos pressupostos e output visual mais intuitivo. Mas o método é subutilizado porque a literatura técnica é inacessível pra quem não é estatístico.

### Contexto dos dados
Não é estudo empírico — é review. Os dados vêm dos studies citados:
- Distâncias entre cidades (exemplo didático)
- Julgamentos de similaridade de odores (Lawless, 1989)
- Percepção de faces emocionais (Izmailov & Sokolov, 1999)
- Dor térmica (Clark et al., 1986)
- Itens de questionário de ansiedade (Roth & Roychoudhury, 1991)
- 31 medidas ambientais × modelo RIASEC de Holland (Armstrong et al., 2008)
- Perfis cognitivos WISC-III (Kim et al., 2004)

### Método — como MDS funciona (pra leigo)

Imagina uma tabela de "quão parecido/diferente é o item A do item B" pra um monte de itens. MDS pega essas distâncias e cria um **mapa espacial** onde itens parecidos ficam perto e diferentes ficam longe. O exemplo clássico: dada apenas a tabela de distâncias entre 10 cidades, o MDS reconstrói o mapa geográfico — dimensão 1 emerge como norte-sul, dimensão 2 como leste-oeste. As dimensões **não são dadas pelo pesquisador** — emergem dos dados.

**Input pode ser:**
- **Direto (raw):** participantes ordenam, comparam ou fazem card sorting de itens — julgamentos subjetivos de similaridade
- **Indireto (derivado):** correlações, tabelas de contingência, matrizes de confusão, co-ocorrências

**Tipos de MDS:**
- **CMDS (Classical):** uma matriz, caso básico
- **RMDS (Replicated):** várias matrizes (vários participantes), testa estabilidade
- **WMDS/INDSCAL:** várias matrizes com pesos individuais, captura diferenças de percepção entre pessoas

**Diagnósticos:** Stress (Kruskal) mede fit — ≤0.1 excelente, ≥0.15 intolerável. R² indica variância explicada (≥0.60 aceitável). Scree plot pro número de dimensões (buscar "cotovelo"). Shepard diagram pra distorção.

### Resultados — o tour pelas aplicações

**Construção de testes:** Roth & Roychoudhury (1991) usaram MDS pra item analysis de questionário de ansiedade. MDS revelou clusters de itens confirmados por cluster analysis hierárquica. Revisão do questionário resultou em α = 0.88-0.91. Vantagem sobre fatorial: menos pressupostos sobre distribuição.

**Perfis de personalidade:** Ding (2006) — MDS representa perfis normativos e mostra como indivíduos desviam. Kim et al. (2004) — comparação direta MDS vs. cluster analysis: **MDS dá nível E padrão do perfil, cluster analysis só dá padrão**. Essa é uma vantagem concreta do MDS.

**Psicologia de aconselhamento:** Armstrong et al. (2008) — modelo RIASEC de Holland (6 tipos vocacionais) mapeado em MDS 3D com 31 medidas ambientais via property vector fitting.

**Percepção:** Odores (Lawless, 1989) — free-sorting → MDS → estrutura circumplexa com odores ambíguos no centro. Emoções (Izmailov & Sokolov, 1999) — faces esquemáticas → MDS → espaço esférico (tom emocional × intensidade × saturação). Dor (Clark et al., 1986) — MDS revelou 2 dimensões de dor térmica: intensidade × qualidade (detectable→warm→hot vs. no pain→noxious).

### Qualitização implícita no estudo

O paper reconhece explicitamente que a interpretação de MDS é "challenging and highly subjective" — ou seja, a qualitização é parte constitutiva do método, não um bônus opcional. Nomear dimensões é o ato central de MDS.

Exemplos de qualitização dimensional nos studies citados:
- Cidades: eixo 1 = "norte-sul", eixo 2 = "leste-oeste" (trivial, verificável)
- Dor: eixo 1 = "intensidade", eixo 2 = "qualidade" (interpretativo, validado por regressão com medidas externas)
- Odores: estrutura circumplexa nomeada por categorias olfativas (interpretativo, corroborado por cluster analysis)

Kim et al. (2004) fazem comparação explícita de qualitização entre métodos: **cluster analysis qualitiza por categorização** (esse perfil pertence ao grupo X), **MDS qualitiza por interpretação dimensional** (esse perfil está na posição Y no eixo intensidade × qualidade). São atos qualitativos diferentes sobre outputs quantitativos diferentes — e MDS preserva mais informação (nível + padrão vs. só padrão).

### Conexão com obsidian-qualia-coding

O plugin já implementa MDS (R-analysis: códigos como pontos no mapa, distância Jaccard). A mesma matriz que alimenta o dendrograma alimenta o MDS — são visualizações complementares do mesmo dado:
- Dendrograma → "quais códigos agrupam" (famílias)
- MDS → "quais dimensões latentes organizam os códigos" (eixos conceituais)

O paper sugere que MDS com **property vector fitting** (projetar variáveis externas no espaço MDS) seria uma extensão poderosa: mapear códigos no espaço E projetar metadados (fonte do dado, fase da pesquisa, tipo de participante) como vetores. Isso conectaria R-analysis com contexto.

---

## Discussões Transversais

### O pipeline completo: AC → codificação → clustering

Juntando Morin e Macia, emerge um pipeline integrado de análise. Cenário concreto:

1. **Setup:** Abro o Obsidian, vault dedicado à análise. Carrego 30 PDFs. Tenho códigos predefinidos da teoria (dedutivos) no meu codebook, mas ainda não codifiquei nada.

2. **AC (exploração pré-codificação):** Rodo Análise de Correspondência no corpus bruto. O método processa o texto dos 30 PDFs e me dá metakeys — temas emergentes. Examino o mapa, aceito algumas metakeys como **códigos complementares** ao meu codebook dedutivo. Agora tenho códigos teóricos + códigos sugeridos pelos dados.

3. **Codificação qualitativa:** Leio os PDFs e codifico usando o codebook expandido. Durante a leitura, novos códigos emergem indutivamente (bottom-up). O codebook cresce organicamente.

4. **Clustering (análise pós-codificação):** Com tudo codificado, transformo os dados em matriz binária (Macia). Rodo cluster analysis. Separo variáveis de agrupamento vs. interpretação. Os clusters revelam padrões que não eram visíveis na codificação manual.

5. **Retorno ao quali:** Uso os clusters como lente pra reler os dados originais. Interpreto. Descubro coisas como o contraste grupos 5 vs. 6 da Macia (mesmas queixas, respostas opostas — o vínculo é que definia).

**O papel de cada método no pipeline:**
- AC = **exploração** (descubro a paisagem temática, informo o codebook)
- Codificação = **análise** (aplico códigos, construo dados estruturados)
- Clustering = **síntese** (descubro padrões nos dados estruturados)
- Retorno ao quali = **interpretação** (explico os padrões com os dados originais)

### Preparação da tabela de contingência para a AC

A AC não roda diretamente em PDFs — precisa de uma **tabela de contingência léxica** como input. O processamento anterior à análise em si:

1. **Extração de texto:** Tirar o texto bruto dos PDFs (OCR se necessário).

2. **Tokenização:** Quebrar o texto em palavras/termos individuais.

3. **Limpeza:**
   - Remover stopwords (the, and, of, is... / de, que, em, o...)
   - Decidir sobre formas gráficas: manter singular e plural como palavras separadas? A Morin mantém (porque "o plural pode significar outra coisa que o singular" — ex: "method" vs. "methods" podem ter contextos distintos). Decisão do pesquisador.
   - Remover palavras que aparecem em menos de X% dos documentos (threshold). X é empírico — a Morin usou valores que eliminaram docs com menos de 10 palavras restantes.

4. **Construção da tabela:** Linhas = documentos, colunas = palavras que sobreviveram à limpeza. Célula = frequência (quantas vezes a palavra aparece naquele documento). No caso da Morin: SERJ ficou 140 docs × 464 palavras, JSE ficou 224 docs × 576 palavras.

5. **Randomização (opcional):** A ordem dos casos pode influenciar — recomenda-se randomizar as linhas.

**Para o Qualia Coding**, os passos 1-4 seriam automatizados pelo plugin. O pesquisador carrega os PDFs, o plugin extrai texto, limpa, e monta a tabela. O threshold de filtragem e a decisão sobre formas gráficas seriam parâmetros configuráveis na UI.

### Validação metodológica: o que já está provado

Henry et al. (2015) é o paper que **baseia a existência do método** de clustering com dados qualitativos binarizados. Antes dele, a prática existia (Macia fez, outros fizeram) mas sem prova formal de que funcionava com as condições típicas de pesquisa qualitativa. A simulação com 48.000 datasets prova:

**O que está validado:**
1. **Clustering hierárquico funciona com dados binários** — contraria a recomendação do próprio SPSS/IBM de que "não deve ser tentado com variáveis binárias". Funciona.
2. **Amostras pequenas não comprometem acurácia** — até N=50, os 3 métodos performam bem. Hierárquico funciona até N=20.
3. **Os 3 métodos (hierárquico, K-Means, LCA) produzem resultados equivalentes** com dados binários — não existe "o melhor", existem trade-offs (ver tabela no Henry).
4. **A binarização de códigos qualitativos é input válido** — o processo Macia (codificar → binarizar → clusterizar) tem base empírica.

**O que ainda não está validado / limitações:**
- A simulação usou só 4 variáveis binárias — estudos reais (como a Macia com 59) têm muito mais. O efeito de alta dimensionalidade não foi testado.
- Não testou medidas de similaridade alternativas (Dice, Jaccard) — só euclidiana e probabilística.
- Não testou a robustez da **interpretação** — só a acurácia da atribuição de casos a clusters.

**Por que isso importa pro argumento geral:** Quando alguém questionar "por que usar clustering em dados qualitativos?", o Henry é a referência de validação. O Macia é o how-to. O Morin é a alternativa exploratória. Os três juntos formam a base metodológica.

### R-analysis vs Q-analysis: o que se agrupa muda tudo

Uma distinção fundamental que emerge ao cruzar os papers com a implementação atual do obsidian-qualia-coding:

| | R-analysis | Q-analysis |
|---|---|---|
| **Agrupa** | Códigos/variáveis que co-ocorrem | Casos/pessoas com perfis parecidos |
| **Matriz** | Código × código (co-ocorrência) | Caso × código (presença/ausência) |
| **Pergunta** | "Quais códigos andam juntos?" | "Quais pessoas/casos se parecem?" |
| **Revela** | Estrutura temática do codebook — famílias, redundâncias, relações inesperadas | Subgrupos de participantes — tipologias, perfis, padrões de comportamento |
| **Qualitização** | Nomear clusters de códigos ("família afetiva", "família estratégica") | Nomear clusters de pessoas ("os resignados", "os confrontadores") |
| **N** | Número de códigos (geralmente 20-100) | Número de casos/participantes (geralmente 20-500) |
| **Quem faz** | Macia não faz. Morin parcialmente (palavras). **Qualia Coding implementa hoje.** | Macia (195 queixas). Henry (77 líderes). **Qualia Coding ainda não implementa.** |

**O Qualia Coding hoje faz R-analysis:** matriz código × código, distância Jaccard, hierárquico aglomerativo com average linkage, dendrograma com corte dinâmico + silhouette scoring. Descobre quais códigos aparecem juntos nos mesmos segmentos.

**Todos os papers que lemos fazem Q-analysis:** agrupar casos/pessoas, não códigos. Pra completar o pipeline, o plugin precisa da Q-analysis — transpor a lógica: em vez de código × código, fazer caso × código.

São **complementares**: R-analysis refina o codebook (antes/durante codificação), Q-analysis descobre subgrupos (depois da codificação).

### Unidade de análise: a decisão que escala o N

A Macia tinha 21 pessoas entrevistadas mas 195 casos de queixa. Ela **redefiniu a unidade de análise** de pessoa para evento — cada queixa é um caso independente. Uma mesma pessoa pode ter 9 queixas em clusters diferentes. O Henry manteve pessoa como unidade (77 líderes = 77 casos).

| | Macia (unidade = evento) | Henry (unidade = pessoa) |
|---|---|---|
| **N real** | 195 queixas de 21 pessoas | 77 pessoas |
| **Descobre** | Tipologia de **situações** | Tipologia de **pessoas** |
| **Independência** | Queixas da mesma pessoa não são independentes (violação potencial) | Cada pessoa é independente |
| **Riqueza** | Mais granular — mesma pessoa em clusters diferentes | Mais holístico — perfil integral da pessoa |
| **Escalabilidade** | Escala N com mais eventos por pessoa | Precisa de mais participantes |

A "violação de independência" da Macia é interessante quando vista pela lente de métodos mistos e transformação de dados: dentro do paradigma estritamente estatístico, é uma violação de pressupostos. Mas dentro da perspectiva de crossover mixed analysis (Onwuegbuzie), pode ser reinterpretada como uma decisão metodológica legítima — a pesquisadora escolheu tratar o **evento** como unidade porque sua pergunta era sobre tipos de queixa, não sobre tipos de pessoa. A "dependência" entre queixas da mesma pessoa é, na verdade, **dado contextual** que enriquece a análise quando o pesquisador volta ao qualitativo.

Essa tensão entre rigor estatístico e riqueza interpretativa ecoa o projeto de ACM em Repositórios de UX da Sicredi (`2025-01-15-sicredi` no vault), onde Marlon aplicou Análise de Correspondência Múltipla em R sobre um **repositório de insights** — uma planilha onde cada linha era um achado/insight vindo de estudos anteriores (testes de conceito, usabilidade, pesquisas diversas sobre diferentes produtos). Cada registro tinha classificações como dores, oportunidades, insights, e metadados do estudo de origem.

A redefinição de unidade de análise aqui é **mais radical que a Macia**: na Macia, a unidade era o evento (queixa) com dependência da pessoa entrevistada. No Sicredi, a unidade era o **insight** com dependência do **estudo de origem** — um teste de usabilidade do produto X gerava 7 linhas na planilha, cada uma um achado. Então a dependência não era pessoa→eventos, era estudo→insights. Múltiplas camadas de não-independência: insights do mesmo estudo, estudos do mesmo produto, produtos da mesma empresa.

Mesmo assim, a ACM funcionou: os insights se organizaram em territórios de experiência ("Relacionamento Humanizado", "Autoserviço Fluido", "Eficiência Operacional") que depois foram qualitizados como princípios de design. O pipeline completo: múltiplos estudos quali → repositório de insights → quantitização via ACM em R → qualitização como territórios e princípios. Mixed methods aplicado em UX research com o mesmo ciclo infinito que o Foundations.md descreve — e com uma violação de independência ainda mais severa que a da Macia, mas pragmaticamente produtiva.

A inquietação sobre a validade desse trabalho no Sicredi — "será que o que fiz é legítimo metodologicamente?" — foi parte da motivação que originou toda a pesquisa do Foundations.md. Pesquisando sobre validade de ACM aplicada a dados qualitativos reaproveitados, surgiram os conceitos de quantitização, qualitização, crossover analysis, e o corpo teórico que hoje sustenta o projeto. É uma genealogia intelectual relevante: a prática veio antes da teoria, e a dúvida sobre a prática gerou a busca teórica.

Quanto ao impacto real da violação de independência no Sicredi: é uma pergunta aberta e honesta. Os territórios que emergiram da ACM poderiam estar inflados por estudos que contribuíram com muitas linhas, criando peso desproporcional de certos produtos ou contextos. Uma análise futura poderia testar a robustez: rodar a ACM com amostragem de 1 insight por estudo e comparar se os territórios se mantêm. Se sim, a dependência não distorceu; se não, os territórios refletiam a composição do repositório, não a estrutura real da experiência. Essa verificação de robustez é, em si, um exercício de validação que o Henry não fez (ele validou acurácia de atribuição, não robustez de interpretação).

### R-analysis no Qualia Coding: mais do que parece

Com a leitura dos papers fica claro que o obsidian-qualia-coding opera inteiramente em **R-analysis** (análise de relações entre códigos) — tanto no dendrograma (clustering hierárquico) quanto no MDS (mapa espacial). Ambos partem da mesma matriz código × código com distância Jaccard.

A diferença entre as duas visualizações do mesmo dado:

| | Dendrograma | MDS |
|---|---|---|
| **Mostra** | Quais códigos agrupam juntos (hierarquia) | Como códigos se posicionam num espaço (dimensões) |
| **Responde** | "MEDO e EVITAÇÃO andam juntos" | "MEDO e EVITAÇÃO andam juntos **e estão na dimensão emocional-passiva**" |
| **Revela** | Famílias de códigos | Dimensões latentes do codebook |
| **Qualitização** | Nomear clusters ("família afetiva") | Nomear dimensões ("passividade ↔ agência") |

O MDS responde uma pergunta que o dendrograma não responde: **quais são os eixos conceituais que organizam seus códigos?** Revela o "esqueleto" do framework analítico que talvez o pesquisador ainda não tenha percebido.

O que o plugin **ainda não faz** e que todos os papers que lemos fazem: **Q-analysis** — agrupar casos/documentos/participantes por perfil de códigos. Pra completar o pipeline Macia/Henry, precisa transpor: em vez de código × código, fazer caso × código. Isso abriria segmentação de participantes, tipologias, perfis comparativos — tudo que os papers demonstram.

### Qualitização: a prática sem nome

Uma linha transversal que emerge da leitura dos papers é que **qualitização é praticada amplamente sem ser nomeada como tal**. A Macia nomeia clusters. A Morin nomeia metakeys. Pesquisadores de mercado criam personas a partir de segmentação estatística. UX researchers constroem journey maps a partir de dados de analytics. Data scientists fazem "storytelling with data". Todos estão qualitizando — transformando output numérico em narrativa interpretativa — mas quase ninguém usa o termo.

Isso sugere que a discussão sobre qualitização na literatura de métodos mistos é escassa **não por falta de prática, mas por falta de denominação**. O campo acadêmico de métodos mistos (Sandelowski, Onwuegbuzie, Tashakkori, Teddlie) deu nome a algo que muitas disciplinas aplicadas fazem intuitivamente há décadas:

- **Pesquisa de mercado:** Nomear clusters de consumidores, criar perfis de segmento
- **Epidemiologia:** Interpretar curvas estatísticas como narrativas de surto
- **UX Research:** Transformar dados de usabilidade em personas e journey maps
- **Data journalism:** "Storytelling with data" — toda matéria jornalística baseada em dados é qualitização
- **Business intelligence:** Dashboards com KPIs que viram "a saúde do negócio"

A contribuição específica da literatura de métodos mistos não é inventar a prática, mas **sistematizá-la e dar-lhe rigor epistemológico**: quando a qualitização é legítima? Que critérios de qualidade se aplicam? Como evitar distorção na tradução? Como manter a tensão produtiva entre o número e a narrativa?

A cada paper que lermos, vale perguntar: **onde está a qualitização?** Mesmo que o autor não use o termo. E especialmente: **como ele qualitiza?** — nomeia categorias (como Macia), interpreta paisagens (como Morin), cria perfis verbais, constrói narrativas causais? Mapear essas variações ajuda a construir uma tipologia empírica da qualitização.

### DIME e o espelho da qualitização: a lacuna taxonômica

O modelo DIME (Onwuegbuzie, 2025) classifica **quantitização** por propósito analítico em 4 níveis: Descritiva, Inferencial, Medição, Exploratória. No Foundations.md (seção 3.3) já existe um espectro espelhado esboçado pra qualitização (Descritiva, Interpretativa, Narrativa, Teórica). Mas quando colocamos lado a lado e tentamos mapear os papers que estamos lendo, aparecem lacunas reveladoras:

| DIME — Quantitização | Espelho — Qualitização | Na tipologia de Tashakkori (1998) | Nos papers que lemos |
|---|---|---|---|
| **Descritiva** — frequências, médias, dispersão | **Descritiva** — descrições verbais de estatísticas | Perfil Modal, Perfil Médio | *(onipresente, invisível — todo paper faz)* |
| **Inferencial** — teste de hipóteses, GLM, SEM | **???** — traduzir p-valor e IC em "há evidência forte de que..." | *(sem nome)* | Macia: χ² = 211.551, p = .000 → "clusters capturam diferenças reais" |
| **Medição** — Rasch, IRT, escalas | **???** — traduzir score calibrado em "levemente deprimido" | Perfil Normativo (parcialmente) | *(não apareceu ainda)* |
| **Exploratória** — cluster, AC, MDS, fatorial | **Interpretativa** — nomeação de fatores e constructos | Perfil Comparativo (parcialmente) | Macia: nomear clusters (solo). Morin: nomear metakeys (com experts). Henry: co-construir nomes com stakeholders |

**O que a tabela revela:**

1. **Qualitização descritiva** é tão onipresente que é invisível — toda seção "descrição da amostra" de todo paper é qualitização descritiva. Ninguém reconhece como tal.

2. **Qualitização inferencial** não tem nome. Mas todo pesquisador que escreve "os resultados sugerem que..." a partir de um teste estatístico está qualitizando. É a prática mais comum da ciência e não está em nenhuma tipologia.

3. **Qualitização de medição** está parcialmente coberta pelo Perfil Normativo de Tashakkori, mas especificamente vinculada a instrumentos calibrados (escalas, inventários). É o que acontece em todo laudo psicológico ("score 27 no BDI = depressão moderada").

4. **Qualitização exploratória** é onde os papers que lemos operam — mas a tipologia de Tashakkori não distingue entre nomear clusters (Macia) e nomear eixos fatoriais (Morin). São atos qualitativos sobre outputs estatísticos diferentes, com lógicas diferentes:
   - **Nomear cluster** = dar identidade a um grupo discreto (ato de categorização)
   - **Nomear eixo/metakey** = dar identidade a uma dimensão contínua (ato de interpretação espacial)
   - **Construir perfil narrativo** = traduzir tabela de características em retrato verbal (ato de storytelling)

**A hipótese de trabalho:** A qualitização é prática antiga e disseminada em pesquisa aplicada (pesquisa de mercado, epidemiologia, UX, business intelligence) mas sub-denominada na literatura acadêmica. A contribuição dos métodos mistos (Sandelowski, Onwuegbuzie, Tashakkori) foi dar nome e sistematizar. Mas a sistematização ainda está fragmentada — o DIME fez isso bem pra quantitização, e o equivalente pra qualitização ainda não existe com o mesmo rigor.

A cada paper que lermos, mapeamos: **que tipo de qualitização está sendo feita, mesmo que o autor não a nomeie?**

### Nota: modelo de 3 camadas (GPT, início da pesquisa)

No início do projeto (mai/2025), uma conversa no ChatGPT produziu um modelo em 3 camadas que captura o fluxo temporal do pipeline de transformação de dados:

1. **Camada 1 — Preparação técnica e epistemológica:** Transformações técnicas na quantitativização + epistemologia da representação qualitativa. O "antes" — como preparar dados quali pra virarem quanti e o que essa transformação significa.

2. **Camada 2 — Operação da quantitização:** Funções exploratórias da quantitização + preservação da complexidade. O "durante" — a quantitização como ferramenta exploratória (DIME nível 4), com a tensão de não achatar o fenômeno.

3. **Camada 3 — Interpretação e reancoragem no qualitativo:** Complementaridade entre análise e interpretação + estilos de enfrentamento e orientação à ação. O "depois" — é aqui que mora a qualitização implícita: voltar pros dados qualitativos usando output quantitativo como lente.

**Arquivo:** `./GTQQ/Output from ChatGPT.png`

Esse modelo captura algo que nenhuma tipologia individual (Tashakkori, DIME) captura: a dimensão temporal do processo. As tipologias classificam tipos ou propósitos (estático); esse modelo classifica **momentos no pipeline** (dinâmico). A camada 3 é o espaço da qualitização sem que o nome apareça.

Histórico das conversas GPT que geraram esse modelo a ser resgatado para reconstrução da timeline intelectual do projeto.

### Quem qualitiza: a dimensão ausente nas tipologias

As tipologias existentes (Tashakkori, DIME espelhado) classificam **o quê** se qualitiza e **como**. Mas uma dimensão que emerge dos papers é **quem** qualitiza — e isso muda radicalmente o processo e o resultado:

| Modo | Quem | Como funciona | Exemplo |
|---|---|---|---|
| **Qualitização pelo pesquisador** | Expert solo | Pesquisador interpreta output, nomeia clusters/eixos | Macia: 7 nomes de cluster criados pela pesquisadora |
| **Qualitização colaborativa** | Pesquisador + stakeholders | Co-construção em reuniões; critério = interpretabilidade | Henry: Executive Director + board + pesquisadores nomeiam juntos; refazem se não faz sentido |
| **Qualitização participativa** | Os próprios participantes | Participantes reagem a dados sobre si mesmos | Saldaña In Vivo: participantes geram "ON-TARGET", "I AGREE" |

A qualitização colaborativa do Henry tangencia fortemente **reuniões de síntese** em pesquisa aplicada (UX research, design research, service design) — aquele momento onde pesquisador apresenta achados e stakeholders co-constroem significado. A diferença: no Henry, os stakeholders interpretam output estatístico (gráficos de barras), não post-its ou quotes. Mas o processo social é o mesmo.

Isso sugere que qualitização colaborativa é praticada em muitos campos sem esse nome — toda reunião de síntese onde alguém apresenta dados e o grupo constrói interpretação é um ato de qualitização coletiva. É mais uma evidência da hipótese central: **qualitização é prática disseminada, sub-denominada**.

A implicação pra tipologia: além do tipo de perfil (Tashakkori) e do propósito analítico (DIME espelhado), precisamos de uma dimensão de **agência** — quem faz a qualitização e com que grau de participação.

### AC vs. Clustering — a diferença fundamental

Clustering (Macia) te dá **grupos fechados**: "esses 25 casos são o grupo 5". Cada caso pertence a um e só um grupo. É mais operacional — você age sobre os grupos.

AC (Morin) te dá um **campo de forças**: "esse paper está sendo puxado 60% pro tema X e 40% pro tema Y". Documentos não pertencem a um tema — estão posicionados num espaço contínuo. É mais exploratório — você entende a paisagem antes de agir.

A consequência pra ferramentas: clustering gera listas discretas (esses casos → esse grupo). AC gera visualização espacial (mapa interativo). São UIs fundamentalmente diferentes.

---

## 6. Driscoll, D. L., Appiah-Yeboah, A., Salib, P., & Rupert, D. J. (2007). Merging Qualitative and Quantitative Data in Mixed Methods Research: How To and Why Not

**Fonte:** Ecological and Environmental Anthropology, 3(1), 19-28.
**Arquivo:** `./GTQQ/Merging Qualitative and Quantitative Data in Mixed Methods Research - How to and Why not.pdf`

| | |
|---|---|
| **Autores** | David L. Driscoll, Afua Appiah-Yeboah, Philip Salib, Douglas J. Rupert |
| **Instituição** | RTI International (Research Triangle Institute) |
| **País** | EUA |
| **Ano** | 2007 |
| **Journal** | Ecological and Environmental Anthropology (University of Georgia) |
| **Setor/Contexto** | Saúde pública / Antropologia ambiental — avaliação de política federal de segurança de vacinas |
| **Tipo** | How-to operacional com case study aplicado |

### Resumo
Paper prático de RTI International mostrando como de fato fazer o merge de dados quali e quanti. Dois designs de coleta (concurrent e sequential), 5 passos concretos do merge com screenshots de ferramentas (NVivo, Access, SAS), e discussão honesta de vantagens e desvantagens. Case study: avaliação federal de guidelines de segurança de vacinas com stakeholders de várias agências.

### Problema
Apesar de Sandelowski (2000), Tashakkori & Teddlie (1998) e outros terem explorado a teoria da integração quali-quanti, "there remains a need for systematic information on how to actually carry out such transformative analytic designs." Faltava o how-to operacional.

### Contexto dos dados
Avaliação de política federal de segurança de vacinas (detalhes limitados por contrato). Stakeholders: especialistas em vacinas, funcionários de agências federais, grupos de advocacy. Dois estudos separados com designs diferentes.

### Os 2 designs de coleta

**Concurrent (Figure 1):** Survey web com perguntas fechadas (Likert) + campo aberto vinculado ("What additional information would you like to provide?"). Mesma pessoa, mesmo momento. Open-ended → NVivo → binarização → merge no Access por ID do respondente → SAS.

**Sequential (Figure 2):** Primeiro survey (fechado), depois entrevistas em profundidade com participantes selecionados. Entrevista customizada com base nas respostas do survey. Entrevista → NVivo → binarização → merge por ID → SAS.

### Os 5 passos do merge

1. Survey data → Access database
2. Qualitative data → NVivo → códigos → Access database (Figure 4: checkboxes 0/1 por código)
3. Link por ID do respondente (cada registro = survey + entrevista da mesma pessoa)
4. Binarização: códigos viram 0/1 — scoring tipo (b) do Boyatzis
5. Análise estatística no SAS (chi-quadrado, frequências, associações)

### Resultados — o achado que justifica o merge

Figure 5: 90% concordaram que "Vaccine Safety Review Process is Scientifically Rigorous and Objective." Mas apenas 45% concordaram que "Recent Vaccine Safety Decisions Are Accurate" — e 30% discordaram ativamente. **Contradição que só aparece com o merge.** A análise qualitativa das respostas abertas explicou: discordavam de guidelines específicas (base científica insuficiente em certos tópicos), não do processo em geral. Sem merge, o survey diria "90% aprovam" e esconderia a divergência.

### As desvantagens (honestas)

**1. Perda de profundidade e flexibilidade:** "Reducing rich qualitative data to dichotomous variables renders them single dimensional and immutable." Códigos qualitativos são multidimensionais; binarizar achata. Códigos podem ser revisitados e refinados durante análise qualitativa; dados binarizados são fixos. Se o codebook muda depois do merge, refaz tudo. É a preocupação da Gerrish operacionalizada.

**2. Colinearidade:** Códigos derivados da mesma questão aberta tendem a ser correlacionados — "response categories are themselves linked as a consequence of the coding strategy." Se uma resposta gera 3 códigos, esses códigos não são independentes. Limita análises paramétricas. Solução deles: usar chi-quadrado (mais tolerante) e só cruzar códigos de fontes diferentes.

**3. Tamanho amostral:** Coleta quali é cara e lenta. O N do quali limita o merge. Pode faltar power estatístico.

**4. Imutabilidade:** Uma vez binarizado, o código é fixo. Diferente do quali, onde se pode voltar, reinterpretar, recodificar.

### Qualitização implícita

A explicação da contradição Figure 5 é qualitização: dados numéricos (90% aprovam processo, 30% discordam das decisões) transformados em narrativa interpretativa ("discordam de guidelines específicas por base científica insuficiente"). O número levantou a questão; a volta ao quali respondeu.

O design sequential inteiro é ciclo: quanti (survey) → quali (entrevista guiada pelos resultados) → quanti (merge + análise) → quali (interpretação da contradição). Ciclo infinito em ação.

### Conexão com obsidian-qualia-coding

A contribuição específica do Driscoll é nomear **colinearidade entre códigos** como problema prático do merge — nenhum outro paper lido trata disso explicitamente. No Qualia Coding, onde múltiplos códigos podem ser aplicados ao mesmo segmento, a colinearidade é estrutural. Ver discussão transversal "Colinearidade" para impactos e guardrails.

---

## 7. Nzabonimpa, J. P. (2018). Quantitizing and qualitizing (im-)possibilities in mixed methods research

**Fonte:** Methodological Innovations, May-August 2018, 1-16.
**Arquivo:** `./GTQQ/References/Quantitizing and qualitizing (im-)possibilities in mixed methods research.pdf`

| | |
|---|---|
| **Autor** | Jean Providence Nzabonimpa |
| **Instituições** | The African Capacity Building Foundation (Harare, Zimbabwe); Stellenbosch University (África do Sul) |
| **País** | Zimbabwe / África do Sul |
| **Ano** | 2018 |
| **Journal** | Methodological Innovations (SAGE) |
| **Setor/Contexto** | Educação / Sociologia — escolha de disciplinas científicas por gênero em escolas secundárias de Ruanda |
| **Tipo** | Artigo empírico-metodológico (PhD research) — único a fazer quantitização E qualitização no mesmo estudo |

### Resumo
Paper ambicioso de PhD (Stellenbosch) que investiga possibilidades e impossibilidades de quantitização e qualitização num design convergente paralelo de duas fases. Estudo sobre fatores de gênero na escolha de disciplinas científicas em 3 escolas secundárias de Ruanda (N=360 Fase 1, N=90 Fase 2). Traz três contribuições que nenhum outro paper lido oferece: (1) a taxonomia "the said / the semi-said / the unsaid," (2) a demonstração empírica da assimetria quantitização > qualitização, (3) a delimitação de "un-quantitizable" e "un-qualitizable" como limites estruturais do ciclo.

### Problema
"While attempts have been made to achieve quantitizing and qualitizing of data, few empirical studies have been conducted in a two-phase convergent parallel mixed methods design to investigate such data conversion approaches, especially dichotomization, within a single inquiry." A maioria dos estudos faz um OU outro; ninguém fazia os dois no mesmo estudo pra comparar.

### Contexto dos dados
Três escolas secundárias típicas de Ruanda (boys-only, girls-only, mixed-sex), selecionadas por purposive sampling pra garantir representação de gênero. Phase 1: N=360 (120 por escola), survey + entrevistas semi-estruturadas + essays narrativos biográficos, concurrent. Phase 2 (3 meses depois): N=90 (metade da Phase 1, grupo experimental), mesmos respondentes mas **instrumentos trocados** — quem fez survey faz entrevista e vice-versa. Permite comparar: mesma pessoa, mesmo tema, dois métodos diferentes.

### O design — convergent parallel com crossover temporal (Figure 1)

Phase 1 e Phase 2 rodam em paralelo com strands quanti e quali. Na Phase 2, respondentes são **switched** entre instrumentos — o que permite testar se respostas qualitativas e quantitativas convergem quando a mesma pessoa usa ferramentas diferentes. McNemar test compara entre fases. Achado: "qualitative responses did not significantly differ across phases" — robustez do dado qualitativo mesmo com troca de instrumento.

### Quantitização no estudo

Codificação no Atlas.ti → binarização (presença/ausência por código por respondente) → export pra Excel (Figure 2: matriz respondent × code, 0/1) → merge com survey data no SPSS → chi-quadrado, regressão logística.

Decisão crucial: **coding for existence > coding for frequency**. Reteve sistematicamente 1 ocorrência por código por participante, independente de quantas vezes apareceu. Justificativa: "repetitive respondents' views would prevail over those of respondents who are concise and to the point." Quem fala muito dominaria. Presença/ausência equaliza — confirma scoring tipo (b) do Boyatzis como mais robusto.

### Qualitização no estudo

Dados quantitativos (Likert) submetidos a **análise fatorial** (PCA). Fatores extraídos com Cronbach's α ≥ .70 recebem **nomes qualitativos** (Table 4):

| Itens que carregam juntos | α | Nome qualitizado |
|---|---|---|
| Razões de escolha de matéria: reputação, política, infraestrutura, parentes | .74 | "Structural factors underlying choice of school subjects" |
| Razões: sou bom nisso, melhores resultados, gosto, oportunidades, dinheiro, metas | .75 | "Personal factors motivating the choice of school subject combination" |
| Atitudes sobre papel da mulher na sociedade (7 itens) | .73 | "Positive attitudes towards the role of women in society" |
| Atitudes sobre equidade de gênero (5 itens) | .72 | "Gender equity or gender equitable practices and attitudes" |

O ato de nomear o fator é qualitização explícita — "finding or imposing an underlying conceptual representation of the items." Hathcoat & Meixner (2015) são citados: "the researcher makes subjective decisions to derive a final solution, actually using the researcher as a subjective instrument to identify the latent variable." O pesquisador **é** o instrumento da qualitização. É arte, não ciência.

#### Por que Likert qualitiza bem e categórico não

Likert tem **gradação contínua** implícita — "strongly agree → agree → neither → disagree → strongly disagree" é um continuum. Quando qualitiza, traduz de volta pra linguagem natural facilmente: score 4.2 vira "atitudes moderadamente progressistas." O número carrega direção (positivo/negativo) e intensidade (forte/moderada/fraca). Tem narrativa embutida.

Dados categóricos/nominais não têm gradação. Tipo de escola (boys-only=1, girls-only=2, mixed=3): score médio 2.1 não significa nada — não é "ligeiramente girls-only." O número é rótulo, não quantidade. Não tem narrativa pra reconstruir.

Qualitização via factor analysis funciona porque os **fatores são dimensões latentes contínuas** extraídas de itens com gradação — o fator herda a propriedade contínua dos itens, e a nomeação reconstrói significado narrativo. Dados nominais binarizados (0/1) limitam a qualitização à nomeação de grupos (como Macia, Henry), não à interpretação dimensional.

### The said, the semi-said, and the unsaid

Taxonomia original (p.13-14) sobre camadas de dados qualitativos:

| Camada | O que é | Quantitizável? | Exemplo |
|---|---|---|---|
| **The said** | O que o respondente declarou explicitamente | Sim — binarizável, contável | "I chose science because of job opportunities" |
| **The semi-said** | O implícito, o não-verbal, o que se lê nas entrelinhas | Parcialmente — qualitativamente analisável mas difícil de binarizar | Tom de revolta ao falar sobre patriarcado; hesitação antes de responder |
| **The unsaid** | O que o respondente não disse — silêncio, omissão | Não — "unspeakable and unanalyzable" (MacLure et al., 2010) | Nunca mencionou casamento/filhos como fator (mas no survey marcou como importante) |

No survey: silêncio = campo vazio = dado faltante. Na entrevista face-a-face: silêncio com linguagem corporal = **dado** — semi-said que dá glimpse do unsaid. Os dois métodos capturam camadas diferentes.

### Un-quantitizable e un-qualitizable — os limites estruturais

**Un-quantitizable:** Dados faltantes, informação implícita, tom/hesitação, respostas não-linguísticas. "Language tones and sense of revolt are not easily quantitizable, unless the process is confined to counting participants whose tone and revolt are raised against the patriarchal order." O semi-said resiste à binarização.

**Un-qualitizable:** "The closed-ended and numerically answered questionnaire does not offer much that can be taken back into narratives, unless in the form of data interpretation." Likert puro sem campo aberto é difícil de qualitizar — o número seco não tem narrativa pra voltar. A não ser via factor analysis + nomeação (que exige escalas com α ≥ .70).

### A assimetria quantitização vs. qualitização — refinamento do ciclo infinito

Nzabonimpa é explícito na conclusão: "quantitizing is more used and documented than qualitizing... qualitizing is the least practised in data conversion and may still lag behind." E: "most qualitative and quantitative software promote quantitizing to the detriment of qualitizing."

**Relação com Sandelowski et al. (2009) — refinamento, não contradição:**

O ciclo infinito da Sandelowski é uma **proposição epistemológica**: quantitização e qualitização se implicam mutuamente, são inseparáveis conceitualmente. Todo ato de quantitizar já envolve qualitização (decidir o que conta como "presença" é julgamento qualitativo) e vice-versa (nomear um fator latente parte de output numérico). Isso continua verdade — Nzabonimpa não invalida o ciclo.

O que Nzabonimpa mostra opera em dois outros níveis:

**1. A prática metodológica é assimétrica** (não o ciclo em si):

| | Quantitização | Qualitização |
|---|---|---|
| **Software** | Suporta (NVivo, Atlas.ti, MAXQDA exportam frequências, matrizes) | Não suporta (como um software ajuda a "nomear um fator latente"?) |
| **Comunidade** | Pratica amplamente | Pratica pouco, documenta menos |
| **Caminho** | Pavimentado (codificar → binarizar → analisar) | Improvável (fator → nome? Como?) |
| **Ato** | Operação computacional (binarizar é algoritmo) | Ato interpretativo do pesquisador (nomear é arte) |

A falta de software pra qualitização **confirma** o argumento da Sandelowski, na verdade: se qualitização é prática disseminada mas sub-denominada (nosso argumento sobre "a prática sem nome"), faz sentido que software não suporte algo que a comunidade nem reconhece como ato formal. O software reflete o estado da consciência metodológica, não os limites do possível.

**2. Existem limites estruturais — dados que não entram no ciclo:**

| Limite | O que é | Por que não entra |
|---|---|---|
| **Un-quantitizable** | The semi-said e unsaid (tom, hesitação, silêncio corporal) | Resistem à binarização — são quali sem volta pro quanti |
| **Un-qualitizable** | Likert fechado sem campo aberto, categóricos nominais | O número seco não tem narrativa pra reconstruir — são quanti sem volta pro quali |

Dentro do que entra no ciclo (o **said**, os dados com gradação), o ciclo opera como Sandelowski descreve. Mas nem todo dado entra. O semi-said e o unsaid ficam fora.

**Síntese — três níveis distintos:**
1. **Ciclo epistemológico** (Sandelowski): simétrico, sempre presente, proposição sobre a natureza dos dados — **válido**
2. **Prática metodológica** (Nzabonimpa): assimétrica — mais gente quantitiza, mais software suporta — **evidência empírica que não invalida o ciclo mas revela gap de infraestrutura**
3. **Limites estruturais** (Nzabonimpa): existem dados que não completam a volta — **refinamento real do ciclo, delimitando seu escopo**

**Implicação pro Foundations.md:** O ciclo infinito pode ser reapresentado com mais nuance — válido epistemologicamente, assimétrico na prática, com pontos cegos estruturais. Não é "espiral com perdas" (que sugere degradação) — é **ciclo com escopo delimitado e infraestrutura desigual**.

### Qualitização implícita e explícita

Esse é o primeiro paper que trata qualitização **explicitamente** como tema — Table 4 é dedicada a mostrar como fatores foram nomeados, seção "Qualitized results" é heading próprio. Mas também mostra os limites: "qualitizing works optimally with scaled items, indicating much more likelihood of qualitizing than quantitizing impossibilities."

### Referência a investigar

**Hathcoat, J. D. & Meixner, C. (2015)** — citado por Nzabonimpa pra "the researcher as subjective instrument to identify the latent variable." Provavelmente trata a subjetividade da interpretação fatorial como feature, não bug. Aprofundaria o ato de nomeação como qualitização. Baixar e ler.

### Conexão com obsidian-qualia-coding

1. **Coding for existence > frequency** — confirma que presença/ausência é mais robusto. O plugin deveria ter modo "existence" (1 por código por documento) além de frequência
2. **A assimetria** — o plugin facilita quantitização (analytics, frequências, co-ocorrência) mas não facilita qualitização. Feature futura: sugerir nomes de clusters/fatores? Gerar perfis narrativos automaticamente?
3. **The semi-said** — o plugin captura anotações de segmentos (o said), mas não captura tom, hesitação, contexto não-verbal. Limitação estrutural de qualquer ferramenta baseada em texto

---

## 8. Tashakkori, A. & Teddlie, C. (1998). Mixed Methodology: Combining Qualitative and Quantitative Approaches (Cap 6)

**Fonte:** Sage Publications (Applied Social Research Methods Series, vol. 46). 185 páginas.
**Arquivos:** `./GTQQ/References/[Applied social research methods series 46]...pag 130-134.pdf` (extração) + `...libgen.li.pdf` (livro completo)

| | |
|---|---|
| **Autores** | Abbas Tashakkori, Charles Teddlie |
| **Instituição** | Louisiana State University |
| **País** | EUA |
| **Ano** | 1998 |
| **Editora** | Sage Publications (Thousand Oaks, CA) |
| **Setor/Contexto** | Metodologia / Ciências sociais e comportamentais — livro fundacional de métodos mistos |
| **Tipo** | Livro fundacional — cunha os termos "quantitizing" e "qualitizing" |

### Resumo
O livro que **cunhou os termos quantitizing e qualitizing** (p.126): "We have given the term quantitizing to the process of converting qualitative data into quantitative data" e "We refer to the reverse process (i.e., converting quantitative data to qualitative data) as qualitizing." Tudo na mesma página, 1998. Miles & Huberman (1994) usaram "quantitizing" informalmente; Tashakkori & Teddlie formalizaram e criaram o par simétrico. É o ground zero terminológico — tudo que veio depois (Sandelowski, Boyatzis, Onwuegbuzie, Nzabonimpa) parte daqui.

Nota: Boyatzis (1998) publicado no **mesmo ano** usa "quantitative translation" em vez de "quantitizing" — dois vocabulários propostos simultaneamente pro mesmo fenômeno. O de Tashakkori & Teddlie prevaleceu.

Foco aqui: **Cap 6 — "Alternatives to Traditional Data Analytic Strategies" (pp.112-136)**, que contém a fundação completa.

### Cap 6, primeira metade (pp.112-129) — O território analítico

**Table 6.1 (p.115) — Quantitative Data Analysis Matrix:**
Matriz 2×2 organizando todas as técnicas estatísticas por: (a) relação entre variáveis vs. diferenças entre grupos, e (b) intervalar/ordinal vs. ordinal/nominal. Chi-quadrado, phi, Cramer's V (pra nominais); Pearson, ANOVA, regressão, fatorial (pra intervalares). O modelo DIME do Onwuegbuzie (2025) é expansão e reorganização desta tabela original.

**Table 6.2 (p.118) — Qualitative Data Analysis Matrix:**
Primeira tipologia de métodos qualitativos organizada por complexidade × origem dos temas:

| | A priori (dedutivo) | Emerging (indutivo) |
|---|---|---|
| **Simples** | Simple valence analysis, manifest content analysis | — |
| **Complexo** | Effects matrices (Miles & Huberman) | Latent content analysis, constant comparative (Glaser & Strauss), Developmental Research Sequence (Spradley) |

O Qualia Coding opera em todos os quadrantes: códigos a priori + emergentes, análise simples (frequência) + complexa (co-ocorrência, clustering).

**Heurística do número de categorias (p.119):**
"Typically, when analyzing data sets with 200 or fewer units of information... the initial number of categories emerging from such a database may be 10 to 15, but through combining similar groups of responses... the number can be reduced to 6 to 8." Empírico e prático — se o codebook tem 40 códigos, provavelmente tem redundância. O dendrograma do Qualia Coding deveria sugerir fusões.

**Manifest vs. latent content (pp.121-123):**
- **Manifest** = o dito explicitamente (contável, binarizável) → conecta com "the said" do Nzabonimpa
- **Latent** = o significado subjacente (interpretativo, não diretamente contável) → conecta com "the semi-said"

A distinção é de 1998 — Nzabonimpa (2018) a redescobre 20 anos depois com vocabulário novo.

**Constant comparative analysis (p.123):**
Glaser & Strauss (1967): (a) unitizing (quebrar texto em unidades codificáveis) + (b) categorizing (agrupar unidades em categorias). É literalmente o que o Qualia Coding implementa: pesquisador seleciona trecho (unitizing) e aplica código (categorizing).

**Quantitizing — onde o termo é cunhado (pp.126-129):**
Três abordagens definidas:
1. Contagem de frequência de temas na amostra
2. Porcentagem de temas por categoria de respondente
3. **Presença/ausência** de cada código por participante — a binarização que Macia, Henry e Driscoll operacionalizam depois

"The results can then be compared with the data from quantitative data collection" — é o merge que o Driscoll faz 9 anos depois com NVivo + Access + SAS.

### Cap 6, segunda metade (pp.130-134) — Qualitizing e os 5 perfis

**Qualitizing — cunhagem do par simétrico (p.126/130):**
Inspirados no quantitizing de Miles & Huberman (1994), criam o termo complementar: qualitizing. Definem como construção de perfis narrativos a partir de dados quantitativos.

**Box 6.3 (p.130) — Exemplo de qualitização:**
Hooper (1994), estudo sobre motivação em tarefas de linguagem. Dados quantitativos (rating scales) → categorias qualitativas ("assigning a category to each range of scores"). Ciclo completo: quali (entrevistas) + quanti (ratings) → quali de novo (categorias).

**Os 5 tipos de perfis qualitativos (pp.130-133):**

| Tipo | O que faz | Exemplo |
|---|---|---|
| **Modal** | Descrição baseada no atributo mais frequente | "Se a maioria tem 50 anos, o grupo é de meia-idade" |
| **Average** | Descrição baseada na média | Tashakkori, Boyd & Sines (1996): Hispanic dropouts — perfil híbrido (modal + average + holístico) |
| **Holistic (inferential, summative)** | Impressões gerais do investigador | O mais vulnerável a viés mas mais rico conceitualmente |
| **Comparative** | Comparação entre unidades via cluster analysis | Fals-Stewart et al. (1994): 102 casais, MMPI → cluster analysis → 5 tipos (conflicted, depressed, etc.) → nomeação verbal = **exatamente o que Macia faz** |
| **Normative** | Comparação com normas/padrões | Wetzler et al. (1994): deprimidos no MMPI → "code types" → "They are confused, ineffective, and unable to see solutions..." |

**Aviso sobre viés (p.133):** "Most profiles assume group homogeneity by taking modal and/or average information" e "the investigators' subjective analysis might affect the results. This is specifically true regarding holistic profiles." Conecta com espelho/janela: perfil holístico é o mais "espelho" de todos.

**Typology development vs. profile formation (pp.133-134):**

Distinção que nenhum outro paper faz claramente:
- **Profile:** QUAN → QUAL (narrativa descritiva a partir de dados numéricos — qualitização)
- **Typology:** QUAL → QUAN (classificação qualitativa validada quantitativamente)

Dois subtipos de sequential QUAL-QUAN:
1. **Forming groups + comparing on QUAN:** Quali classifica pessoas em tipos → compara em variáveis quanti (ANOVA, discriminant function). "Que variável discrimina os tipos?"
2. **Construct identification + construct validation:** Temas quali viram categorias → survey → análise fatorial confirmatória valida. Ex: Iwanicki & Tashakkori (1994) — "proficiencies of effective principals" extraídas quali, validadas por fatorial. Algumas confirmaram, outras migraram.

### Qualitização implícita e explícita

O livro trata qualitização **explicitamente** — é onde o termo nasce. Mas o exemplo comparativo (Fals-Stewart, clusters MMPI) mostra que a **prática** já existia antes do nome: cluster analysis → nomeação verbal de tipos é qualitização, feita em psicologia clínica sem usar esse vocabulário. Confirmação da hipótese central: qualitização é prática antiga, sub-denominada.

### Conexão com obsidian-qualia-coding

1. **A heurística 10-15 → 6-8 códigos** como métrica de saúde do codebook. O plugin poderia avisar: "Seu codebook tem 35 códigos — o dendrograma sugere que 12 são redundantes"
2. **Manifest vs. latent** como dois modos de codificação que o pesquisador pode explicitar
3. **Profile vs. typology** como dois pipelines de analytics: profile (QUAN→QUAL, qualitizar output) vs. typology (QUAL→QUAN, validar classificação)
4. **A binarização (tipo 3 de quantitizing)** é exatamente o scoring tipo (b) do Boyatzis e o que o plugin faz na co-ocorrência

### Referências anteriores a investigar

Os autores construíram a base ao longo de décadas. Referências que podem ter material mais antigo sobre esses conceitos:
- Tashakkori, Boyd & Sines (1996) — o estudo de Hispanic dropouts com perfis híbridos
- Tashakkori & Thompson (1991); Tashakkori, Thompson & Mehryar (1987) — surveys longitudinais no Irã com mixed methods
- Miles & Huberman (1994) — onde "quantitizing" aparece informalmente pela primeira vez

---

## 9. De Lisle, J. (2011). The Benefits and Challenges of Mixing Methods and Methodologies: Lessons Learnt From Implementing Qualitatively Led Mixed Methods Research Designs in Trinidad and Tobago

**Fonte:** Caribbean Curriculum, 18, 87-120.
**Arquivo:** `./GTQQ/The Benefits and Challenges of Mixing Methods and Methodologies.pdf`

| | |
|---|---|
| **Autor** | Jerome De Lisle |
| **Instituição** | University of the West Indies |
| **País** | Trinidad e Tobago |
| **Ano** | 2011 |
| **Journal** | Caribbean Curriculum |
| **Setor/Contexto** | Educação — designs qualitatively-led em políticas educacionais no Caribe |
| **Tipo** | Artigo teórico-empírico (survey do campo + 2 case studies) |

### Resumo
Survey abrangente do campo de mixed methods com foco em designs onde o qualitativo lidera ou tem peso igual. Primeira parte teórica: paradigm wars, emergência do terceiro paradigma, tipologias de design, stances filosóficas. Segunda parte empírica: 2 estudos em Trinidad e Tobago (escolha de escola secundária + escolas com baixo desempenho). O foco aqui é na contribuição teórica/epistemológica — os case studies são contextuais.

### Contribuição 1 — As 5 stances filosóficas (Greene, 2006, 2007)

Cinco posições que justificam por que e como misturar paradigmas:

| Stance | Posição | Implicação |
|---|---|---|
| **A-paradigmatic** | Desconecta paradigma de metodologia — método é ferramenta, não cosmovisão | Mais liberdade técnica, menos rigor epistemológico |
| **Alternative** | Propõe novos modelos mentais pra guiar a prática | Busca framework próprio pro mixed methods |
| **Complementary strengths** | Cada método tem forças filosóficas próprias que devem ser honradas | Implementa cada strand dentro do seu paradigma original |
| **Substantive** | Entrelaça paradigma e questões substantivas | O problema de pesquisa determina a combinação |
| **Dialectic** | As diferenças entre paradigmas são a fonte de novos insights | A tensão é produtiva — não resolve, explora |

Isso dá vocabulário pra posicionar cada autor que lemos:
- **Boyatzis / Sandelowski:** pragmatistas (a-paradigmatic tendendo a substantive) — "o que funciona, funciona"
- **Gerrish / Giddings:** dialectic com cautela — reconhecem a tensão e temem que o mixing suavize as diferenças em vez de explorar
- **Nzabonimpa:** substantive — o problema (escola, gênero, Ruanda) determina o mix
- **Macia / Henry:** a-paradigmatic na prática — usam o método sem discutir paradigma

### Contribuição 2 — A advertência de Giddings (2006)

"Clothed in a semblance of inclusiveness, mixed methods could serve as a cover for the continuing hegemony of positivism, and maintain the marginalisation of non-positivist research methodologies." (Giddings, 2006, p. 195)

Mais radical que a Gerrish: não diz só "cuidado, pode diluir riqueza qualitativa" — diz "o mixed methods inteiro pode ser roupagem inclusiva pra manter o positivismo no comando." De Lisle reconhece: "perhaps there was some validity to these fears" — pesquisa ruim mascarada de mixed methods frequentemente viola pressupostos dos dois paradigmas, com o quali em papel subserviente.

Conecta com a assimetria do Nzabonimpa: se software e comunidade favorecem quantitização, e se o quali frequentemente fica subserviente no mix, a infraestrutura reforça a hegemonia positivista que Giddings denuncia. O Qualia Coding, paradoxalmente, pode ser ferramenta de resistência: software de QDA que oferece analytics — mas precisa oferecer analytics que **sirvam ao quali**, não que convertam o quali em quanti como fim em si.

### Contribuição 3 — Definição de consensus e subtipos (Johnson et al., 2007)

"Mixed methods research is the type of research in which a researcher combines elements of qualitative and quantitative research approaches for the broad purposes of **breadth and depth of understanding and corroboration**." (Johnson et al., 2007, p. 123 — síntese de 19 definições)

Três subtipos: qualitative dominant, pure mixed, quantitative dominant. Classificação dos papers que lemos:
- **Macia, Henry:** quantitative dominant (quali vira input pro quanti via binarização e clustering)
- **Nzabonimpa:** pure mixed (faz quantitização e qualitização com peso igual)
- **Sandelowski (2001):** qualitative dominant (números servem ao quali, não o contrário)
- **Driscoll:** quantitative dominant (merge pra análise estatística)
- **Boyatzis:** posiciona análise temática como ponte — pode servir qualquer subtipo

### Conexão com o Foundations.md
As 5 stances e a advertência de Giddings alimentam diretamente as seções epistemológicas do Foundations (1.1, 1.2). A classificação dominant/pure/mixed dá framework pra posicionar o pipeline: quando o Qualia Coding oferece clustering e AC, está no modo quantitative dominant? Ou serve ao quali? A resposta depende de como o pesquisador usa — mas o design do plugin pode favorecer um ou outro. A distinção espelho/janela é relevante aqui: R-analysis (espelho) serve ao quali (auditar codebook); Q-analysis (janela) tende ao quanti (tipologias estatísticas). São modos diferentes com posicionamentos paradigmáticos diferentes.

---

## 10. Rodrigues, A. S. (2007). A definição do conceito de grupo e suas implicações no funcionamento do sistema: O caso das Equipas Cirúrgicas (Tese de Doutoramento)

**Fonte:** Universidade do Porto, Faculdade de Psicologia e Ciências da Educação. 472 páginas.
**Arquivo:** `./GTQQ/References/29879.pdf`

| | |
|---|---|
| **Autora** | Anabela Santos Rodrigues |
| **Instituição** | Universidade do Porto, FPCEUP / CITTE |
| **País** | Portugal |
| **Ano** | 2007 |
| **Tipo** | Tese de doutoramento em Psicologia |
| **Orientadores** | Prof. José Miguez (orientador), Prof. Paulo Renato Lourenço (co-orientador) |
| **Setor/Contexto** | Psicologia dos grupos / Saúde — dinâmica de equipas cirúrgicas (bloco operatório). Foco aqui: capítulo metodológico (Cap IV, pp.104-215) |

### Resumo (foco metodológico)

Tese sobre dinâmica de grupos em equipas cirúrgicas — mas o **capítulo metodológico** (Cap IV, ~110 páginas) é uma contribuição densa sobre métodos mistos, validade, integração quali-quanti, e controlo de qualidade das inferências. Fonte citada extensivamente no Foundations.md (Rodrigues, 2007 aparece múltiplas vezes). Escrita em português europeu, sintetiza a literatura anglo-saxónica com perspectiva lusófona.

### Contribuição 1 — A distinção quantificação vs. quantitização (pp.138-139)

A formalização mais clara em português da fronteira entre contar e transformar:

**Quantificação:** "Apenas uma quantificação da informação qualitativa" — contagens de frequência que mantêm a natureza qualitativa dos dados. Os números são descritivos, não operáveis estatisticamente. É o que a Sandelowski (2001) defende: números servem ao quali sem mudar sua natureza.

**Quantitização:** "Uma forma de transformação dos dados qualitativos em quantitativos" que "pressupõe uma recodificação de cada categoria, com a atribuição de códigos numéricos" permitindo análises estatísticas subsequentes. Os dados **mudam de natureza**.

**O conflito:** Nem todos concordam onde fica a fronteira. Sandelowski (2001, nota 82) cita Onwuegbuzie & Teddlie (2003) e Boyatzis (1998) entre autores que consideram que "a vertente mais quantitativa da análise de conteúdo, como as contagens, constitui uma forma de quantitização." A Rodrigues discorda — pra ela, contar não é transformar. E a própria Sandelowski muda de posição entre papers: em 2001 defende contagem como parte do quali; em 2000 define quantitizing como transformação.

**Implicação pro Qualia Coding:** O plugin opera nos dois lados da fronteira. Frequência de códigos = quantificação (descritivo, mantém o quali). Exportar co-ocorrência matrix pra clustering/AC = quantitização (transforma natureza do dado). A ferramenta deveria explicitar em qual lado o pesquisador está operando.

### Contribuição 2 — Theoretical drive (p.139, nota 92, citando Morse 2003)

"A direção global, principal ou básica de um projecto de investigação, que pode ser indutiva ou dedutiva." Rodrigues reinterpreta: não é sobre paradigma (quanti vs. quali) mas sobre **estratégia** — as técnicas dominantes na recolha e análise. Conecta com os subtipos do Johnson et al. (2007) que documentamos via De Lisle: qualitative dominant, pure mixed, quantitative dominant.

### Contribuição 3 — Double-coding como controle inter-rater (pp.189, 204)

Rodrigues usou check-coding com 2 codificadores independentes no NUD*IST (QSR N6). Resultado: 89% de consenso inicial → ajustes em definições e codificações → 98.4% de consenso no segundo round. Praticamente **blind scoring** — os codificadores não sabiam as fontes.

Conecta diretamente com a discussão **espelho vs. janela**: se dois codificadores independentes veem a mesma co-ocorrência, é evidência de que o padrão é do fenômeno, não artefato do codificador individual. O inter-rater é o mecanismo que transforma espelho em janela. É o que o Boyatzis fez (caso Dreyfus, 79%) com rigor ainda maior (98.4%).

### Contribuição 4 — 9 tipos de legitimação (pp.129-130, citando Onwuegbuzie & Johnson 2006)

Tipologia de formas de legitimação em métodos mistos, incluindo:

| Tipo | O que avalia |
|---|---|
| a) Integração da amostra | Relação entre desenho amostral quali/quanti |
| b) Inside-outside | Equilíbrio emic (participante) / etic (investigador) |
| c) Minimização das fraquezas | Compensação mútua das abordagens |
| d) Sequenciação | Impacto da ordem quali→quanti vs. quanti→quali |
| **e) Conversão** | **"O grau em que a qualitização e a quantitização produzem meta-inferências com qualidade"** |
| f) Combinação paradigmal | Integração de crenças epistemológicas |
| g) Comensurabilidade | Se as meta-inferências produzem um terceiro ponto de vista |
| h) Validades múltiplas | Uso de formas de validade quali, quanti e mistas |
| i) Política | Se consumidores valorizam as meta-inferências |

O **tipo (e) — legitimação de conversão** é específico pra transformação de dados. É o único tipo de legitimação na tipologia dedicado a avaliar se a quantitização/qualitização foi bem feita. Conecta com toda a discussão que temos: a J-curve do Boyatzis, as armadilhas da Sandelowski, a assimetria do Nzabonimpa, a diluição da Gerrish — todos são aspectos de legitimação de conversão.

### Contribuição 5 — Integração como complementaridade (p.195)

A integração da tese foi por complementaridade, não triangulação: "encarando as possíveis faltas de convergência como oportunidades de interpretação." Divergências entre quali e quanti não invalidam — enriquecem. Ecoa a stance dialectic do Greene: a tensão é produtiva.

### Contribuição 6 — Software QDA e a tensão espelho/janela (p.192, Quadro 3)

Citando Bazeley (2003, p.385): software QDA permite "transforming os códigos qualitativos num formato que permite a análise estatística." Desvantagem correspondente: "podem tirar o lugar de uma análise cuidadosa do material" (Creswell, 1998; Silverman, 2000). É a tensão espelho/janela formulada em 2007: a ferramenta facilita a transformação mas pode substituir o pensamento.

### Qualitização implícita

A tese não faz qualitização no sentido técnico (não usa clustering nem AC). Mas o Cap VI inteiro (Respostas às Questões de Investigação, pp.224-415) é qualitização na acepção ampla: dados de observação estruturada (frequências de comportamentos) são interpretados qualitativamente como evidência de dinâmicas grupais. "Síntese reflexiva da informação recolhida" é o heading que se repete — é qualitização como prática, sem o nome.

### Contribuição 7 — As 4 posições sobre validade e o que cada uma diz sobre transformação de dados (pp.122-125)

Rodrigues sintetiza 4 posições sobre validade em investigação qualitativa — e cada uma implica uma atitude diferente sobre transformação de dados:

**1. Posição Positivista**
Aplica critérios quanti ao quali sem adaptação: validade interna, externa, de constructo, de conclusão estatística (Cook & Campbell, 1976, 1979). Transformação é legítima se mantém **validade estatística**. Os critérios são: J-curve controlada (Boyatzis), N amostral suficiente (Henry), independência entre variáveis (Driscoll), pressupostos paramétricos respeitados. É a posição implícita de todos os papers técnicos que lemos — nenhum questiona se transformar é legítimo, só se a transformação é tecnicamente correta.

**2. Posição Neo-positivista (duas sub-posições)**

(a) **Tradução de etiquetas:** Guba (1981) — validade interna → credibilidade, validade externa → transferabilidade, validade de constructo → confirmabilidade, conclusão estatística → dependência. Transformação é legítima se mantém **credibilidade e transferabilidade**. Mecanismos: double-coding (Rodrigues: 89%→98.4%), audit trail (Sandelowski 2001), member checking. É a posição que trata o quali como ciência que precisa de rigor, mas com vocabulário próprio.

(b) **Seleção de critérios:** Miguez (2005), Trochin (1999) — usa apenas validade de constructo e validade inferencial, descartando validade interna e externa (que não fazem sentido no quali). Transformação é legítima se as **inferências são defensáveis** — não precisa de generalização, precisa de qualidade argumentativa. Mais flexível que (a).

**3. Posição Integradora (duas sub-posições)**

(a) **Reconceptualização parcial:** Whittemore et al. (2001) — critérios primários (credibilidade, autenticidade, criticalidade, integridade) + secundários (explicitness, vividness, criatividade, thoroughness, congruência, sensibilidade). Transformação é legítima se preserva **autenticidade** e produz resultados com **vividness** — ou seja, se os números não matam a vivacidade do dado qualitativo. A legitimação de conversão (Onwuegbuzie & Johnson, tipo e) opera aqui.

(b) **Reconceptualização radical:** Guba & Lincoln (1989) — 5 critérios de autenticidade: *fairness* (equilíbrio de perspectivas), *autenticidade ontológica e educativa* (consciência), *autenticidade catalítica e táctica* (indução de ação). Transformação é legítima se mantém **fairness** — todas as vozes representadas, nenhuma omitida pela binarização. Conecta com o "unsaid" do Nzabonimpa: se a transformação omite vozes que o quali capturava, viola fairness.

**4. Posição Interpretativa**
Rejeição total do conceito de validade. Schwandt (1996): "adeus à criteriologia." Ellis (1999): **evocação** como critério — "o facto de a história evocar, no leitor, o sentimento de que a experiência descrita é autêntica e possível." Richardson (1997): **cristalização** substitui triangulação — "a imagem central da validade da investigação qualitativa é o cristal e não o triângulo. Os cristais mudam, alteram-se, reflectem a exterioridade e refractam." Transformação pode ser **ilegítima por princípio** — binarizar é violentar o dado, reduzir o cristal a um ponto. É a posição da Gerrish levada ao extremo, e a posição que a advertência de Giddings (2006) protege.

**Síntese — transformação de dados vista por cada posição:**

| Posição | Transformação é legítima quando... | Critério central | Autores-chave |
|---|---|---|---|
| **Positivista** | Mantém validade estatística | Rigor técnico | Cook & Campbell, Boyatzis |
| **Neo-positivista** | Mantém credibilidade e transferabilidade | Rigor adaptado | Guba, Miguez, Trochin |
| **Integradora** | Preserva autenticidade e vividness | Qualidade interpretativa | Whittemore, Guba & Lincoln |
| **Interpretativa** | Quase nunca — binarizar violenta o dado | Evocação / cristalização | Schwandt, Ellis, Richardson |
| **Pragmatista** | Produz conhecimento útil | Funciona? | Tashakkori, Sandelowski, todos os papers técnicos |

A maioria dos papers que lemos opera na **posição pragmatista** (não listada por Rodrigues, mas implícita): não discutem paradigma, usam o que funciona. O Foundations.md tende pra integradora — busca autenticidade na transformação sem rejeitar a transformação. A Gerrish é neo-positivista cautelosa. A Giddings é interpretativa preocupada.

**Pro Qualia Coding:** O plugin deveria ser agnóstico de posição — funcionar pra qualquer uma. Mas a **comunicação** dos resultados deveria respeitar a posição do pesquisador. Um positivista quer p-valores e intervalos de confiança. Um integrativista quer narrativa + números lado a lado. Um interpretativista pode nem querer usar os analytics. A interface deveria adaptar.

### Conexão com o Foundations.md

A Rodrigues (2007) é fonte direta do Foundations.md — citada extensivamente pra: bricolagem metodológica, theoretical drive, distinção quantificação/quantitização, cartões de pertença (card sorting). É a voz lusófona que traduz e contextualiza a literatura anglo-saxónica (Tashakkori, Sandelowski, Morse, Onwuegbuzie) pro contexto europeu.

---

## 11. Sandelowski, M. (2000). Combining Qualitative and Quantitative Sampling, Data Collection, and Analysis Techniques in Mixed-Method Studies

**Fonte:** Research in Nursing & Health, 23, 246-255.
**Arquivo:** `./GTQQ/Combining Qualitative and Quantitative Sampling 2000.pdf`

| | |
|---|---|
| **Autora** | Margarete Sandelowski |
| **Instituição** | University of North Carolina–Chapel Hill, School of Nursing |
| **País** | EUA |
| **Ano** | 2000 |
| **Journal** | Research in Nursing & Health |
| **Setor/Contexto** | Metodologia / Enfermagem — artigo fundacional que formaliza e expande quantitização/qualitização |
| **Tipo** | Artigo teórico-metodológico (Focus on Research Methods) |

### Resumo
Dois anos após Tashakkori & Teddlie (1998) cunharem os termos, Sandelowski formaliza e expande quantitizing/qualitizing dentro de um framework mais amplo de combinações técnicas em mixed methods. Cobre sampling, coleta e análise. A contribuição específica: posiciona **transformação de dados** como conceito guarda-chuva, com quantitização e qualitização como os dois processos direcionais dentro dele. Distingue transformação de dados (converter um tipo no outro) de linking (combinar datasets sem converter).

### Contribuição principal — Linking vs. Transforming

Duas estratégias de combinação de dados (p.252):

- **Linking:** Tratar cada dataset com suas técnicas nativas (quali com quali, quanti com quanti) e combinar **na interpretação**. Datasets permanecem analiticamente separados.
- **Transforming:** Converter um tipo de dado no outro pra criar **um dataset unificado**. É aqui que entra quantitizing/qualitizing.

### Figure 1 — Os 7 design templates (p.249)

Primeira sistematização visual dos designs de combinação:

| Template | Design | Adjunct QUAL | Adjunct QUAN |
|---|---|---|---|
| #1 | QUAL>quan | | measured description, validation |
| #2 | QUAN>qual | explanation, validation | |
| #3 | quan>QUAL | | guide sampling, suggest paths |
| #4 | Qual>QUAN | generate items, hypotheses | |
| #5 | Quan ↔ Qual (rolling waves) | ambos | ambos |
| **#6** | **Qual>Quan>Qual** | | **instrumental bridge** |
| #7 | Quan>Qual>Quan | fieldwork bridge | |

O **template #6 (Qual>Quan>Qual) é exatamente o pipeline que estamos documentando**: começa qualitativo (codificação) → transforma em quantitativo (binarização, clustering, AC) → volta pro qualitativo (interpretação, nomeação, perfis). O Foundations.md descreve isso como ciclo infinito — aqui é formalizado como design template específico.

### Borkan et al. (1991) — o exemplo elegante (p.253)

Estudo com idosos e fraturas de quadril: narrativas sobre como a fratura aconteceu → análise narrativa identificou 2 **emplotments** (mechanical: "broke hip before falling" e organic: "fell and broke hip") → reliability testing → agruparam idosos por tipo de narrativa → correlação com outcomes funcionais. **A narrativa orgânica predisse melhor recuperação que a mecânica.**

É um dos exemplos mais elegantes de quantitização: não é binarização bruta (0/1), é **tradução de tipo narrativo em variável categórica** que mantém riqueza interpretativa. O tipo de história que a pessoa conta sobre sua fratura prediz o futuro funcional. Qualitativo vira variável preditora sem perder significado. É o que a Gerrish diria ser impossível (traduzir sem diluir) — e funciona.

### Qualitizing como explicitação (p.254)

"Qualitizing entails further studying these theoretical groups to explicate the features of members in each group that make them like each other and the groups themselves different from each other, and to choose a name that will capture these features."

Qualitizar não é só dar nome — é **explicar as features** que fazem o grupo ser grupo. A Macia faz exatamente isso nos clusters 5 vs 6: não só nomeia, mas explica que o vínculo com a outra pessoa é o que os diferencia.

### "Qualitative quagmire" — o aviso (p.254)

Barbour (1998) alerta sobre pesquisa ruim mascarada de mixed methods. Chen (1997): "mixed-method research is in danger of becoming the new ideology." Ecoa Giddings (2006) no De Lisle. A Sandelowski endossa: "mixed-method research should never be used because of the misguided assumptions that more is better."

### Posição na genealogia

Este paper é o **elo entre** Tashakkori & Teddlie (1998) e Sandelowski (2001, "Do Not Count") e (2009, ciclo infinito). Cronologia:
- **Caracelli & Greene (1993):** Usam "transformation" como estratégia — o conceito guarda-chuva
- **Miles & Huberman (1994):** "Quantitizing" aparece informalmente
- **Tashakkori & Teddlie (1998):** Formalizam quantitizing/qualitizing como par de termos
- **Boyatzis (1998):** "Quantitative translation" — vocabulário concorrente (mesmo ano)
- **Sandelowski (2000):** **Este paper** — costura vocabulários: transformação como estratégia, quantitização/qualitização como processos dentro dela. Distingue de linking.
- **Sandelowski (2001):** Legitima números dentro do quali
- **Sandelowski, Voils & Barroso (2009):** Ciclo infinito

### Qualitização implícita

O paper trata qualitização explicitamente (seção "Qualitizing", p.253), repetindo os 5 perfis de T&T 1998. Mas o exemplo do Borkan (emplotments → variável preditora) é mais rico que os perfis: mostra que qualitização pode ser a **origem** da variável, não só a interpretação do output.

### Conexão com obsidian-qualia-coding

O template #6 (Qual>Quan>Qual) é o pipeline que o plugin deveria suportar: codificação → analytics (clustering, AC, MDS) → interpretação qualitativa (nomeação, perfis, retorno ao texto). A distinção linking vs. transforming sugere dois modos de analytics: um que mantém quali e quanti separados (linking = views separadas), outro que integra num dataset unificado (transforming = merge como o Driscoll).

### Referência a investigar

**Caracelli, V.J. & Greene, J.C. (1993).** "Data analysis strategies for mixed-method evaluation designs." *Educational Evaluation and Policy Analysis*, 15, 195-207. — Onde "transformation" aparece como estratégia pela primeira vez. Ground zero do conceito. Campo: avaliação educacional (não ciências sociais nem saúde). Confirma que a prática atravessa disciplinas.

---

## 12. Sandelowski, M. (2001). Real Qualitative Researchers Do Not Count: The Use of Numbers in Qualitative Research

**Fonte:** Research in Nursing & Health, 24, 230-240.
**Arquivo:** `./GTQQ/Real Qualitative Researchers Do Not Count - The Use of Numbers in Qualitative Research.pdf`

| | |
|---|---|
| **Autora** | Margarete Sandelowski |
| **Instituição** | University of North Carolina–Chapel Hill, School of Nursing |
| **País** | EUA |
| **Ano** | 2001 |
| **Journal** | Research in Nursing & Health |
| **Setor/Contexto** | Metodologia / Enfermagem / Ciências sociais — artigo teórico sobre o uso de números em pesquisa qualitativa |
| **Tipo** | Artigo teórico-argumentativo (Focus on Research Methods) |

### Resumo
A Sandelowski — mesma autora que formalizou quantitização/qualitização (2000) e expandiu o ciclo infinito quali↔quanti (2009, com Voils e Barroso) — desmonta dois mitos: que pesquisadores qualitativos "de verdade" não contam, e que pesquisadores qualitativos não sabem contar. Argumenta que números são **integrais** à pesquisa qualitativa, não estranhos a ela: "meaning depends, in part, on number" (Dey, 1993). Toda codificação já é atribuição de dados nominais que podem ser scored. A contagem não é oposto da interpretação — é parte dela.

### Problema
Os "antinumber myths" levaram à subutilização, sub-reconhecimento e até evitação de números em pesquisa qualitativa. Isso empobrece a pesquisa e cria uma visão simplista de que qualitativo = palavras e quantitativo = números. Sandelowski quer legitimizar o uso de números no quali, mostrando quando é produtivo e quando é armadilha.

### As 4 funções dos números em pesquisa qualitativa

**1. Gerar significado (Generating Meaning)**
Contar é integral ao reconhecimento de padrões. "Finding that a few, some, or many participants showed a certain pattern implies something about frequency, typicality, or even intensity." A contagem é frequentemente **inconsciente** — o pesquisador "sente" que um padrão é comum sem perceber que está contando. Toda vez que codifica temas, está atribuindo dados nominais (presença/ausência) — scoring tipo (b) do Boyatzis, sem saber.

Sandelowski cita Tashakkori & Teddlie (1998, p.126) pra "quantitizing" e Boyatzis (1998, p.129) pra "quantitative translation" — posiciona os dois como complementares e contemporâneos. E vai além: a quantitização dentro do quali é **mais antiga e mais disseminada** do que o nome sugere.

Exemplo: Blaxter (1983) listou frequência de 11 categorias de doenças mencionadas por 46 mulheres. Tuberculose era a mais mencionada (n=36) MAS a menos discutida em termos de causa. Esse achado — a doença mais comum é a menos explicada — emergiu do **número**, não da leitura qualitativa. A contagem revelou uma lacuna interpretativa.

**2. Documentar, verificar e testar conclusões**
Números dão audit trail — mostram que o pesquisador "accounted for all and have not discounted any" dos dados. Evitam as 3 armadilhas clássicas: (a) overweighting dramatic accounts, (b) underweighting dados que não confirmam a interpretação, (c) "regressing to the mean" — suavizar contradições.

Exemplo próprio (Sandelowski & Jones, 1996): Table 2 mostra semanas gestacionais com/sem conhecimento de diagnóstico fetal pra 12 casais. O display numérico revelou que casais que terminaram a gravidez tinham recebido diagnóstico mais cedo (antes de 21 semanas) que os que continuaram (depois de 18 semanas). Invisível nas narrativas.

Conceito de **"number play"**: uso exploratório de números em dados qualitativos. "Playing this number game not only enabled me to see my data in a new way, but also to see more about the characteristics of my sample." É a quantitização exploratória (DIME nível 4) vinda de dentro da tradição qualitativa, não da tradição mista.

**3. Re-presentar dados e vidas**
Tabelas e números comunicam padrões qualitativos com mais clareza que texto em certas situações. Pesquisadores qualitativos preferem "figures of speech over figures, and tableaux of experience over tables of numbers" — mas displays numéricos podem complementar sem substituir.

Exemplo: Figure 2 (Borkan et al., 1991) — display híbrido com números E quotes lado a lado numa escala de "Organic → Mechanistic". Scores numéricos posicionados num continuum nomeado qualitativamente, com falas dos pacientes ilustrando cada posição. É qualitização visual pura.

Figure 4 (Simon, 1999) — mapa esquemático de dinâmicas espaciais numa conferência de diagnóstico por imagem: posição dos participantes (homens e mulheres) com shading numérico pra dar credibilidade à interpretação sobre gender dynamics. O número sustenta a narrativa, não substitui.

**4. Evitar as armadilhas da contagem**

### As 4 armadilhas — guardrails diretos pro Qualia Coding

**Verbal counting:** Usar "a few", "some", "many", "most" sem definir operacionalmente. O leitor não sabe o que significa. Solução: definir — "common = occurring in more than 50% of participants; few or rarely = occurring in less than 20%." Implicação pro plugin: se o analytics mostra "frequente" ou "raro", precisa explicitar o threshold.

**Overcounting — representational:** Contar o que deve ser contado, mas exibir de forma que números dominam. "3 women said this... 6 women said that..." — legítimo mas esteticamente desastroso e distrai do conteúdo. Solução: integrar números na narrativa, não listar. Implicação pro plugin: views de analytics devem sempre mostrar o contexto (o segmento codificado), não só a contagem.

**Overcounting — analytic:** Contar tudo que é contável, mesmo que não adicione compreensão. Se encontrou 5 padrões entre 25 mulheres com HIV, documentar que "5 showed Pattern A, 10 showed Pattern B, 7 showed Pattern C, 1 showed Pattern D, 2 showed Pattern E" é menos importante que descrever o que cada padrão **é** qualitativamente. "Patterns has less importance than detailing the patterns themselves." Implicação pro plugin: a view de frequência de códigos não deve ser a primeira coisa que o pesquisador vê — a co-ocorrência e o conteúdo são mais informativos.

**Misleading counting:** Porcentagens em amostras pequenas. "50% of the sample" quando N=2. Regra de ouro: **se N < 25, use números absolutos**. Implicação pro plugin: se o dataset tem menos de 25 documentos/casos, não mostrar porcentagens — só contagens absolutas.

**Acontextual counting:** Contar sem contexto qualitativo. "40% of the children were angry" sem dizer mais nada. Ou contar menções e concluir importância — quando repetição pode ser retórica, não indicador de saliência. Implicação pro plugin: toda contagem precisa de link pra o contexto original.

### Qualitização implícita

O paper inteiro é sobre quantitização dentro do quali — mas contém qualitização em vários pontos:

- **Table 2** (período de conhecimento de diagnóstico fetal): datas numéricas (semanas gestacionais) transformadas em narrativa sobre experiência temporal dos casais. Números → insight qualitativo sobre impacto do timing.
- **Figure 2** (Borkan et al., 1991): display híbrido Organic↔Mechanistic. Scores posicionados num continuum nomeado qualitativamente + quotes. Qualitização visual.
- A própria **conclusão** é um ato de qualitização: ela pega todo o argumento numérico do paper e traduz na frase "The desire to move 'beyond numbers' should not prevent qualitative researchers from using numbers to get there."

### Posição na genealogia do campo

Este paper (2001) é o **elo entre** o artigo fundacional sobre quantitização/qualitização (Sandelowski, 2000) e o framework expandido do ciclo infinito (Sandelowski, Voils & Barroso, 2009). Cronologia:
- **2000:** Formaliza quantitização/qualitização como conceitos (artigo "Combining Qualitative and Quantitative Sampling")
- **2001:** Este paper — argumenta que números já são parte do quali, destrói o mito da separação
- **2009:** Expande o framework mostrando que quantitização e qualitização se implicam mutuamente (ciclo infinito)

A progressão é: primeiro nomeou os processos (2000), depois legitimou os números dentro do quali (2001), depois mostrou que os processos são cíclicos e inseparáveis (2009). É a autora construindo o argumento ao longo de uma década.

### Conexão com obsidian-qualia-coding

As 4 armadilhas são **guardrails de design** diretos:
1. **Verbal counting** → definir thresholds explícitos nas views (o que significa "frequente"?)
2. **Representational overcounting** → nunca mostrar contagem sem contexto (segmento codificado acessível)
3. **Analytic overcounting** → não fazer da frequência a view default — co-ocorrência e conteúdo primeiro
4. **Misleading counting** → não mostrar porcentagens com N < 25
5. **Acontextual counting** → toda contagem com link pro contexto original

---

## 13. Sandelowski, M., Voils, C. I., & Knafl, G. (2009). On Quantitizing

**Fonte:** Journal of Mixed Methods Research, 3(3), 208-222.
**Arquivo:** `./GTQQ/References/On Quantitizing.pdf`

| | |
|---|---|
| **Autores** | Margarete Sandelowski, Corrine I. Voils, George Knafl |
| **Instituições** | UNC Chapel Hill, School of Nursing; Duke University / VA Medical Center |
| **País** | EUA |
| **Ano** | 2009 |
| **Journal** | Journal of Mixed Methods Research (SAGE) |
| **Setor/Contexto** | Metodologia — artigo teórico-filosófico sobre os fundamentos da quantitização |
| **Tipo** | Artigo fundacional — desconstrução epistemológica da quantitização. Terceiro e último da trilogia Sandelowski (2000 → 2001 → 2009) |

### Resumo

O paper mais filosófico e profundo da trilogia. Não apresenta técnica nem case study — desconstruí os **pressupostos** que todos os outros papers que lemos dão como dados: que existem dois tipos de dados, que contar é transparente, que 1/0 é simples, que quantitizar é unidirecional. É aqui que o ciclo infinito é formalmente proposto e fundamentado.

### Contribuição 1 — "Data-as-given" vs. "data-as-taken" (p.2)

A primeira conversão não é quali→quanti — é **experiência→dado**. Dados não são "dados" (given, existindo lá fora esperando coleta). São "tomados" (taken, construídos pelo pesquisador que decide o que anotar e o que ignorar).

Wolcott (1994, pp.3-4): "Everything has the potential to be data, but nothing becomes (italics in original) data without the intervention of a researcher who takes note—and often makes note—of some things to the exclusion of others."

Implicação: antes de qualquer quantitização, já houve um ato qualitativo radical — **selecionar**. O pesquisador decidiu que certas experiências merecem virar dado e outras não. Essa primeira conversão (experiência → dado) é mais consequencial que a segunda (dado quali → dado quanti), mas é invisível.

**Nota sobre posicionamento epistemológico:** O "data-as-taken" tem raízes construtivistas (Valsiner, 2000) — dados são construídos, não existem "lá fora." Mas Sandelowski **não se declara construtivista**. Opera numa zona deliberadamente pragmatista: usa o argumento construtivista como ferramenta pra desconstruir a ilusão positivista de que dados são neutros, mas não vai ao extremo construtivista de que não existe realidade externa.

A posição é mais sutil: **existe experiência** (real, vivida pelos participantes), mas o que vira **dado** é produto de decisão do pesquisador. A experiência não é construída; o dado é. É a diferença entre "a realidade é construída" (construtivismo forte) e "nossa representação da realidade é construída" (pragmatismo / realismo crítico).

Na prática: quando a Macia binariza queixas, as queixas **existiram** — imigrantes latinos viveram discriminação, dívida, conflitos reais. Mas o fato de que "support sought = família" virou 1 e "support sought = nenhum" virou 0 é construção da pesquisadora. A experiência é real; o 1/0 é tomado, não dado.

Essa posição permite usar métodos quantitativos (porque aceita que experiência é real e padrões existem) sem ser ingênuo sobre eles (porque reconhece que a representação é construída). É por isso que o ciclo infinito funciona sem cair em relativismo — há algo real pra ciclar, mas o ciclar é ato interpretativo. E é por isso que a pergunta "devo quantitizar?" faz sentido: não é "posso representar a realidade com números?" (positivista diria sim, construtivista diria não) — é "essa representação numérica **adiciona** algo à compreensão da experiência real?" (pragmatista).

### Contribuição 2 — "The Vagaries of Counting" — contar é ato interpretativo (pp.4-5)

Martin (2004, p.925): "To count a number of objects, we must render them distinct and discrete, so that we can tell what 'counts' as an object in question and what doesn't. We must have tricks or techniques to mark and exclude what has already been counted, to make sure that nothing is counted twice or not counted at all."

Contar exige tornar objetos "docile" — dar-lhes "clear and nonoverlapping boundaries." Mas experiência qualitativa resiste a isso — é "uncountable singular and indivisible" (Holliday, 2002, p.69). Contar é **violência ontológica necessária**: força discretude sobre o contínuo.

**O experimento de Schwarz (1999):** Escala 0-10 ("not at all successful" → "extremely successful") vs. escala -5 a +5 (mesmos anchors). 34% escolheram valores entre -5 e 0 na segunda escala, mas só 13% escolheram equivalentes formais (0-5) na primeira. Zero com label "not at all successful" = "ausência de achievements." Zero como ponto médio = "presença de explicit failures." **O mesmo número significa coisas diferentes dependendo do contexto.** Toda quantitização carrega essa ambiguidade.

**Outro exemplo:** Mulheres pedidas pra avaliar experiência de cesariana não-planejada de 0 (bad) a 10 (good). Nenhuma deu 0, mesmo as que contaram histórias altamente negativas. Uma disse: "I wouldn't put myself at a 0." Interpretavam como nota escolar — 0 é fracasso pessoal, não avaliação da experiência.

### Contribuição 3 — "1 (Present) Versus 0 (Absent)" — a binarização desconstruída (pp.8-9)

Desconstrução completa do scoring tipo (b) do Boyatzis — o mesmo que Macia, Henry e Driscoll usam:

**"Present" (1) pode significar:**
1. Surgiu espontaneamente na fala do participante
2. Foi direcionado pela pergunta do entrevistador
3. O analista viu entre as linhas (interpretação de conteúdo latente)
4. É realmente dimensão da experiência do participante
5. Refere-se a conteúdo informacional (o que a pessoa disse)
6. Refere-se a features narrativas/discursivas (como disse)
7. É produto da relação entrevistador-entrevistado (co-construção)

**"Absent" (0) pode significar:**
1. Não surgiu na conversa
2. O analista não viu (viés de percepção)
3. O participante esqueceu
4. Era tão óbvio pro participante que não precisava mencionar
5. Era fator mas o participante não quis falar (tabu, vergonha, medo)
6. A conversa desviou e não chegou lá
7. Realmente não era dimensão da experiência

"1 or 0 may signal a host of such diverse circumstances." Cada 1 e cada 0 numa matriz binarizada carrega 7+ significados possíveis — e o clustering/AC/MDS trata todos como equivalentes.

**O custo da binarização:** Cohen (1983, p.253): dicotomizar resulta em "significant losses of variance on the original variables" e perda de poder equivalente a "discarding one-third to two-thirds of the sample." A binarização que todo mundo usa (Macia, Henry, Driscoll, Qualia Coding) tem custo estatístico formal quantificado.

**Alternativa proposta:** Variáveis ordinais em vez de 0/1 — "not discernible → noted in passing → important → dominant." Preserva gradações que a binarização elimina. Mas não operacionaliza como fazer isso na prática.

### Contribuição 4 — O ciclo infinito formalizado (pp.5, 10)

"No clear line can be drawn between quantitizing and qualitizing as they entail each other." (p.5)

"Quantitative knowing depends on qualitative knowing." (Campbell, 1978, p.361)

"Conceiving quantitizing as unidirectional—as moving from so-called qualitative to quantitative data—masks the continuous cycling between assigning numbers to meaning and meaning to numbers." (p.5)

É a formalização do que o Foundations.md chama de ciclo infinito. Não é pipeline linear (quali → quanti → quali) — é ciclo constitutivo onde cada ato de quantitizar já envolve qualitizar e vice-versa.

### Contribuição 5 — Três standpoints que justificam quantitizar (p.3, conclusão)

| Standpoint | O que defende | Autores |
|---|---|---|
| **Conditional complementarity** | Métodos se complementam sob certas condições, não universalmente | Maynard & Schaeffer, 2000 |
| **Critical remediation** | Quantitizar pode "remediar" limitações do quali (revelar padrões invisíveis) | Love et al., 2005 |
| **Analytic alternation** | Alternar entre quali e quanti sistematicamente como estratégia | Hammersley, 2008 |

### Contribuição 6 — A pergunta que importa (p.10)

"Researchers must have a clear sense of why they want to quantitize at all. They must consider what the added value is of transforming qualitative into quantitative data: **whether and how qualitative data are enhanced by putting them into a form that allows the assignment of numerical values.**"

Frase final: "Numbers have tremendous rhetorical appeal, in part, because of their association with scientific precision and rigor. They substitute the simplification and security of numerical precision for the complication and ambiguity of narrative. **The issue is whether numerical precision can satisfactorily grab enough of the complexity of narrative both to understand and communicate it.**"

### Qualitização implícita

Ironicamente, o paper sobre quantitização é ele mesmo um ato de qualitização: pega conceitos numéricos (0/1, escalas, frequências) e os transforma em narrativa interpretativa sobre o que significam. O paper inteiro é qualitização da quantitização.

### Referências anteriores a investigar

| Obra | Autor | Ano | Por que importa |
|---|---|---|---|
| "Qualitative knowing in action research" | Donald Campbell | 1978 | O pai da validade admitindo que quanti depende do quali |
| "Transforming Qualitative Data" | Harry Wolcott | 1994 | "Nothing becomes data without intervention" — raiz anterior a T&T 1998 |
| Sobre contagem de cromossomos como ato social | Emily Martin | 2004 | Contar é "disciplinary technology" — não é neutro |
| Sobre perda de variância na dicotomização | Jacob Cohen | 1983 | Binarizar perde 1/3 a 2/3 da variância — custo formal |

### Posição na genealogia

Terceiro e último da trilogia Sandelowski:
- **2000:** Formaliza quantitização/qualitização, costura vocabulários, 7 design templates
- **2001:** Legitima números dentro do quali, destrói mitos, 4 armadilhas
- **2009:** **Desconstruí os pressupostos** — data-as-taken, contar é interpretativo, 1/0 é ambíguo, ciclo é constitutivo

A progressão: nomeou (2000) → legitimou (2001) → desconstruiu (2009). Cada paper é mais profundo que o anterior.

### Gaps identificados — contribuição original do nosso projeto

**5 gaps que o cruzamento dos papers revela e que Sandelowski et al. (2009) não cobrem:**

**1. O ciclo é epistemologicamente simétrico mas praticamente assimétrico (Nzabonimpa, 2018).** Sandelowski propõe simetria constitutiva. Nzabonimpa mostra que software, comunidade e documentação favorecem quantitização. A infraestrutura é enviesada. Mas isso não invalida o ciclo — refinamos: ciclo válido epistemologicamente, assimétrico na prática, com limites estruturais (said/semi-said/unsaid).

**2. A desconstrução para no input — não chega ao output.** Os 7 significados de present/absent desconstroem os dados. Mas quando esses dados ambíguos alimentam clustering/AC/MDS, o output (clusters, eixos, dimensões) herda a ambiguidade sem que ninguém a discuta. Nossa distinção espelho/janela opera aqui: o output reflete padrões do fenômeno ou padrões de como o pesquisador codificou? Sandelowski desconstruiu o 1/0 mas não desconstruiu o cluster que emerge do 1/0.

**3. Colinearidade como amplificador da ambiguidade.** Se dois códigos estão "present" num segmento por razões diferentes (um espontâneo, outro direcionado), a co-ocorrência é artefato. A ambiguidade do 1/0 se amplifica na co-ocorrência. Nenhum paper trata isso — é contribuição da discussão sobre Qualia Coding.

**4. A alternativa ordinal (not discernible → dominant) é proposta mas não operacionalizada.** Boyatzis dá os 5 tipos de scoring (incluindo intensidade). Sandelowski et al. propõem ordinal como alternativa ao binário. Mas ninguém mostra como fazer na prática com software de QDA. O Qualia Coding poderia ser o primeiro a implementar scoring ordinal por código como alternativa à binarização.

**5. Falta o paper prometido sobre qualitização.** "We plan to emphasize qualitizing in another article" (p.1). Até onde se sabe, esse artigo nunca foi publicado. A qualitização ficou sub-teorizada pela própria autora que propôs o ciclo. O Foundations.md pode ser o documento que faz essa teorização — usando os papers técnicos (Macia, Henry, Morin) como evidência empírica de qualitização na prática.

### Conexão com obsidian-qualia-coding

1. **Os 7 significados de present/absent** como tooltip/warning quando o pesquisador aplica código: "Marcar como presente pode significar 7 coisas diferentes — qual é o seu caso?"
2. **Scoring ordinal** como alternativa à binarização: em vez de 0/1, oferecer escala (não discernível → mencionado de passagem → importante → dominante)
3. **A pergunta "devo quantitizar?"** como prompt antes de rodar analytics: "Os dados qualitativos são enhanced pela atribuição de valores numéricos? O que você espera descobrir que a leitura qualitativa não revelaria?"

---

## 14. Onwuegbuzie, A. J. (2025). On Quantitizing Revisited

**Fonte:** Frontiers in Psychology, 15:1421525.
**Arquivo:** `./GTQQ/References/fpsyg-15-142152533.pdf`

| | |
|---|---|
| **Autor** | Anthony J. Onwuegbuzie |
| **Instituição** | Faculty of Education, University of Johannesburg |
| **País** | África do Sul (autor americano baseado em Joanesburgo) |
| **Ano** | 2025 (publicado 23 janeiro 2025) |
| **Journal** | Frontiers in Psychology (Methods) |
| **Setor/Contexto** | Metodologia — resposta formal ao Sandelowski et al. (2009), 16 anos depois |
| **Tipo** | Artigo fundacional — meta-framework completo pra quantitização (5W1H + DIME hierárquico). Estado da arte absoluto. O paper mais recente que lemos — publicado 5 meses antes de ser baixado pro projeto. |

### Resumo

Resposta formal do Onwuegbuzie ao "On Quantitizing" da Sandelowski et al. (2009), que acumulou 1000+ citações. Onde a Sandelowski desconstruiu (por que questionar), o Onwuegbuzie reconstrói (como fazer com rigor). Propõe meta-framework 5W1H (Why, What, When, Where, How, Who) e o modelo DIME hierárquico de 4 níveis. Mapeia a propensão de ~20 filosofias de pesquisa a quantitizar (Tables 1-3). Inclui busca sistemática da história do termo desde 1894 e análise do JMMR (55/346 artigos = 15.9% mencionam quantitizing). É o estado da arte do campo em janeiro 2025.

### Contribuição 1 — A história do termo "quantitizing" (pp.2-3)

Busca sistemática no Scopus revela que o termo é **muito mais antigo** do que a genealogia que construímos:

- **Allen (1894):** Prosódia latina — "a quantitizing Saturnian" (análise de métrica poética). Primeiro uso documentado.
- **Escudie et al. (1965):** Processamento de sinais — converter contínuo em discreto
- **Schippers et al. (1967):** Condutividade elétrica em solos — transformar observação qualitativa de umidade em medida
- **Miles & Huberman (1994):** Primeiro uso em ciências sociais (informal)
- **Tashakkori & Teddlie (1998):** Formalização do par quantitizing/qualitizing
- **Sandelowski (2001):** Primeiro artigo indexado no Scopus a usar o termo citando T&T
- **Onwuegbuzie (2003):** Primeira vez que o termo é usado em título de artigo indexado

A genealogia que construímos (Caracelli & Greene 1993 → Miles & Huberman 1994 → T&T 1998) é validada e estendida 100 anos pra trás. O conceito de transformar qualitativo em quantitativo é tão antigo quanto a análise de poesia latina.

### Contribuição 2 — Dado revelador sobre adoção (p.3)

De 346 artigos no JMMR (1997-2024), apenas **55 (15.9%)** mencionaram "quantitizing." Análise ARIMA mostra: sem tendência linear, quadrática, cúbica ou quártica na frequência ao longo do tempo. A publicação é aleatória com flutuações. A técnica é fundamental mas **não está crescendo** em adoção. Confirma o Nzabonimpa (2018) e reforça o argumento central do nosso projeto: a prática é disseminada (muitos fazem sem chamar assim) mas a denominação é sub-utilizada.

### Contribuição 3 — O framework 5W1H completo (pp.4-18)

**WHY — Por que quantitizar? (pp.4-6)**

6 razões formais, organizadas via Greene et al. (1989):
- **Complementaridade:** Elaborar, ilustrar, clarificar achados quali com quanti e vice-versa
- **Desenvolvimento:** Usar resultados da quantitização pra guiar próximas fases
- **Expansão:** Ampliar escopo usando múltiplas strands analíticas
- **Triangulação:** Comparar achados quantitizados com outros dados quanti pra validar
- **Iniciação:** Identificar paradoxos e contradições que reframing a questão de pesquisa

E a fórmula 1+1=1 (Onwuegbuzie, 2017): integração completa onde as strands são "so cleverly and iteratively interwoven that it becomes an exercise in semantics to disentangle the two" (Creamer, 2018, p.100). Quantitizar não é somar — é fundir.

**WHEN — Quando quantitizar e quando NÃO? (pp.6-7)**

Quantitizar quando: dependent research questions, emergent questions, overarching mixed methods questions, issue research questions, procedural/mixing questions.

Quando NÃO: "when the intent is merely to transform qualitative data into quantitative form without regard for the richness and complexity of the original data" — quando é simplificação sem valor agregado, quando força dados quali em frameworks quanti sem alinhamento. São os guardrails da Sandelowski (2009) operacionalizados como decisão de design de pesquisa.

**WHAT — O que pode ser quantitizado? (pp.7-8)**

Hierarquia de abstração do que pode ser quantitizado:

```
Code → Category → Sub-theme → Theme → Figure of speech → Meta-theme → Narrative
```

Cada nível tem forma diferente de quantitizar: codes por frequência, categories por proporção, themes por presença/ausência cross-dataset, figures of speech por contagem e tipo, narratives por breakdown em codes/themes/unidades. É o mapa do que o Qualia Coding manipula em cada nível do codebook.

**WHERE — Onde quantitizar? (p.8)**

Offline (entrevistas, observações, documentos) + online (redes sociais, reviews, posts, tweets). Big data de plataformas digitais é fronteira: volume permite quantitização exploratória que seria impossível com N pequeno. Mas com os mesmos riscos de colinearidade e ambiguidade do 1/0.

**HOW — Como quantitizar? O meta-modelo DIME de 4 níveis (pp.8-17)**

O DIME não é mais 4 tipos paralelos — é **modelo hierárquico** (Figure 4):

**Level 1 — DIME (fundação):**
- **D**escriptive: frequências, médias, dispersão, posição, forma distribucional (skewness, kurtosis)
- **I**nferential: GLM, t-test, ANOVA, MANOVA, correlação canônica, SEM, HLM — inferir pra população
- **M**easurement: Rasch, IRT (2, 3, 4 parâmetros) — desenvolver e validar instrumentos
- **E**xploratory: PCA, EFA, cluster analysis, correspondence analysis, MDS — descobrir padrões

**Level 2 — Dimensões adicionais:**
- **Spatial:** GIS, heat maps, distribuição geográfica de temas
- **Time:** Time series, event history, survival analysis

**Level 3 — Design temporal:**
- **Cross-sectional:** Snapshot num ponto do tempo
- **Longitudinal:** Ao longo do tempo (logistic regression for repeated measures, GLMM, mixed models)

**Level 4 — Orientação temporal:**
- **Retrospective:** Dados já existentes, quantitizados a posteriori
- **Prospective:** Coleta planejada desde o início pra quantitizar

Cada nível incorpora o anterior. Level 4 subsume Level 3, que subsume Level 2, que subsume Level 1.

**Figure 3 — 8 níveis de complexidade quantitativa (Ross & Onwuegbuzie, 2014):**
Continuum de complexidade crescente: Descriptive → Univariate → Multivariate → Group Membership (cluster, AC, MDS) → Measurement → Time/Space → Multi-Directional/Multilevel → Multi-Directional AND Multilevel.

Achado empírico: estudos existentes "predominantly employ only the first three levels." Quase ninguém vai até Group Membership (nível 4). **Todos os papers técnicos que documentamos (Macia, Henry, Morin) operam no nível 4** — que é raro na prática. O Qualia Coding oferece analytics de nível 4.

**WHO — Quem deveria quantitizar? (pp.17-18)**

Não é exclusivo de mixed methods researchers — qualitative researchers e quantitative researchers também se beneficiam. "Quantitizing is not confined to mixed methods research" (citando Sandelowski et al., 2009, p.210).

### Contribuição 4 — Tables 1-3: Propensão filosófica a quantitizar (pp.18-20)

Mapeamento de ~20 filosofias de pesquisa e sua propensão a quantitizar. Expande massivamente as 4 posições da Rodrigues (2007):

**Filosofias qualitativas mais propensas:** Critical theory, feminist theory — "if it serves critical insights and emancipatory goals." Feminist standpoint — "if it supports advocacy goals." Pragmatism — "highly compatible."

**Filosofias qualitativas menos propensas:** Social constructionism ("perceived as reducing richness"), radical constructivism ("rarely embraced — contradicts emphasis on individual subjective experiences"), symbolic interactionism, postmodernism ("highly skeptical of grand narratives and reduction to simple categories"), poststructuralism, phenomenology ("opposes the phenomenological commitment to capturing depth and nuance").

**Filosofias quantitativas mais propensas:** Platonism, formalism, logicism, objectivism, empiricism, postpositivism.

**Filosofias quantitativas menos propensas:** Intuitionism, psychologism, fictionalism, nominalism, anti-realism — "view mathematics as a mental construct."

### Contribuição 5 — O estudo RESPECTED como thread (pp.10, 14)

O Onwuegbuzie demonstra cada nível do DIME usando um único dataset (912 respostas sobre professores eficazes):
- **D:** 9 temas RESPECTED (Student-centered = 58.88%)
- **I:** Correlação canônica temas × demográficas — "only GPA did not appear to play a role" (p.140 do estudo original)
- **M:** Rasch analysis (proposta, não implementada no estudo original)
- **E:** PCA com correlações tetracóricas → 4 meta-temas nomeados CARE (Communicator 81%, Advocate, Responsible 41.1%, Empowering 59.6%)

A nomeação de CARE é **qualitização** — output de PCA nomeado como acrônimo significativo. Mais uma evidência da prática sem nome.

### Qualitização no paper

O Onwuegbuzie foca em quantitização (como o título indica) e diz explicitamente: "We plan to emphasize qualitizing in another article" — repetindo a promessa da Sandelowski (2009) que nunca se concretizou. O paper sobre qualitização continua sem ser escrito. É o gap #5 dos que identificamos.

Mas o paper está cheio de qualitização implícita: RESPECTED (9 temas nomeados), CARE (4 meta-temas nomeados), a nomeação dos 4 tipos DIME, a interpretação dos clusters no exemplo de mental health coping ("Holistic Copers," "Active Copers," "Passive Copers" — p.14). Todo ato de nomear output quantitativo é qualitização que o paper não reconhece como tal.

### Conexão com o Foundations.md

Este paper é a **atualização completa** do framework do Foundations.md:
- O DIME que o Foundations cita (seção 3.3) agora é modelo hierárquico de 4 níveis
- A genealogia que construímos (Caracelli & Greene 1993) agora vai até 1894
- O dado de 15.9% de menção no JMMR confirma a tese de sub-denominação
- As Tables 1-3 expandem as 4 posições da Rodrigues pra ~20 filosofias
- O achado de Ross & Onwuegbuzie sobre nível de complexidade na prática posiciona o Qualia Coding como ferramenta de nível 4 (raro)

### Conexão com obsidian-qualia-coding

1. **O plugin opera no nível 4 do DIME (Exploratory)** — cluster, AC, MDS. É o nível que a maioria dos pesquisadores não alcança. Isso é diferencial e responsabilidade: a ferramenta democratiza acesso a análises sofisticadas, mas precisa dos guardrails pra uso responsável
2. **A hierarquia What (code → category → theme → meta-theme → narrative)** é exatamente o que o codebook do plugin estrutura. Cada nível pode ser quantitizado de forma diferente
3. **O Level 4 (retrospective)** descreve exatamente o caso Sicredi: dados quali já existentes (repositório de insights) quantitizados a posteriori via ACM
4. **A fórmula 1+1=1** como princípio de design: os analytics não devem ser "camada quanti sobre dados quali" — devem ser integrados a ponto de serem indistinguíveis

### Nota temporal

Paper publicado em **23 janeiro 2025**, baixado pro projeto em **2 junho 2025** (5 meses depois). É o paper mais recente do corpus e provavelmente o mais atualizado framework de quantitização existente em janeiro 2025. O Foundations.md, sendo escrito em maio-junho 2025, é contemporâneo — o que significa que pode dialogar com esse paper no mesmo nível temporal, não retrospectivamente.

---

## 15. Onwuegbuzie, A. J. & Leech, N. L. (2021). Qualitizing Data (Cap 13)

**Fonte:** In A. J. Onwuegbuzie & R. B. Johnson (Eds.), *The Routledge Reviewer's Guide to Mixed Methods Analysis* (pp. 141-149). Routledge.
**Arquivo:** `./GTQQ/References/13.Qualitizing Data.pdf` (extração do Cap 13)
**Livro completo:** `./GTQQ/Anthony J. Onwuegbuzie, R. Burke Johnson - The Routledge Reviewer's Guide to Mixed Methods Analysis (2021, Routledge) - libgen.li.pdf`

| | |
|---|---|
| **Autores** | Anthony J. Onwuegbuzie, Nancy L. Leech |
| **Instituições** | University of Johannesburg; University of Colorado Denver |
| **País** | África do Sul / EUA |
| **Ano** | 2021 |
| **Editora** | Routledge |
| **Setor/Contexto** | Metodologia — capítulo dedicado à qualitização dentro do handbook de referência pra mixed methods analysis |
| **Tipo** | Capítulo de livro — **a sistematização mais completa de qualitização existente**. Preenche parcialmente o gap #5 (paper solo sobre qualitização nunca publicado). |

### Resumo

O capítulo sobre qualitização que a Sandelowski prometeu em 2009 e o Onwuegbuzie repetiu em 2025 — mas que nunca saiu como artigo solo. Existe como Cap 13 do Routledge Reviewer's Guide. Traz a definição expandida com 5 elementos, as fórmulas de integração explicadas, cluster analysis como ferramenta de qualitização (não de quantitização), demonstração empírica com 4.419 estudantes sul-africanos durante COVID-19, e o dado de que qualitizing é mencionado 2.3× menos que quantitizing no JMMR.

### Contribuição 1 — As fórmulas de integração explicadas (pp.141-143)

A progressão de fórmulas é a história conceitual dos métodos mistos em forma matemática. Cada uma representa um grau diferente de integração:

**1+1=2 (Low integration — "parallel")**
Você faz pesquisa qualitativa e pesquisa quantitativa sobre o mesmo tema, mas **separadas**. O relatório final tem uma seção quali e uma seção quanti, cada uma analisada com seus métodos nativos. Não se cruzam. Publicadas às vezes até separadamente. É o que a maioria dos estudos "mixed methods" faz na prática — dois estudos colados, não integrados. Exemplo: fazer entrevistas E survey sobre satisfação, reportar cada um em capítulo separado.

**1+1=3 (Medium integration — "partial")**
Os dois lados produzem algo que nenhum dos dois teria sozinho: **meta-inferências**. O "3" é o terceiro elemento que emerge do cruzamento. Você analisa o quali, analisa o quanti, e na interpretação cruza os achados — "a entrevista dizia X, o survey dizia Y, juntos revelam Z que nenhum dos dois via sozinho." É o que o Driscoll fez: survey disse 90% aprovam o processo, respostas abertas revelaram que 30% discordam das decisões. A contradição (Z) só apareceu no cruzamento.

**1+1=1 (Full integration — "fully integrated")**
As strands qualitativa e quantitativa são tão entrelaçadas **desde o início** que vira "exercício de semântica" separar uma da outra (Creamer, 2018, p.100). Não é "faço quali, depois faço quanti, depois cruzo." É: em cada momento do processo, quali e quanti estão operando juntos. A codificação já considera a análise estatística. A análise estatística já alimenta a volta ao texto. Exemplo: o pipeline Macia — codifica pensando na binarização, binariza pensando no retorno qualitativo, interpreta os clusters voltando às narrativas. Se alguém pergunta "essa parte é quali ou quanti?" a resposta é: não dá pra separar.

**ΣL^i + ΣN^j = 3 (Multi-mixed methods — medium integration)**
Agora com **múltiplas fontes**. L = número de fontes qualitativas (entrevistas, observações, documentos...), N = número de fontes quantitativas (surveys, escalas, dados transacionais...). Cada fonte pode ser analisada de várias formas. O "3" significa que as meta-inferências emergem mas as tradições permanecem distinguíveis. Exemplo: no Sicredi — field visits (L1) + avaliação heurística (L2) + análise documental (L3) + survey/escala (N1) + dados do repositório (N2) → territórios de experiência emergem do cruzamento, mas você ainda sabe qual achado veio de qual fonte.

**ΣL^i + ΣN^j = 1 (Meta-methods — full integration)**
Múltiplas fontes, totalmente integradas. Não só as strands são indistinguíveis — as próprias fontes se fundem. É o mais raro e ambicioso: começa com integração na concepção do estudo (não no final). O case COVID-19 (Ojo & Onwuegbuzie, 2020) exemplifica: Likert + open-ended + text mining + PCA + cluster analysis + sentiment analysis + chi-square + narrative profiles → tudo operando sobre tudo simultaneamente.

### Contribuição 2 — A definição expandida de qualitização com 5 elementos (p.143)

Onwuegbuzie & Leech (2019, p.122) — definição que supera "converter quanti em quali":

**Elemento 1 — Origem múltipla:** Pode operar sobre dados originalmente quantitativos OU sobre dados qualitativos que foram quantitizados. O ciclo completo de Sandelowski em ação: quali → quantitiza → qualitiza o output.

**Elemento 2 — Pluralidade analítica:** Pode envolver análises qualitativas E/OU **quantitativas**. Cluster analysis, AC, MDS, fatorial são **ferramentas de qualitização** — o clustering é o meio (quanti), a nomeação dos clusters é o fim (quali). Isso resolve um paradoxo: métodos quantitativos a serviço de fins qualitativos.

**Elemento 3 — Complexidade processual:**
- **Single qualitizing:** Uma operação sobre um dataset. Ex: pegar médias de Likert e criar perfil verbal ("moderadamente satisfeito").
- **Multi-qualitizing:** Múltiplas iterações. Ex: PCA → nomear fatores → cluster analysis dos fatores → nomear clusters → criar perfis narrativos dos clusters. Cada passo é uma qualitização sobre o output da anterior.
- **Fully Integrated Qualitizing (FIQ):** Dados quanti E quali, análises quanti E quali, tudo informando o processo.

**Elemento 4 — Integração completa:** Na forma mais integrada, adota 1+1=1.

**Elemento 5 — Multiplicidade representacional:** Pode gerar codes, categories, sub-themes, themes, figures of speech, meta-themes, e narrativas (prosa ou poesia). A escolha depende de: questão de pesquisa, design, tamanho da amostra, outlet pretendido, e audiência.

### Contribuição 3 — Clustering como ferramenta de QUALITIZAÇÃO (pp.144-147)

Ponto crucial que reconfigura como entendemos os papers técnicos: cluster analysis, AC, MDS, fatorial **não são ferramentas de quantitização quando usadas pra qualitizar**. São ferramentas de qualitização quando o output é interpretação qualitativa.

Demonstração empírica — Ojo & Onwuegbuzie (2020), 4.419 estudantes Wits University, COVID-19:
1. Text mining (VOSviewer) das respostas abertas → 6 co-word clusters → 6 metathemes (**qualitização** do text mining)
2. Sentiment analysis dos metathemes → positivo=1, negativo=0 (**quantitização**)
3. Twostep cluster analysis → 4 attitudinal clusters (**quantitização** exploratória)
4. Chi-square dos 4 clusters × demográficas + experiências (**crossover** analysis)
5. **Comparative narrative profiles** dos 4 clusters baseados em AMBOS quanti e quali (**qualitização** final)

Table 13.1 é **crossover display** — metathemes à esquerda, achados estatísticos à direita. Materialização visual da fórmula 1+1=1.

O ciclo no case: texto (quali) → text mining (quanti) → metathemes (quali) → sentiment (quanti) → clusters (quanti) → chi-square (quanti) → narrative profiles (quali). Cinco cruzamentos. É multi-qualitizing em ação.

### Contribuição 4 — O dado da assimetria (p.148)

Do JMMR (2007-2019):
- **145 artigos empíricos:** 10 (6.9%) mencionam qualitize/qualitizing
- **95 artigos teórico-metodológicos:** 10 (10.5%) mencionam

Compare com Onwuegbuzie (2025): 55/346 (15.9%) mencionam quantitize/quantitizing no JMMR (1997-2024).

**Quantitizing é mencionado 2.3× mais que qualitizing** no principal journal de mixed methods. É a evidência mais forte da assimetria que o Nzabonimpa documentou — agora com números.

### Contribuição 5 — 5 goals de qualitização (via Greene et al., 1989)

| Goal | O que faz na qualitização |
|---|---|
| **Complementaridade** | Elaborar, ilustrar achados quali com resultados da qualitização |
| **Triangulação** | Comparar dados qualitizados com achados quali de outras fontes |
| **Iniciação** | Descobrir paradoxos e contradições entre qualitizado e quali |
| **Desenvolvimento** | Usar qualitização pra informar próximas fases (quali ou quanti) |
| **Expansão** | Ampliar escopo usando qualitização em múltiplas strands |

### Contribuição 6 — Sugestões criativas e poesia (pp.148-149)

Onwuegbuzie encoraja: "be as creative as possible in their qualitizing representations." Sugere uso de **poesia** — ABC Poem, Acrostic, Bio Poem, Haiku, Sonnet, Villanelle — e **crossover displays** + **joint displays** como formas visuais. Poesia como qualitização é o extremo mais criativo: transformar output estatístico em forma literária. Raro, provocativo, mas metodologicamente legítimo.

### Qualitização explícita e meta

O capítulo inteiro é sobre qualitização — é o primeiro texto dedicado exclusivamente ao tema. Mas ironicamente confirma o gap: existe como capítulo de livro (2021), não como artigo solo. "We encourage authors of mixed methods research books to provide a richer discussion of the topic of qualitizing in their books" (p.148). O gap #5 continua: o paper solo sobre qualitização permanece não-publicado.

### O que isso muda pra nossa análise

1. **Cluster analysis como ferramenta de qualitização resolve o paradoxo espelho/janela:** O dendrograma do Qualia Coding não é quantitização — é ferramenta pra qualitização. O output estatístico (clusters) é meio; o fim é interpretação qualitativa (nomes, perfis, retorno ao texto). A distinção espelho/janela se reconfigura: R-analysis é meta-análise do codebook pra refinar (ferramenta de qualitização do codebook); Q-analysis é exploração do fenômeno pra gerar tipologias (ferramenta de qualitização dos participantes).

2. **Multi-qualitizing é o que o Qualia Coding deveria facilitar:** Não uma operação, mas um pipeline iterativo: co-ocorrência → dendrograma → nomear clusters → MDS → nomear dimensões → voltar ao texto. Cada passo é qualitização sobre o anterior.

3. **O dado 6.9% vs. 15.9%** é argumento quantitativo pro Foundations.md: a qualitização é 2.3× menos mencionada, confirmando que o lado quali do ciclo é sub-teorizado e sub-praticado.

### Sobre o livro completo (Routledge Reviewer's Guide)

O livro tem capítulos sobre cada método exploratório aplicado a dados qualitativos quantitizados — EFA (Cap 2), AC (Cap 3), MDS (Cap 4), Cluster (Cap 5), CHAID (Cap 6), Multiple Regression (Cap 7), SEM (Cap 8), HLM (Cap 9), entre outros. É basicamente o **manual operacional** do DIME do Onwuegbuzie (2025), publicado 4 anos antes. Cada capítulo do livro é o detalhe técnico de um nível do DIME.

---

## 16. Saldaña, J. (2021). Coding Techniques for Quantitative and Mixed Data (Cap 14)

**Fonte:** In A. J. Onwuegbuzie & R. B. Johnson (Eds.), *The Routledge Reviewer's Guide to Mixed Methods Analysis* (pp. 151-160). Routledge.
**Arquivo:** `./GTQQ/References/2- Coding Techniques for Quantitative and Mixed Data.pdf`

| | |
|---|---|
| **Autor** | Johnny Saldaña |
| **Instituição** | Arizona State University (Professor Emeritus) |
| **País** | EUA |
| **Ano** | 2021 |
| **Editora** | Routledge |
| **Setor/Contexto** | Metodologia — técnicas de codificação qualitativa aplicadas a dados quantitativos e mistos |
| **Tipo** | Capítulo de livro — how-to operacional da qualitização via codificação. Complemento prático do Cap 13 (Onwuegbuzie & Leech). |

### Resumo

Enquanto o Cap 13 (Onwuegbuzie & Leech) dá a definição expandida e o framework de qualitização, o Saldaña dá as **técnicas concretas com exemplos**. Demonstra como aplicar 10 técnicas de codificação qualitativa a dados quantitativos (estatísticas de COPD, dados de violência armada, survey sobre teatro). Inclui o Magnitude Coding system expandido (a alternativa ordinal que Sandelowski 2009 propôs mas não operacionalizou) e dois case studies empíricos de multi-qualitizing.

### A fórmula da qualitização (p.151)

`How Much / Many → What Kind / Quality`

Seis palavras que capturam a essência: qualitizar é transformar "quanto" em "que tipo."

### 4 razões pra qualitizar (pp.151-152)

1. **Concordância/corroboração paradigmática:** Reality check — quali e quanti "look alike" e "feel alike" quando combinados? (Lincoln & Guba, 1985, p.347)
2. **Integração:** Qualitizados, dados quanti podem "talk to one another" com dados quali "in a compatible, mediated language"
3. **Indexação e classificação:** Magnitude Codes criam categorias narrativas sobre distribuições
4. **Meta-inferência:** Articular "not just the statistical properties but the qualitative nuances interpreted from a quantitative data set"

### 10 técnicas de codificação aplicadas a dados quanti (pp.152-155)

Cada técnica demonstrada com mesmo dataset (estatísticas de COPD da CDC):

| Técnica | O que faz | Exemplo | Tipo |
|---|---|---|---|
| **Process Coding** | Gerúndio que connota ação | "LIVING WITH WORRY" | Organizacional |
| **Descriptive Coding** | Substantivo que sumariza tópico | "SMOKING OUTCOME" | Organizacional |
| **Structural Coding** | Frase conceitual ligada à questão de pesquisa | "CAUSES OF DEATH" | Organizacional |
| **Magnitude Coding** | Tag suplementar de intensidade/avaliação | "RELATIVE PREVALENCE: MODERATE" | Inferencial |
| **Evaluation Coding** | Julgamento de mérito com recomendação | "±TV-PSA CAMPAIGN; REC: ENCOURAGE TESTING" | Inferencial |
| **Emotion Coding** | Emoção inferida ou declarada | "DISTRESSING" | Afetivo |
| **Metaphor Coding** | Comparação/imagem evocativa | "DEADLY VIRUS", "A HOUSE ON FIRE" | Afetivo |
| **Values Coding** | V=valor, A=atitude, B=crença | V: "TRAGIC LOSS", A: "DISTURBING TREND", B: "NOT SURPRISING" | Afetivo |
| **In Vivo Coding** | Palavras dos próprios participantes | "ON-TARGET", "I AGREE", "THIS VALIDATES" | Participativo |
| **Causation Coding** | Triplet antecedente→mediador→resultado | COMPETITION → WINNING → SELF-ESTEEM | Relacional |

Nota: as técnicas se dividem em 3 tipos — **organizacionais** (estruturam), **inferenciais** (interpretam), **afetivas** (capturam emoção/valor). É uma taxonomia funcional das técnicas de qualitização.

### Magnitude Coding system expandido (p.153)

A **alternativa ordinal** que Sandelowski (2009) propôs ("not discernible → dominant") mas não operacionalizou. Saldaña dá o vocabulário concreto:

| Dimensão | Escala |
|---|---|
| **Quantidades** | MINOR / MODERATE / MAJOR; NIL / UNCERTAIN / LOW / HIGH |
| **Qualidades** | POOR / MODERATE / GOOD; WEAK / ADEQUATE / STRONG |
| **Mudança** | DROPPED / REVISED / ADDED; NOT PERTINENT / PERTINENT / IMPORTANT |
| **Efeitos** | NEGATIVE / POSITIVE; NO IMPACT / SOME IMPACT / HIGH IMPACT |

Aplicável tanto a dados QUAL quanto QUAN — é o sistema de scoring ordinal que o Boyatzis (tipo e, intensidade) e a Sandelowski (alternativa ao binário) descrevem teoricamente, agora com vocabulário implementável. Pro Qualia Coding: cada código poderia ter um Magnitude Code anexo selecionável de uma lista pré-definida.

### Case Leal et al. (2018) — multi-qualitizing de perfis individuais (pp.155-156)

Yoga tibetana + linfoma. 4 medições longitudinais de scores psicológicos por paciente. Cada paciente teve seu **variation pattern** qualitizado:

| Paciente | Padrão | Tema qualitizado | Códigos quali |
|---|---|---|---|
| #102 | Minimum variation | CONSISTENCY (Extremely stable) | EQUILIBRIUM, DOUBT, INCONGRUOUS |
| #38 | Maximum variation | TRANSFORMATION (Marked positive) | GROWING, TAINTED, LOSS/OUT OF CONTROL |
| #63 | Congruent, little variation | MODERATE (Slight positive) | ACCEPTANCE, FUNDAMENTALLY TRANSFORMATIVE |
| #19 | Incongruent, internal contradiction | CONFLICT (Both positive and negative) | POSITIVE, SHIFTING PRIORITIES, INCONGRUOUS |

É **qualitização de perfis individuais** — cada paciente vira caso com tema qualitizado do seu padrão quantitativo. Perfil Comparativo de Tashakkori elevado ao nível de retrato individual.

### "So what?" codes e analytic memos (pp.157-158)

Após cada teste estatístico, o pesquisador cria um "so what?" code — qualitização imediata:
- Mean 3.82/4.00 → "HIGH!-LIFELONG AFFECTS" (interpretação)
- p < .64, sem diferença de gênero → "THIS CAN'T BE RIGHT" (reação honesta)
- Confirmação quali sem diferença → "PATTERN: NO GENDER DIFFERENCES" (consolidação)

Os "so what?" codes são seguidos de **analytic memos** — reflexões pessoais do pesquisador. É qualitização como **prática reflexiva**. O memo é "permissibly messy" — é pra pesquisador, não pra publicação.

O Saldaña lista **16 prompts pra analytic memos** após qualitização, incluindo o #16 específico pra mixed methods: "how qualitized codes/themes interrelate (i.e., congruency, divergence, contradiction, explanation) with qualitative codes/themes."

### Diferença codes vs. themes (p.155)

Distinção prática: "a code is a word or short phrase; a theme is an extended phrase or sentence." Aside from length, "a theme identifies what a unit of data is about and/or what it means." Codes são sobre o que é (indexação). Themes são sobre o que significa (interpretação). Ambos podem ser qualitizados, mas themes são qualitização de nível superior.

### Excel como "playground" (p.157)

"The Excel spread sheet was a playground for inductive queries because the software quickly enabled various configurations of data arrays. Numbers and narratives were always kept close together." A proximidade visual entre número e narrativa é **feature de design**, não acidente.

### Conexão com obsidian-qualia-coding

**O CSV grid do Qualia Coding já implementa o "playground" do Saldaña** — e vai além:
- Grid com linhas (casos/registros) e colunas (variáveis + códigos como tags coloridas)
- Detail sidebar mostrando código no contexto com metadados
- Batch coding (263 linhas no print) — operação em escala
- Column Settings configuráveis por questão de pesquisa

É o Excel do Saldaña industrializado dentro do Obsidian: dados tabulares (quanti/categóricos) lado a lado com códigos qualitativos, tudo na mesma view. O pesquisador vê número e narrativa juntos.

**Extensões possíveis pro plugin:**
1. **Magnitude Codes** como tags suplementares selecionáveis de lista pré-definida (MINOR/MODERATE/MAJOR etc.)
2. **"So what?" prompts** automáticos após rodar analytics — "O que esse resultado significa pra sua questão de pesquisa?"
3. **Analytic memos** vinculados a output de analytics (dendrograma gerou memo, cluster gerou memo)
4. **Causation Coding** como tipo de código com 3 campos (antecedente, mediador, resultado)

### Qualitização explícita

O capítulo inteiro é sobre qualitizar — cada técnica é demonstrada aplicando códigos qualitativos a dados quantitativos. Saldaña é o autor que mais operacionaliza a qualitização na prática (vs. Onwuegbuzie que dá framework, vs. Sandelowski que desconstroí).

Frase-chave (p.160): "Whether the qualitized choice is straightforwardly descriptive, evocatively metaphoric, or unabashedly values-laden is the analyst's judgment call." A qualitização é ato de julgamento — não tem "resposta certa." É arte, como Hathcoat & Meixner (2015) e o Nzabonimpa (2018) dizem.

---

## 17. Suerdem, A. (2021). Multidimensional Scaling of Qualitative Data (Cap 4)

**Fonte:** In A. J. Onwuegbuzie & R. B. Johnson (Eds.), *The Routledge Reviewer's Guide to Mixed Methods Analysis* (pp. 45-56). Routledge.
**Arquivo:** `./GTQQ/6- Multi Dimentional Scale.pdf`

| | |
|---|---|
| **Autor** | Ahmet Suerdem |
| **Instituição** | Istanbul Bilgi University (inferido do Routledge handbook) |
| **País** | Turquia |
| **Ano** | 2021 |
| **Editora** | Routledge |
| **Setor/Contexto** | Metodologia — MDS aplicado especificamente a dados qualitativos, com fundamentação hermenêutica |
| **Tipo** | Capítulo de livro — complementa Jaworska (2009) com perspectiva filosófica |

### Resumo

Capítulo do mesmo handbook Routledge (Caps 13 e 14 já documentados). Onde a Jaworska (2009) trata MDS como técnica estatística, o Suerdem trata como **ferramenta de hermenêutica visual** — posicionamento filosófico único entre todos os papers que lemos.

### Contribuição principal — MDS como hermenêutica visual (pp.46-47)

O argumento: codificar dados qualitativos é um **processo hermenêutico circular** — ler → codificar → reinterpretar → recodificar. Esse ciclo pode gerar "enormous cognitive overload, leading the coder to be lost in circles if the internal and external boundaries of the corpus are not clearly framed" (citando Miles & Huberman, 1994).

MDS **fecha o círculo**: "Statistical dimension reduction techniques such as MDS can help us to close this hermeneutical circle by providing access to code patterns and to discover their underlying dimensions." O pesquisador vê a estrutura emergente do codebook e pode ajustar — não está mais preso no loop de codificação sem visão do todo.

Conecta com o conceito de **semiosis** (Peirce, via Eco 1987): MDS como parte de um processo abdutivo de construção de um **code model** — "a system made of signs, meanings, and coding rules." O pesquisador "makes inferences about the world of the text by grounding the expressions to his/her preconceptions to generate a conjectural interpretation. A theory helps to explain this interpretation by outlining the rules holding the text together." MDS é a ferramenta que revela as regras — as dimensões latentes que organizam como o pesquisador codificou (e, por extensão, como o fenômeno se estrutura).

"It is appropriate and useful to use MDS in the quantitative analysis of qualitative data unless it is used together with hermeneutical reading and understanding through an abductive process." MDS sem hermenêutica é número sem sentido. Hermenêutica sem MDS é interpretação sem mapa.

### Conexão com a distinção espelho/janela

O Suerdem articula implicitamente o que discutimos: MDS mostra as **dimensões latentes do codebook** — que podem ser dimensões do fenômeno (janela) ou dimensões de como o pesquisador pensa (espelho). A hermenêutica visual é justamente o processo de **discernir** qual é qual: o pesquisador olha o mapa MDS e se pergunta "essa dimensão é do meu objeto ou do meu olhar?"

O círculo hermenêutico é o mecanismo de calibração: ler → codificar → ver MDS → reinterpretar → recodificar → ver MDS de novo. A cada iteração, o espelho se torna mais janela — se o pesquisador está atento.

### Detalhes técnicos complementares à Jaworska

- Medidas de proximidade pra dados qualitativos: **Jaccard** (binário — o que o Qualia Coding usa), **Cramer's V** (nominal), **Euclidean** (numérico)
- Software QDA (QDA Miner, WordStat) já exporta matrizes de proximidade pra MDS
- R: pacote SMACOF (Mair, De Leeuw & Groenen, 2015) pra aplicações avançadas
- Shiny app interativo disponível: asuerdem.shinyapps.io/MDS-master/
- Case empírico: 15 termos de parentesco (Rosenberg & Park Kim, 1975) — dissimilaridade percebida entre termos familiares

### Conexão com obsidian-qualia-coding

O Qualia Coding já implementa MDS com Jaccard (R-analysis). O que o Suerdem adiciona é o **enquadramento**: o MDS do plugin não é "analytics quantitativo" — é **hermenêutica visual assistida**. O pesquisador usa o mapa pra ver o codebook de cima, identificar dimensões latentes, e decidir se precisa recodificar. É ferramenta do **passo 4 do Boyatzis** (interpretar padrões) via abdução semiótica.

A sugestão de iteração (MDS → recodificar → MDS de novo) poderia ser feature: "Codebook evolution" — mostrar como o mapa MDS muda entre rounds de codificação. Se as dimensões se estabilizam, o codebook amadureceu.

---

## 18. Péladeau, N. (2021). Cluster Analysis for Mixed Methods Research (Cap 5)

**Fonte:** In A. J. Onwuegbuzie & R. B. Johnson (Eds.), *The Routledge Reviewer's Guide to Mixed Methods Analysis* (pp. 57-67). Routledge.
**Arquivo:** `./GTQQ/5 - Cluster Analysis for Mixed Methods Research.pdf`

| | |
|---|---|
| **Autor** | Normand Péladeau |
| **Instituição** | Provalis Research (criador do QDA Miner e WordStat) |
| **País** | Canadá |
| **Ano** | 2021 |
| **Editora** | Routledge |
| **Setor/Contexto** | Metodologia / Software QDA — capítulo técnico sobre cluster analysis pra mixed methods, por quem faz software de QDA |
| **Tipo** | Capítulo de livro — o mais técnico sobre clustering que temos. Autor é desenvolvedor de ferramenta QDA, não só acadêmico. |

### Resumo

Capítulo escrito pelo criador do QDA Miner — ou seja, alguém que pensa clustering tanto como método quanto como feature de software. É o capítulo mais técnico do Routledge handbook pra nosso foco: traz a terminologia formal R-mode/Q-mode, dois exemplos empíricos lado a lado, alertas sobre armadilhas técnicas (MDS+clustering, número de clusters), e aplicações não-óbvias (clustering pra amostragem). Cita diretamente Macia (2015) e Henry et al. (2015).

### Contribuição 1 — R-mode vs. Q-mode com terminologia formal (p.58)

Péladeau é o primeiro que lemos a usar explicitamente os termos dentro do contexto de mixed methods:

"In the former situation, we talk about a **Q-mode analysis**, while clustering variables, like a typical factor analysis, is an **R-mode analysis**. An example of a Q-mode clustering would be to collect qualitative and quantitative data on numerous participants, compare them on several of those variables, and cluster them into homogenous groups of participants based on how similar they are on those. Alternatively, an R-mode clustering would compare the distribution of variables (or attributes) across participants to create groupings of variables."

É a formalização da distinção espelho/janela que construímos:
- **Q-mode** (janela) = agrupar participantes por perfil → Macia, Henry
- **R-mode** (espelho) = agrupar variáveis/códigos por co-ocorrência → Qualia Coding hoje

### Contribuição 2 — Clustering como ferramenta de amostragem (Example 1, pp.62-63)

Uso que nenhum outro paper discutiu: 239 respondentes de survey, 5 perguntas abertas codificadas → 62 variáveis numéricas por participante → clustering hierárquico em 20 clusters → silhouette = 0.296 → **selecionar 1 participante por cluster** pro follow-up qualitativo (entrevista em profundidade).

O critério de seleção: o participante com **maior silhouette score** dentro de cada cluster — o mais representativo, o mais "típico" do grupo. Resultado: 20 participantes que representam a máxima diversidade de perfis, não uma amostra aleatória.

É clustering como **ferramenta de design de pesquisa**, não de análise. Conecta com o template #7 da Sandelowski 2000 (Quan>Qual>Quan): survey (quanti) → clustering (quanti) → seleção de participantes → entrevista (quali). O clustering opera como ponte entre fases.

### Contribuição 3 — Example 2: R-mode com concept mapping (pp.63-64)

81 afirmações sobre alfabetização em pesquisa. 8 participantes fizeram card sorting → co-ocorrência (quantas vezes dois itens caíram na mesma pilha) → Jaccard → dendrograma hierárquico com weighted average linkage → 15 clusters.

Figure 5.5: dendrograma de 81 statements com Jaccard. Figure 5.6: silhouette index por número de clusters (4-25). Figure 5.7: número de itens misclassificados por número de clusters.

Decisão do número de clusters: todas as soluções têm silhouette > 0.5 (bom). Mas soluções com 14 ou menos clusters têm mais itens misclassificados. Soluções com 15+ têm zero ou poucos. Escolheu 15 — "the objective of achieving a more parsimonious concept extraction justifies choosing a 15-cluster solution."

É **exatamente** o que o Qualia Coding faz: R-analysis, Jaccard, dendrograma, silhouette. O capítulo valida a implementação do plugin.

### Contribuição 4 — Alerta: NÃO clusterize output de MDS (p.58)

"One might be tempted to apply multidimensional scaling, a technique that transforms similarity measures into Euclidian distances, and then cluster those to provide a visual representation of the obtained clusters. However, such an approach can be very problematic and often results in cluster solutions that are **suboptimal** compared to the clustering on the original similarity measures."

Guardrail técnico direto: clusterize na **matriz de similaridade original** (Jaccard, Dice, etc.), não nas coordenadas do MDS. O MDS transforma similaridades em distâncias euclidianas, e essa transformação pode distorcer a estrutura original. O dendrograma e o MDS devem operar **em paralelo** sobre o mesmo dado, não em cascata.

Pro Qualia Coding: o plugin faz certo (dendrograma e MDS partem ambos da co-ocorrência Jaccard). Mas se alguém quisesse "clusterizar o mapa MDS" — não. O alerta deveria estar na documentação.

### Contribuição 5 — Clustering como pré-codificação de texto (p.66)

"A preliminary hierarchical cluster analysis of word co-occurrence could very well represent an efficient way for a qualitative researcher to obtain a broad overview of the various topics that will be encountered during the analysis. It could even **suggest a codebook structure** that will accommodate the variety of themes that will be encountered."

Clustering de palavras (bag-of-words → co-ocorrência → hierárquico) pode **sugerir o codebook** antes da codificação manual. É o pipeline pré-codificação que a Morin (2006) demonstra com AC, e que o Suerdem (Cap 4, MDS) descreve como hermenêutica visual. Péladeau confirma que clustering também serve pra isso — é o terceiro método exploratório (com AC e MDS) que pode operar antes do codebook existir.

"Based on such a property, a preliminary hierarchical cluster analysis of word co-occurrence could very well represent an efficient way for a qualitative researcher to obtain a broad overview of the various topics... We could also use the same approach to **sample documents** when the number of text sources is too high to be analyzed qualitatively."

### Contribuição 6 — Fuzzy clustering como alternativa (p.66)

"Some **fuzzy clustering** techniques do exist, allowing objects to belong to more than one cluster, those forms are not widely available in computer applications. Other multivariate techniques such as principal component analysis or factor analysis might thus be more appropriate."

Reconhece a limitação central do clustering que discutimos (força cada caso num grupo, não lida com politematicidade) e aponta fuzzy clustering como alternativa teórica — mas admite que não é amplamente disponível. A AC (Morin) e o MDS (Jaworska/Suerdem) são alternativas mais acessíveis pra quem precisa de posicionamento contínuo.

### Contribuição 7 — Medidas de similaridade pra dados qualitativos (p.59)

Detalhamento técnico das medidas, com fórmulas e quando usar cada uma:

| Medida | Fórmula | Quando usar | Trata ausências |
|---|---|---|---|
| **Jaccard** | a/(a+b+c) | Dados binários onde ausência compartilhada não é informativa | Ignora co-ausência (d) |
| **Dice/Sørensen** | 2a/(2a+b+c) | Similar ao Jaccard, mais peso pra co-presença | Ignora co-ausência |
| **Simple matching** | (a+d)/(a+b+c+d) | Quando co-ausência é informativa (ex: gene ausente em duas doenças) | Considera co-ausência |
| **Pearson correlation** | — | Dados contínuos, perfis de variação | Sensível ao padrão, não ao nível |
| **Intraclass correlation** | — | Quando nível E padrão importam | Sensível a ambos |

Onde a=co-presença, b=presente em 1 mas não em 2, c=presente em 2 mas não em 1, d=co-ausência.

O Qualia Coding usa Jaccard — validado por Péladeau como escolha correta pra dados de codificação qualitativa onde "the potential number of attributes is large and their probability of occurrence is low" (p.59). É a J-curve do Boyatzis confirmada: com muitos códigos possíveis e baixa frequência, co-ausência não é informativa.

### Qualitização implícita

O capítulo tem dois atos de qualitização:
- **Example 1:** Os 20 clusters de participantes recebem representantes "arquetípicos" — o participante mais típico é selecionado como **exemplar** do grupo. É qualitização por exemplificação (não por nomeação).
- **Example 2:** Os 15 clusters de afirmações formam **conceitos** nomeáveis — o dendrograma é cortado e cada cluster vira um conceito no concept map. É qualitização por categorização (similar à Macia).

A citação de Guest & McLellan (2003, p.98): "cluster analysis can help frame thematic analysis and interpretation" — clustering é **meio** pra análise temática, não fim em si.

### Conexão com obsidian-qualia-coding

1. **O plugin já implementa corretamente** o que o Péladeau descreve no Example 2: R-mode, Jaccard, dendrograma, silhouette. Validação direta pelo criador do QDA Miner.
2. **Q-mode (Example 1) é o que falta**: transpor pra caso × código e clusterizar participantes. O Péladeau mostra que serve inclusive pra amostragem, não só pra análise.
3. **Não clusterizar output de MDS** — confirmar que o plugin faz certo (paralelo, não cascata).
4. **Clustering pra sugerir codebook** — feature de pré-codificação que complementaria a AC/MDS como exploração inicial.

---

## 19. Dickinson, W. B. (2021). Correspondence Analysis of Qualitative Data (Cap 3)

**Fonte:** In A. J. Onwuegbuzie & R. B. Johnson (Eds.), *The Routledge Reviewer's Guide to Mixed Methods Analysis* (pp. 37-42). Routledge.
**Arquivo:** `./GTQQ/4 - Correspondence Analysis of Qualitative Data.pdf`

| | |
|---|---|
| **Autora** | Wendy B. Dickinson |
| **Instituição** | University of South Florida (inferido das referências) |
| **País** | EUA |
| **Ano** | 2021 |
| **Editora** | Routledge |
| **Setor/Contexto** | Metodologia / Educação — CA aplicada a dados qualitativos em mixed methods, com foco em visualização e display |
| **Tipo** | Capítulo de livro — complementa Morin (2006) com perspectiva de visualização e posicionamento trans-paradigmático |

### Resumo

Capítulo do Routledge handbook (o quinto que documentamos desse livro) sobre Correspondence Analysis aplicada a dados qualitativos. Onde a Morin (2006) foca no método aplicado a text mining, a Dickinson foca em **por que visualizar** e **o que o mapa CA revela** que outros métodos não revelam. A contribuição central é posicionar CA como método que coloca linhas E colunas no mesmo mapa (biplot) — algo que clustering e MDS não fazem — e como ponte trans-paradigmática que opera pré-linguisticamente.

### Contribuição 1 — O biplot: temas E participantes no mesmo mapa (p.38)

Citando Onwuegbuzie et al. (2011), CA aplicada a dados qualitativos cumpre **três objetivos** simultâneos:

1. Mapear relações **entre temas** (como na R-analysis do clustering)
2. Mapear relações **entre participantes** (como na Q-analysis do clustering)
3. Mapear relações **entre temas e participantes** simultaneamente

O terceiro objetivo é o diferencial da CA: o **biplot** coloca linhas (participantes/documentos) E colunas (códigos/temas) no mesmo espaço bidimensional. Proximidade entre um participante e um tema significa associação. Nenhum outro método que documentamos faz isso:

| Método | O que posiciona no mapa | Biplot? |
|---|---|---|
| **Clustering** | OU casos OU códigos (R ou Q mode) | Não — escolhe um |
| **MDS** | OU casos OU códigos | Não — escolhe um |
| **AC/CA** | **Casos E códigos juntos** | Sim — biplot |

Isso significa que a CA responde uma pergunta que os outros não respondem: **"quais participantes estão mais associados a quais temas?"** Não "quais temas andam juntos" (R-mode) nem "quais participantes se parecem" (Q-mode), mas a relação **cruzada** entre os dois.

### Contribuição 2 — CA como ponte trans-paradigmática (p.39)

Citando Wainer & Friendly (2018, p.62): "Graphical representation cuts across artificial boundaries of natural language, and across disciplinary boundaries 'to capture phenomena as diverse as the pulse of a heart and the downturn of an economy.'"

O argumento: a visualização opera em nível **pré-paradigmático**. Enquanto palavras e números carregam bagagem epistemológica (palavras são quali, números são quanti), formas visuais comunicam **atravessando** fronteiras. O mesmo mapa CA pode ser lido por:
- **Positivista:** como representação objetiva de distâncias estatísticas entre categorias
- **Construtivista:** como construção interpretativa de relações entre experiências
- **Pragmatista:** como ferramenta útil que revela padrões

A visualização não resolve diferenças paradigmáticas, mas cria espaço comunicativo onde elas podem coexistir. É o argumento do Suerdem (MDS como hermenêutica visual) estendido pra CA — e mais radical: não é só ferramenta interpretativa do pesquisador, é **ferramenta de comunicação** entre pesquisadores de tradições diferentes.

Isso conecta com o Foundations.md (seção 1.2): Sandelowski (2000, p.247) dizia que combinações no nível paradigmático "não são verdadeiras combinações." A CA sugere que visualização pode ser o nível onde a combinação **acontece** — porque opera antes da linguagem e do paradigma.

### Contribuição 3 — John Snow (1854) como mixed methods avant la lettre (p.40)

Snow combinou contagens de mortalidade (quanti) com entrevistas familiares (quali) e mapeamento espacial (proto-CA visual) pra resolver o surto de cólera em Londres. Wainer (1997): de 10 famílias entrevistadas, 5 percorriam distâncias maiores até a bomba da Broad Street porque "preferiam o sabor daquela água."

"By combining all these methods of inquiry—quantitative mortality counts, and qualitative data obtained from oral accounts—Snow solved a multivariate, complex problem."

É a mesma referência que abre o Foundations.md (seção 1.1, citando Dickinson 2021 e Wainer 1997). O caso Snow é: dados de registro (quanti) + entrevista de campo (quali) + visualização espacial (proto-CA) = integração que nenhum método sozinho alcançaria. É o template #6 de Sandelowski (Qual>Quan>Qual) em 1854.

### Contribuição 4 — Três critérios de design visual (Wainer 2005, via Playfair 1786 e Tukey 1977) (p.39)

| Critério | O que significa | Implicação pro Qualia Coding |
|---|---|---|
| **Impact** | A primeira impressão — o "wow factor" do gráfico. "A powerful, and sometimes life-changing message." | Dendrograma, MDS, CA devem causar impacto visual imediato — o pesquisador olha e vê a estrutura |
| **Understanding is not automatic** | Clareza importa — gráfico obscuro perde valor. "If the message is hidden or obscured, the narrative value of the image plummets." | Labels, cores, tooltips — a visualização precisa ser auto-explicativa |
| **A graph can tell us things not seen otherwise** | O gráfico revela o que números escondem. "A graph can tell us things that might not have been seen otherwise." | É a justificativa de existência dos analytics: mostrar o que a leitura manual não mostra |

Esses 3 critérios são **princípios de design** pra qualquer visualização no plugin — não só CA, mas dendrograma, MDS, co-ocorrência heatmap, tudo.

### Contribuição 5 — Case Parents in Prison (Figure 3.1, p.40)

MCA aplicada a dados de censo prisional (Survey of Inmates in State and Federal Correctional Facilities, 2004): gênero do preso cruzado com tipo de cuidador dos filhos menores.

O mapa CA mostra em um gráfico o que narrativas não capturam tão imediatamente:
- **Pais presos (male)** → filhos com a mãe (otherparent). Próximos no mapa.
- **Mães presas (female)** → filhos com avós (grandparent), parentes (relative), ou foster care. Distribuídos, mais distantes.
- **Friends** → isolado no topo do mapa, outlier (raríssimo).

"By examining the resultant CA output, viewers can easily discern the striking disparities between men and women respondents." A desigualdade de gênero no sistema prisional — mães presas perdem a guarda muito mais que pais presos — fica **visualmente óbvia** no mapa. É qualitização visual em nível social: um gráfico que comunica injustiça.

### Contribuição 6 — Table 3.1: Comprehension + Extension = Mixed Methods (p.41)

Adaptado de Blasius & Greenacre (2014):

| Type of Mode | Comprehension (quali) | Extension (quanti) |
|---|---|---|
| Mode of being | Wisdom | Data |
| Mode of knowing | Experience | Knowledge |
| **Summary** | **Comprehension + Extension = Mixed Methods** | |

Formulação elegante: mixed methods não é "quali + quanti" — é **compreensão + extensão**. Compreensão vem da experiência e da sabedoria (quali). Extensão vem dos dados e do conhecimento formal (quanti). CA integra os dois no mesmo display. É outra forma de dizer 1+1=1.

### Qualitização implícita

O capítulo inteiro é sobre como CA produz displays que precisam ser **interpretados** — nomeação de dimensões, identificação de associações, leitura de proximidades. A Figure 3.1 não tem labels automáticos explicando "mães presas perdem a guarda" — o pesquisador qualitiza o mapa ao interpretá-lo. Cada leitura de um mapa CA é um ato de qualitização.

E Dickinson é explícita sobre a qualitização como ato criativo: cita Eisner (2002): "Imagination gives us images of the possible, that provide a platform for seeing the actual.... The image, the central term of imagination, is qualitative in character. We do indeed see with our mind's eye." Qualitizar um gráfico é ver com o olho da mente.

### Conexão com obsidian-qualia-coding

1. **CA como biplot é feature que o plugin não tem** — clustering e MDS operam em R-mode (só códigos). CA colocaria códigos E documentos no mesmo mapa. É a única visualização que mostra a relação cruzada.
2. **Os 3 critérios de design visual** (impact, understanding, revelation) como princípios pra todas as views de analytics.
3. **A ponte trans-paradigmática** como argumento de comunicação: o output do plugin deveria ser compartilhável com stakeholders de diferentes backgrounds sem requerer conhecimento estatístico — a visualização opera pré-paradigmaticamente.

### Sobre o livro Routledge — quinteto completo

Com este capítulo, documentamos 5 dos capítulos do handbook:

| Cap | Autor | Método | Contribuição única |
|---|---|---|---|
| **3** | Dickinson | CA | Biplot (temas+participantes juntos), ponte trans-paradigmática |
| **4** | Suerdem | MDS | Hermenêutica visual, semiosis (Peirce) |
| **5** | Péladeau | Cluster | R-mode/Q-mode formal, clustering pra amostragem |
| **13** | Onwuegbuzie & Leech | Qualitização | Definição expandida 5 elementos, fórmulas de integração |
| **14** | Saldaña | Coding | 10 técnicas de codificação, Magnitude Coding system |

Juntos formam o **manual operacional** do DIME do Onwuegbuzie (2025), publicado 4 anos antes do paper que formaliza o framework.

---

## 20. Onwuegbuzie, A. J. & Johnson, R. B. (2021). Mapping the Emerging Landscape of Mixed Analysis (Cap 1)

**Fonte:** In A. J. Onwuegbuzie & R. B. Johnson (Eds.), *The Routledge Reviewer's Guide to Mixed Methods Analysis* (pp. 1-10). Routledge.
**Arquivo:** `./GTQQ/1.Mapping the Emerging Landscape of Mixed Analysis.pdf`

| | |
|---|---|
| **Autores** | Anthony J. Onwuegbuzie, R. Burke Johnson |
| **Instituições** | University of Johannesburg; University of South Alabama |
| **País** | África do Sul / EUA |
| **Ano** | 2021 |
| **Editora** | Routledge |
| **Setor/Contexto** | Metodologia — capítulo de abertura que mapeia o campo inteiro da mixed analysis e organiza o handbook |
| **Tipo** | Meta-capítulo — o mapa do território. Posiciona todos os métodos num framework único (CAF). Fecha nossa leitura do handbook. |

### Resumo

Capítulo de abertura do Routledge handbook, escrito pelos editores. Não apresenta método novo — **organiza todos os métodos num framework único**. É o meta-mapa: as 5 equações de mixed analysis, a distinção horizontal vs. vertical, a crossover matrix 3×3×3 (Table 1.1), os 3 tipos de inter-respondent matrix, a hierarquia technique→method→approach, e o número combinatório explosivo. Tudo o que documentamos nos 19 papers/capítulos anteriores cabe numa célula da Table 1.1. É a referência pra dizer "onde cada coisa se encaixa."

### Contribuição 1 — As 5 equações de mixed analysis (pp.2-3)

A progressão formal mais completa que existe:

**Equação 1:** `Mixed analysis = Non-crossover + Crossover`
Toda análise mista combina os dois tipos em alguma proporção.

**Equação 2:** `Non-crossover = Quanti monoanalysis + Quali monoanalysis`
Cada lado analisado com seus métodos nativos, sem cruzar. É o que a maioria faz.

**Equação 3:** `Quanti monoanalysis = análise quanti de dados quanti`
O que todo curso de estatística ensina.

**Equação 4:** `Quali monoanalysis = análise quali de dados quali`
O que todo curso de métodos qualitativos ensina.

**Equação 5:** `Crossover = (quanti de quali) ∪ (quali de quanti) ∪ (quanti de quanti+quali) ∪ (quali de quanti+quali) ∪ (quali ∪ quanti de multidata)`
As 5+ combinações possíveis de crossover. **Quantitização** (quanti analysis de quali data) e **qualitização** (quali analysis de quanti data) são subtipos, mas existem combinações mais complexas que nenhum dos dois termos cobre sozinho.

O conceito de **multidata** (Onwuegbuzie, Gerber & Abrams, 2017, p.28): dados que não são claramente quali NEM quanti — "noös data" que "includes a sense of 'being present with' and empathy... [that] is not as easily defined, qualified, or quantified." É o **unsaid** do Nzabonimpa (2018) formalizado como tipo de dado dentro da Equação 5.

### Contribuição 2 — O número combinatório explosivo (p.1)

Onwuegbuzie, Leech & Collins (2011): com 58 classes de análise quanti e 60 de análise quali, existem **3.480 combinações** possíveis usando apenas 1 técnica quanti + 1 quali. Incluindo não-paramétricas e bayesianas, cresce exponencialmente.

Com **8 fontes de dados** (5 quali + 3 quanti): mais de **1 milhão** de permutações pra análise sequencial.
Com **10 fontes**: mais de **1 bilhão**.
Com **12 fontes**: excede a definição britânica de 1 bilhão.

O campo de mixed analysis tem possibilidades combinatórias **praticamente infinitas** — e a maioria dos pesquisadores usa as 3 mais básicas (non-crossover horizontal). O handbook inteiro — e por extensão todo o nosso projeto — é exploração de um espaço quase virgem.

### Contribuição 3 — Figure 1.1: Horizontal vs. Vertical mixed analysis (p.4)

| | Horizontal | Vertical |
|---|---|---|
| **Interação** | Nenhuma durante análise; só na interpretação final | Achados quanti e quali **interagem** durante a análise |
| **Design** | Concurrent/paralelo — strands independentes | Sequential — uma fase informa a seguinte |
| **Integração** | Low — separadas até o final | High — cruzam durante o processo |
| **Cross-tracks?** | Não | Sim (Li, Marquart & Zercher, 2000): "oscillating continually between both data sets" |

O pipeline que documentamos (Macia, Henry) é **vertical**: codificação (quali) → binarização (quanti) → clustering (quanti) → retorno ao quali (qualitização). Cada fase informa a seguinte. A maioria da pesquisa publicada é **horizontal** — quali e quanti lado a lado, reportados em seções separadas, sem interação real.

### Contribuição 4 — Table 1.1: A crossover matrix 3×3×3 (pp.5-6)

A tabela mais completa que lemos. Cruza 3 dimensões:

**Eixo 1 — Nível de análise:**
- **Technique** (microanalysis): procedimento singular (calcular média, in vivo coding, single quantitizing)
- **Method** (mesoanalysis): conjunto integrado de técnicas (t-test = média + desvio + comparação; within-case analysis; multi-qualitizing)
- **Approach** (macroanalysis): sistema completo (descriptive analyses; constant comparison; fully integrated mixed analysis)

**Eixo 2 — Complexidade:**
- **Non-complex:** poucos passos, descritivo (frequência de temas, word count, parallel analysis)
- **Intermediate:** múltiplos passos, relacional (ANOVA, cross-case display, values coding, multi-qualitizing, joint display)
- **Complex:** altamente inferencial (HLM, Bayesian, interpretative phenomenological analysis, fully integrated quantitizing/qualitizing, CA, EFA, MDS, cluster analysis)

**Eixo 3 — Tradição:** Quantitative / Qualitative / Mixed

Na célula **Complex + Mixed + Methods** estão listados: "fully integrated quantitizing; fully integrated qualitizing (Chapter 13); correspondence analysis of themes (Chapter 3); exploratory factor analysis of themes (Chapter 2); multidimensional scaling (Chapter 4); cluster analysis (Chapter 5)..." — **tudo o que documentamos nos papers e capítulos anteriores cabe nesta célula**. É o mapa do território, e nosso corpus inteiro habita o quadrante mais sofisticado.

### Contribuição 5 — Os 3 tipos de inter-respondent matrix (Tables 1.2-1.4)

Os 3 tipos de scoring do Boyatzis (1998) reformulados como **tipos de matriz**:

| Tipo de matriz | Conteúdo das células | Equivalente Boyatzis | Exemplo |
|---|---|---|---|
| **Frequency-based** (Table 1.2) | Contagem de ocorrências por tema por participante | Scoring tipo (d) — frequência livre | Halle: Theme 1 = 5, Theme 5 = 6 |
| **Incident-based** (Table 1.3) | Presença/ausência 0/1 | Scoring tipo (b) — presença/ausência | ID 001: Theme 1 = 1, Theme 3 = 0 |
| **Intensity-based** (Table 1.4) | Rating scale (1-5) por tema por participante | Scoring tipo (e) — intensidade | ID 001: Theme 1 = 1, Theme 4 = 4 |

A incident-based (Table 1.3) é a binarização que Macia, Henry e Driscoll usam. A frequency-based (Table 1.2) é o scoring com J-curve que Boyatzis alerta. A intensity-based (Table 1.4) é a alternativa ordinal que Sandelowski (2009) propôs e Saldaña (2021) operacionalizou com Magnitude Coding.

### Contribuição 6 — A hierarquia Technique → Method → Approach (pp.4-5)

Via Crossover Analysis Framework (CAF) de Hitchcock & Onwuegbuzie (2020):

"In qualitative, quantitative, and mixed research, with respect to data analysis, **techniques are nested within methods, which, in turn, are nested within approaches**" (p.66).

Posiciona tudo o que documentamos:
- **Dendrograma do Qualia Coding** = technique (microanalysis)
- **Pipeline dendrograma → nomeação → retorno ao texto** = method (mesoanalysis)
- **Processo completo codificação → analytics → interpretação → iteração** = approach (macroanalysis)

### Contribuição 7 — "Effect sizes" qualitativos (p.8)

Onwuegbuzie (2003): frequências da inter-respondent matrix são **manifest effect sizes** — "effect sizes that pertain to observable content." A frequência de um tema na amostra não é "contagem" — é **medida de efeito qualitativo**. Complementa Sandelowski (2001) sobre "number play" e dá vocabulário formal pro que ela descrevia informalmente.

### Contribuição 8 — Qualitizing como core crossover (p.10)

Seção dedicada: "Qualitizing as a Core Crossover Mixed Analysis." Posiciona qualitização como **core** — não periférica. Confirma a progressão single → multi → fully integrated qualitizing (Cap 13). E: "Consistent with qualitizing, a structured narrative may be built around each grouping of codes/themes" — clustering gera narrativa. Confirmação editorial: clustering é ferramenta de qualitização.

### Contribuição 9 — Tour pelos 24 capítulos como mapa (pp.9-10)

Cada capítulo posicionado no CAF com o tipo de inter-respondent matrix que usa. Documentamos 6 dos 24 (Caps 1, 3, 4, 5, 13, 14). Os outros 18 oferecem extensões potenciais: EFA (Cap 2), CHAID (Cap 6), Regressão Múltipla (Cap 7), SEM (Cap 8), HLM (Cap 9), Bayesian (Cap 10), IRT (Cap 11), Diachronic (Cap 12), Mixed Methodological Discourse Analysis (Cap 15), Ethnographic Decision Models (Cap 16), Qualitative Comparative Analysis (Cap 17), Q Methodology (Cap 18), Social Network Analysis (Cap 19), Social Media Analytics (Cap 20), GIS (Cap 21), Nonverbal Communication (Cap 22), Joint Display (Caps 23-24).

### Qualitização implícita

O capítulo inteiro é meta-qualitização: pega a estrutura numérica do handbook (24 capítulos, 3×3×3 matrix, 5 equações) e transforma em narrativa interpretativa sobre "the emerging landscape." O ato de **nomear** o landscape — mapear, posicionar, organizar — é qualitização do campo inteiro.

### Conexão com o Foundations.md e o projeto

1. **O número combinatório** (3.480 a 1+ bilhão de permutações) é o argumento mais forte pra justificar o projeto: o campo é vastíssimo e sub-explorado. O que estamos documentando habita o quadrante Complex + Mixed da Table 1.1 — o mais sofisticado e menos praticado.

2. **A distinção horizontal vs. vertical** posiciona o pipeline do Foundations.md como vertical — cada fase informa a seguinte. É a forma mais integrada de mixed analysis, que a maioria dos pesquisadores não pratica.

3. **Os 3 tipos de inter-respondent matrix** dão vocabulário formal pras escolhas de scoring: o Qualia Coding hoje gera incident-based (0/1 por código por segmento). Poderia gerar frequency-based (contagem) e intensity-based (Magnitude Coding do Saldaña) como opções.

4. **A hierarquia technique→method→approach** dá framework pra comunicar o que o plugin é: não é uma técnica — é **método** (pipeline integrado) e potencialmente **abordagem** (sistema completo de análise).

---

## Leitura Cruzada — Cada Referência Vista pelas Outras

Seção que cresce a cada nova referência. Analisa como um paper/livro ilumina, valida, contradiz ou expande os outros.

### Boyatzis (1998) como lente

#### Sobre Macia (2015)

A Macia usa scoring tipo (b) — presença/ausência — que é exatamente o que Boyatzis recomenda como **mais robusto**. A binarização dela (59 variáveis 0/1) é o tipo de scoring que menos distorce os dados qualitativos. Escolha acertada, conscientemente ou não.

Mas ela vai além do Boyatzis num ponto: **separa variáveis de agrupamento vs. interpretação** (excluindo demográficas do clustering e usando-as depois na cross-tabulação). Boyatzis discute clustering conceitual vs. empírico, mas não trata dessa separação estratégica de variáveis. É uma contribuição metodológica da Macia que o framework do Boyatzis não antecipou.

A unidade de análise (evento/queixa, não pessoa) é exatamente o tipo de decisão que o Cap 3 do Boyatzis diz que precisa ser **explicitada e justificada**. Macia explicitou bem — mas pelo framework de Boyatzis, a dependência entre queixas da mesma pessoa (21 → 195) mudaria a distribuição dos scores e portanto quais análises são legítimas. Boyatzis avisaria: a J-curve já distorce com dados independentes; com dependência estrutural, a distorção pode ser pior.

#### Sobre Henry et al. (2015)

Henry também usa scoring tipo (b) (presença/ausência, 56 códigos binarizados). A codificação puramente indutiva (grounded theory) é o que Boyatzis chamaria de "data-driven" (Cap 4). A unidade de análise é a pessoa (77 líderes) — mais conservadora que a Macia, mais alinhada com os exemplos do Boyatzis (gerentes como unidade).

A qualitização colaborativa do Henry (Executive Director + board validam nomes de clusters) ecoa diretamente o que Boyatzis descreve: os executivos validaram os clusters empíricos de competências, e a apresentação "appeared to make sense to executives and human resource professionals". São processos sociais muito parecidos, 17 anos de diferença — e nenhum dos dois chama de qualitização.

A simulação do Henry (validando que clustering funciona com binários e N pequeno) é a **evidência que Boyatzis não tinha em 1998**. Boyatzis sabia que J-curve e N pequeno eram problemas — alertou sobre distribuições não-normais e limitações de análises paramétricas. Mas não tinha simulação pra provar que clustering hierárquico ainda assim funciona com dados binários até N=20. O Henry preenche essa lacuna 17 anos depois.

#### Sobre Morin (2006) / AC

A AC opera sobre texto bruto (não codificado), então não usa scoring no sentido de Boyatzis. Mas o conceito de **metakeys** da Morin é análogo aos **clusters conceituais** do Boyatzis — são agrupamentos temáticos nomeados pelo pesquisador. A diferença: Boyatzis agrupa **códigos já existentes**, Morin descobre "códigos" (metakeys) **direto do texto**.

É como se a AC fizesse os passos 1-2 do Boyatzis (sensing themes + developing themes) automaticamente, pulando o passo 3 (codificação manual). As metakeys são temas emergentes não-codificados — proto-códigos descobertos estatisticamente. Isso posiciona a AC como ferramenta pro estágio **anterior** ao que Boyatzis trata: antes de ter um codebook, a AC pode sugerir o território temático.

Na discussão sobre clustering conceitual vs. empírico: as metakeys da Morin são **clustering empírico de palavras**, e a nomeação delas é o equivalente da qualitização que Boyatzis descreve quando executivos nomeiam clusters de competências.

#### Sobre Jaworska (2009) / MDS

Conexão menos direta. MDS opera sobre matrizes de dissimilaridade que podem vir de qualquer fonte — não usa scoring temático diretamente. Mas no contexto do Qualia Coding, o MDS opera sobre a **mesma matriz de co-ocorrência de códigos** que alimenta o clustering, e co-ocorrência é derivada de dados que foram scored (presença/ausência nos segmentos). Então o MDS é downstream do scoring do Boyatzis, mesmo que ele não trate disso.

O ponto de contato mais relevante: Kim et al. (2004), citado pela Jaworska, compara MDS com cluster analysis pra perfis cognitivos e conclui que **MDS dá nível + padrão enquanto cluster analysis só dá padrão**. Isso complementa o framework de Boyatzis: o scoring produz dados → clustering agrupa em categorias → MDS revela as dimensões latentes que organizam os clusters. São camadas de abstração crescente sobre o mesmo scoring inicial.

#### Sobre o projeto Sicredi (2025)

O Sicredi é o caso mais radical do ponto de vista do framework de Boyatzis:

**Unidade de análise:** O insight (nem pessoa, nem evento, nem organização) — nenhum dos exemplos do Boyatzis usa essa unidade. O Cap 3 diria que é válido mas precisa de justificativa explícita. A justificativa no caso era pragmática: o repositório já existia organizado por insights, e a pergunta era sobre tipos de experiência (não sobre tipos de pessoa ou tipos de estudo).

**Dependência multinível:** Estudo → insights (um teste de usabilidade gera 7 insights), produto → estudos (vários estudos sobre o mesmo produto), empresa → produtos. É mais severo que qualquer cenário que Boyatzis discute. A J-curve que ele descreve pra dados independentes provavelmente se agrava: insights do mesmo estudo tendem a compartilhar vocabulário e classificações, inflando co-ocorrências artificialmente.

**Scoring misto:** O repositório misturava tipos de scoring — campos nominais (tipo de insight: dor/oportunidade/insight), presença/ausência de atributos, e texto livre (descrição). A ACM operou sobre essa mistura. Pelo framework de Boyatzis, misturar níveis de medida (nominal com ordinal) sem explicitar é arriscado — a J-curve e as propriedades da escala variam por tipo de scoring.

**Qualitização:** Os territórios de experiência ("Relacionamento Humanizado", "Autoserviço Fluido", "Eficiência Operacional") foram validados com stakeholders do Sicredi — ecoando tanto o Henry (stakeholders nomeiam clusters) quanto o próprio Boyatzis (executivos validam clusters de competências). O processo social é o mesmo: output estatístico → reunião colaborativa → nomes emergem → stakeholders confirmam que "faz sentido".

**A questão aberta:** O teste de robustez proposto (rodar ACM com 1 insight por estudo e comparar territórios) seria, no framework de Boyatzis, uma verificação de se a **unidade de análise** está distorcendo os clusters empíricos. Se os territórios se mantêm com amostragem reduzida, a dependência não distorceu. Se mudam, os territórios refletiam a composição do repositório (quais estudos contribuíram mais insights), não a estrutura real da experiência.

### Driscoll et al. (2007) como lente

#### Sobre a colinearidade no Qualia Coding e o insight espelho vs. janela

A colinearidade que Driscoll nomeia como problema do merge é o gatilho pra uma distinção mais profunda: quando o pesquisador aplica múltiplos códigos ao mesmo segmento e depois roda analytics, o que vê é o **reflexo da sua própria codificação** (espelho), não a exploração do fenômeno (janela). A R-analysis atual do plugin — dendrograma, MDS, co-ocorrência — mostra como o codificador organizou os dados. A Q-analysis (Macia, Henry) mostraria como o fenômeno se estrutura entre participantes. São dois níveis de análise complementares que precisam ser explicitados. Ver seção transversal "Espelho vs. Janela".

#### Sobre o Sicredi

A ACM do Sicredi operava sobre classificações de segundo grau (como a equipe categorizou insights) — espelho do conhecimento declarado, não janela pro fenômeno da experiência. A colinearidade era estrutural: insights do mesmo estudo compartilhavam classificações. O Driscoll diria: "response categories are themselves linked as a consequence of the coding strategy" — exatamente o que acontecia com insights do mesmo estudo sendo classificados pela mesma equipe.

### Sandelowski (2001) como lente

#### Sobre Macia (2015)

A Macia faz exatamente o que a Sandelowski defende: usa números pra **gerar significado** que não era visível na análise qualitativa pura. O contraste entre clusters 5 e 6 (mesmas queixas, estratégias opostas) é um achado que emergiu do número — o clustering revelou que o vínculo, não o tipo de problema, definia a resposta. Sem contar (binarizar, clusterizar), esse padrão ficaria enterrado nas 195 narrativas.

Mas pela lente das armadilhas: a Macia está atenta ao **misleading counting** — usa N absolutos, não porcentagens (85 casos, 38 casos, etc.). E evita **acontextual counting** — sempre volta pros dados qualitativos pra interpretar os clusters. Uso exemplar de números dentro do quali.

#### Sobre Henry et al. (2015)

O Henry opera na zona que Sandelowski chama de **"number play"**: uso exploratório de números pra "see data in a new way." A simulação (48k datasets) é number play em escala industrial — mas com propósito claro de validação, não de overcounting. E a qualitização colaborativa (stakeholders rejeitam se não faz sentido) é o guardrail que Sandelowski implicitamente defende: o número só vale se gera interpretação significativa. Se o cluster não é interpretável, refaz — o número serve à compreensão, não o contrário.

#### Sobre Boyatzis (1998)

São contemporâneos (1998 e 2001) e Sandelowski cita o Boyatzis explicitamente (p.231): "Boyatzis (1998, p. 129) referred to it as 'quantitative translation.'" Ela posiciona o trabalho dele como **uma das formas** de usar números no quali — não a única. O Boyatzis sistematiza a tradução (5 tipos de scoring); a Sandelowski legitima a tradução epistemologicamente (por que contar é válido, quando é armadilha).

São complementares: Boyatzis diz **como** fazer; Sandelowski diz **por que** é legítimo e **quando** é problemático. O Boyatzis sem a Sandelowski é um manual sem justificativa. A Sandelowski sem o Boyatzis é uma justificativa sem método.

#### Sobre o Qualia Coding

A Sandelowski dá os **critérios de design** que o Boyatzis não dá. O Boyatzis diz "aqui estão 5 tipos de scoring" — a Sandelowski diz "e aqui estão 4 armadilhas de como o scoring pode dar errado." Pra uma ferramenta de software, as armadilhas são mais importantes que as técnicas — porque a ferramenta pode implementar as técnicas automaticamente, mas precisa **alertar** o pesquisador sobre as armadilhas. São guardrails de UX informados por epistemologia.

### Espelho vs. Janela: dois níveis de análise em dados codificados

Distinção emergente da leitura cruzada dos papers com a implementação atual do Qualia Coding:

**R-analysis (espelho):** Agrupa **códigos** por co-ocorrência. Mostra como o **pesquisador** organizou os dados — padrões de co-aplicação, famílias de códigos, redundâncias. É meta-análise da codificação: um espelho do codificador, não uma janela pro fenômeno.

**Q-analysis (janela):** Agrupa **casos/participantes** por perfil de códigos. Mostra como o **fenômeno** se estrutura — subgrupos, tipologias, padrões de comportamento que emergem entre pessoas, não entre códigos.

| | R-analysis (espelho) | Q-analysis (janela) |
|---|---|---|
| **Agrupa** | Códigos | Pessoas/casos |
| **Revela** | Padrões de co-aplicação do codificador | Padrões do fenômeno estudado |
| **Co-ocorrência significa** | "O pesquisador viu esses códigos no mesmo trecho" | "Essas pessoas têm perfis parecidos" |
| **Viés principal** | Reflete comportamento do codificador | Reflete estrutura do fenômeno (menos viés de codificação) |
| **Analogia** | Espelho (como eu organizo) | Janela (como o mundo se organiza) |
| **Utilidade** | Auditar codebook, identificar redundâncias, acompanhar evolução da codificação | Tipologias de participantes, segmentação, padrões contra-intuitivos |

**Ambos são válidos — mas são coisas diferentes.** O problema surge quando o pesquisador acha que está vendo o fenômeno (janela) quando está vendo a si mesmo (espelho).

**O Qualia Coding hoje opera exclusivamente em R-analysis** (dendrograma, MDS, co-ocorrência — tudo código × código). Os papers que lemos operam em Q-analysis (Macia: queixa × código; Henry: pessoa × código). São pipelines complementares:

- R-analysis (espelho) é útil **durante** a codificação: refinar codebook, detectar redundâncias, auditar vieses
- Q-analysis (janela) é útil **depois** da codificação: descobrir subgrupos, testar hipóteses, gerar teoria

**O caso Sicredi como ilustração:** A ACM operou sobre insights × classificações (tipo de insight: dor/oportunidade/etc.). Os territórios de experiência que emergiram representavam o **mapa cognitivo dos pesquisadores** — como as equipes organizaram e classificaram os achados. Não o terreno experiencial dos usuários — como eles viveram as experiências. Territórios do mapa, não do terreno. Válido como organização do conhecimento acumulado, mas epistemologicamente diferente de fenômeno.

Pra ser análise do fenômeno, precisaria de dados mais próximos da experiência: verbatims dos usuários codificados (não classificações de segundo grau feitas pela equipe). E a unidade de análise seria o usuário ou a sessão de pesquisa, não o insight.

**O que isso muda pra cada método:**
- **Clustering:** Mesmo algoritmo, outra matriz. R-analysis = famílias de códigos. Q-analysis = tipologias de pessoas.
- **AC/ACM:** AC sobre códigos × códigos = meta-análise. AC sobre casos × códigos = exploração do fenômeno. AC sobre insights × classificações (Sicredi) = mapa do conhecimento da equipe.
- **MDS:** Dimensões latentes do codebook (como o pesquisador pensa) vs. dimensões latentes do fenômeno (como o mundo funciona).

**Implicação de design pro Qualia Coding:** Dois modos explícitos com labels claros:
- **"Análise do codebook"** (R-analysis) — "Explore como seus códigos se relacionam. Útil pra refinar codebook, identificar redundâncias, auditar vieses de codificação."
- **"Análise do fenômeno"** (Q-analysis) — "Explore como seus casos/participantes se agrupam. Útil pra descobrir tipologias, padrões e subgrupos."

**Nota:** Nenhum dos papers lidos distingue explicitamente entre esses dois níveis. Boyatzis fala de clusters conceituais vs. empíricos — mas ambos operam sobre a mesma matriz (código × código). A distinção aqui é que a **escolha da matriz** determina se a análise é espelho ou janela. É uma distinção de nível superior às tipologias existentes.

**A reliability inter-rater como controle da distinção:**

Boyatzis (1998) não faz essa distinção — mas opera num contexto onde ela é parcialmente neutralizada: seus estudos usam codebooks dedutivos com **reliability inter-rater alta** (Cap 7). No caso Dreyfus (p.96), dois codificadores independentes concordaram 79%. Quando dois codificadores diferentes veem a mesma co-ocorrência entre códigos, é evidência de que o padrão é do **fenômeno**, não do codificador individual — porque vários espelhos mostrando a mesma imagem sugerem que é o objeto, não o espelho.

Isso sugere um mecanismo de controle: **a confiabilidade inter-codificador transforma espelho em janela**. Se um codificador solo faz R-analysis, é espelho puro — reflete seus padrões de codificação. Se dois codificadores independentes codificam o mesmo material e a co-ocorrência se mantém entre os dois, o padrão provavelmente é do fenômeno.

**Implicação pro Qualia Coding:** O plugin hoje é ferramenta pra pesquisador solo — não tem inter-rater. Então **todo analytics é espelho por definição**, a menos que o pesquisador saiba disso e use com essa consciência. Opções futuras:
- Importar codificação de segundo codificador e comparar co-ocorrências
- Mostrar explicitamente: "Análise baseada em codificação de 1 codificador — resultados refletem padrões de codificação, não necessariamente padrões do fenômeno"
- Alternativamente, a Q-analysis (caso × código) é menos sensível ao viés do codificador individual, porque agrupa **participantes** (que são independentes entre si), não códigos (que dependem de quem codifica)

### Colinearidade: o problema estrutural da multi-codificação

A colinearidade entre códigos é consequência direta da prática de QDA: aplicar múltiplos códigos ao mesmo segmento. É feature da codificação qualitativa, mas problema da análise quantitativa.

**Como surge:** O pesquisador lê um trecho e aplica 3 códigos (MEDO, EVITAÇÃO, INSEGURANÇA). Esses 3 códigos vão co-ocorrer em toda entrevista onde aquele trecho aparece — não porque MEDO "causa" EVITAÇÃO no fenômeno, mas porque o codificador viu os três na mesma passagem.

**Impacto nos métodos:**

1. **Clustering inflado** — códigos colineares colam no dendrograma imediatamente. Parece achado ("formam uma família!") mas pode ser artefato (o codificador aplicou ambos). O dendrograma reflete comportamento do codificador, não estrutura do fenômeno.

2. **Análise estatística perde poder** — chi-quadrado assume independência entre variáveis. Se MEDO e EVITAÇÃO são colineares, cruzar MEDO × GÊNERO pode estar contaminado pela presença de EVITAÇÃO. Regressão múltipla fica instável (multicolinearidade): coeficientes oscilam, nenhuma variável parece significativa sozinha.

3. **AC/ACM distorce** — variáveis colineares "votam juntas" pra puxar eixos, inflando a inércia. 5 códigos colineares de 20 podem dominar o eixo 1 — não por serem o tema mais importante, mas por serem redundantes. No Sicredi, insights do mesmo estudo provavelmente compartilhavam classificações parecidas, criando blocos de colinearidade que podem ter enviesado os territórios.

4. **MDS dimensionalidade fictícia** — a matriz de dissimilaridade tem rank efetivo menor que o aparente. 15 códigos com 10 redundantes em pares = 5 dimensões reais, não 15. Dimensões do MDS podem representar a mesma coisa com nomes diferentes.

**Guardrails pro Qualia Coding:**

*Antes da análise:*
1. Checar correlação phi entre todos os pares de códigos (a co-ocorrência matrix já é base pra isso)
2. Identificar pares com phi > 0.7 — candidatos a fusão ou exclusão
3. Distinguir: colineares por construção (codificador aplicou ambos ao mesmo trecho) ou por fenômeno (realmente co-ocorrem na experiência dos participantes)

*Na análise:*
4. Testar robustez: rodar com e sem códigos colineares, comparar resultados
5. Separar por contexto: como Driscoll — não cruzar códigos da mesma resposta/segmento

*No plugin:*
6. Warning automático: "Esses códigos co-ocorrem em 80% dos segmentos. Pode ser artefato de codificação."
7. View de colinearidade: heatmap de phi com thresholds visuais (vermelho >0.7, amarelo >0.5)
8. Métrica: "Sua taxa média de códigos por segmento é 3.2 — isso gera colinearidade média de phi=0.45"

**Conexão com Boyatzis:** A decisão de aplicar múltiplos códigos ao mesmo segmento (passo 3: codificar) tem consequência direta no passo 4 (interpretar padrões). Codificação "frouxa" (muitos códigos/segmento) cria muita colinearidade. Codificação "apertada" (1 código/segmento) perde nuance. A ferramenta pode mostrar a consequência sem julgar a decisão.

### Worldviews e transformação: onde cada posição nos coloca

Rodrigues (2007) sintetiza 4 posições sobre validade (positivista, neo-positivista, integradora, interpretativa) + a posição pragmatista (implícita em Tashakkori, Sandelowski). Cada posição implica uma atitude sobre a legitimidade da transformação de dados.

Mapeando os papers e atores que documentamos:

| Autor/Paper | Posição | Atitude sobre transformação |
|---|---|---|
| Macia (2015), Henry (2015), Driscoll (2007) | **Pragmatista** (a-paradigmatic) | Transforma sem discutir paradigma — foca na técnica |
| Boyatzis (1998) | **Pragmatista** | "Se você é qualifóbico ou quantifóbico, esse livro não é pra você" |
| Sandelowski (2001) | **Neo-positivista cautelosa** | Números são legítimos no quali — com guardrails |
| Sandelowski (2000) | **Integradora** | Linking vs. transforming como opções, não como hierarquia |
| Nzabonimpa (2018) | **Integradora** (substantive) | Reconhece limites (un-quantitizable) mas faz a transformação |
| Gerrish (1999) | **Neo-positivista→interpretativa** | "Cuidado, traduzir pode diluir riqueza" |
| Giddings (2006) | **Interpretativa** | Mixed methods como "cover for hegemony of positivism" |
| Rodrigues (2007) | **Integradora** | Complementaridade — divergências são oportunidades |
| Foundations.md | **Integradora pragmatista** | Busca autenticidade sem rejeitar transformação |

**O que o mapa revela:** Os papers técnicos são pragmatistas — não justificam epistemologicamente por que transformar. Os papers teóricos são integradores ou neo-positivistas — justificam com nuance. A posição interpretativa radical (Schwandt, Richardson) está **ausente** do nosso corpus — nenhum paper a defende de fato, só a Giddings a evoca como advertência.

**Implicação:** O Foundations.md pode ganhar força ao explicitar que opera na posição integradora pragmatista — reconhecendo que a transformação tem limites (Nzabonimpa), guardrails (Sandelowski), e riscos de hegemonia positivista (Giddings), mas que o pipeline Qual>Quan>Qual (template #6 de Sandelowski 2000) preserva autenticidade quando a volta ao quali é feita com rigor.

### Genealogia do conceito de transformação de dados

A árvore conceitual completa, reconstruída a partir das referências cruzadas:

```
Caracelli & Greene (1993)
│  "Data analysis strategies for mixed-method evaluation designs"
│  Conceito: "transformation" como estratégia de análise
│  Campo: avaliação educacional
│
├── Miles & Huberman (1994)
│   "Qualitative Data Analysis"
│   "Quantitizing" usado informalmente
│
├── Tashakkori & Teddlie (1998)
│   "Mixed Methodology"
│   Formalizam quantitizing/qualitizing como par de termos
│   Ground zero terminológico
│
├── Boyatzis (1998) — mesmo ano
│   "Transforming Qualitative Information"
│   "Quantitative translation" — vocabulário concorrente (perdeu)
│
├── Sandelowski (2000) — este paper
│   "Combining Qualitative and Quantitative..."
│   Costura: transformação = conceito guarda-chuva
│   Quantitização/qualitização = processos dentro dela
│   Distingue de linking (combinar sem transformar)
│
├── Sandelowski (2001)
│   "Real Qualitative Researchers Do Not Count"
│   Legitima números dentro do quali
│
├── Onwuegbuzie & Teddlie (2003)
│   Framework de análise mista
│
├── Sandelowski, Voils & Barroso (2009)
│   Ciclo infinito — quantitização e qualitização se implicam mutuamente
│
├── Nzabonimpa (2018)
│   (Im-)possibilities — assimetria prática, said/semi-said/unsaid, limites estruturais
│
└── Onwuegbuzie (2025)
    Modelo DIME — reorganização hierárquica da quantitização
```

**O que a genealogia revela:**
- "Transformação de dados" (Caracelli & Greene 1993) é o conceito mais amplo
- "Quantitização/qualitização" (Tashakkori & Teddlie 1998) são os processos direcionais dentro dele
- A Sandelowski (2000) é quem faz a costura entre os vocabulários
- O campo nasce na avaliação educacional (1993), migra pras ciências sociais (1998), enfermagem/saúde (2000-2009), e volta pra educação (Nzabonimpa 2018). Prática transdisciplinar.
- Boyatzis (1998) é contemporâneo mas com vocabulário que não prevaleceu — evidência de que o campo precisava desses termos e dois autores independentes chegaram ao mesmo lugar

**Referência a investigar:** Caracelli & Greene (1993) — o ground zero do conceito de transformação. Anterior a tudo. Baixar e ler.

### Onwuegbuzie & Leech (2021, Cap 13) como lente — qualitização tem framework

#### Sobre o gap #5 — parcialmente preenchido

O paper solo nunca saiu. Mas o capítulo existe (2021) com definição expandida, 5 elementos, demonstração empírica, e dados de sub-utilização. O gap se reconfigura: não é "qualitização não tem sistematização" — é "qualitização tem sistematização escondida num capítulo de livro que poucos leram." A sub-denominação é meta: o próprio conceito de qualitização é sub-denominado na literatura sobre si mesmo.

#### Sobre todos os papers técnicos — relidos como qualitização

Se cluster analysis é ferramenta de qualitização (não de quantitização) quando o output é interpretação qualitativa, então:
- **Macia (2015):** Fez **multi-qualitizing** — binarização (meio) → clustering (meio) → cross-tab (meio) → nomeação de 7 clusters com retorno ao quali (fim)
- **Henry (2015):** Fez **qualitização colaborativa** — clustering (meio) → co-construção com stakeholders (fim)
- **Morin (2006):** Fez **qualitização interpretativa** — AC (meio) → nomeação de metakeys com experts (fim)
- **Boyatzis (1998):** Teorizou qualitização avant la lettre — os 5 perfis de T&T 1998 são formas de qualitização
- **Sicredi:** Fez **multi-qualitizing retrospective** — repositório (dados existentes) → ACM (meio) → territórios de experiência (fim)

Nenhum deles usou o termo "qualitização." Todos fizeram.

#### Sobre o Qualia Coding — o plugin é ferramenta de qualitização

Reconfiguração fundamental: o dendrograma, MDS, co-ocorrência do Qualia Coding não são "analytics quantitativos sobre dados qualitativos." São **ferramentas de qualitização** — meios quantitativos a serviço de fins qualitativos. O pesquisador não usa o dendrograma pra ter números — usa pra **entender seu codebook** e **interpretar seus dados**. O output final é sempre qualitativo: um nome, um perfil, um insight, um retorno ao texto.

Isso muda a comunicação do plugin: em vez de "Analytics" (que soa quanti), poderia ser "Exploração" ou "Interpretação assistida" — linguagem que reflete o fim qualitativo, não o meio quantitativo.

### Onwuegbuzie (2025) como lente — o estado da arte reconfigura tudo

#### Sobre Sandelowski et al. (2009) — desconstrução → reconstrução

Sandelowski desconstruiu: data-as-taken, vagaries of counting, 7 significados de 1/0. Onwuegbuzie reconstrói: OK, contar é complexo — e aqui está o framework de como fazer com rigor (5W1H + DIME hierárquico). São complementares, não opostos. Sandelowski é o "por que questionar," Onwuegbuzie é o "como fazer depois de questionar."

#### Sobre todos os papers técnicos — posicionamento no DIME

| Paper | Nível DIME | Tipo DIME |
|---|---|---|
| Macia (2015) | Level 1 | E (cluster analysis) |
| Morin (2006) | Level 1 | E (correspondence analysis) |
| Henry (2015) | Level 1 | E (cluster + K-Means + LCA) |
| Boyatzis (1998) | Level 1 | D + E (scoring + clustering conceitual/empírico) |
| Driscoll (2007) | Level 1 | D + I (frequências + chi-quadrado) |
| Nzabonimpa (2018) | Level 1 | D + I + E (frequências + regressão + fatorial) |
| Sicredi (2025) | Level 1 + Level 4 (retrospective) | E (ACM sobre dados já existentes) |

Todos operam no Level 1 do DIME. Nenhum vai até Level 2 (spatial/temporal), Level 3 (cross-sectional/longitudinal), ou Level 4 (retrospective/prospective) — exceto o Sicredi que é retrospective por natureza (repositório de insights pré-existente). O Qualia Coding poderia expandir pra Level 2 (temporal: como códigos evoluem ao longo de uma série de entrevistas).

#### Sobre o gap #5 — o paper sobre qualitização nunca escrito

Tanto Sandelowski (2009, p.1: "We plan to emphasize qualitizing in another article") quanto Onwuegbuzie (2025: repete a intenção) prometem artigo dedicado à qualitização. Nenhum foi publicado até 2025. São 16 anos de promessa. O Foundations.md pode ser a primeira sistematização dedicada — usando a evidência empírica dos papers técnicos como base.

#### Sobre a tese de sub-denominação

O dado de 15.9% no JMMR é a evidência estatística mais forte pra nossa hipótese: quantitização é prática disseminada mas sub-denominada. Se o principal journal de mixed methods tem apenas 1 em 6 artigos mencionando o termo, e a prática de transformar dados é muito mais comum que isso, a maioria faz sem nomear. É o argumento empírico que faltava.

### Sandelowski, Voils & Knafl (2009) como lente — o que a desconstrução revela nos papers técnicos

#### Sobre Macia (2015) — 195 "1s" que significam coisas diferentes

Quando a Macia binariza 195 queixas em 59 variáveis (0/1), cada 1 pode significar: a queixa envolveu esse atributo espontaneamente, ou o protocolo de entrevista perguntou sobre isso, ou a pesquisadora inferiu da narrativa. A cross-tabulação e o clustering tratam todos os 1s como equivalentes. Os clusters que emergem herdam essa ambiguidade — mas o insight sobre "vínculo define resposta" pode ser robusto apesar disso, porque padrões fortes sobrevivem a ruído.

#### Sobre Boyatzis (1998) — os 5 tipos de scoring à luz da desconstrução

Boyatzis propõe presença/ausência como "mais robusto" — mas a Sandelowski 2009 mostra que é o mais ambíguo. A escala ordinal (tipo e, intensidade) que Boyatzis trata como "mais problemática" é na verdade a que preserva mais informação. A hierarquia se inverte: o que é estatisticamente mais robusto (binário) é epistemologicamente mais lossy. O que é estatisticamente mais problemático (ordinal/intensidade) é epistemologicamente mais rico.

#### Sobre o Qualia Coding — espelho/janela ganha nova camada

A distinção espelho/janela que propusemos opera no output (o cluster reflete o codificador ou o fenômeno?). A Sandelowski 2009 adiciona uma camada anterior: o **input** (o 1/0) já é ambíguo. Então o espelho tem 2 camadas: (1) o 1/0 reflete a experiência ou o método de coleta? (2) o cluster reflete os 1/0 ou os padrões do codificador? São dois níveis de ambiguidade acumulada.

#### Os 5 gaps como programa de pesquisa

Os gaps identificados não são falhas do paper — são extensões que a autora não fez (e reconhece: prometeu artigo sobre qualitização que não publicou). Constituem um programa de pesquisa que o Foundations.md pode articular:

1. Assimetria prática do ciclo (documentada pelo Nzabonimpa)
2. Desconstrução do output, não só do input (nossa contribuição: espelho/janela)
3. Colinearidade como amplificador (nossa contribuição via Driscoll + Qualia Coding)
4. Operacionalização do scoring ordinal (lacuna técnica)
5. Teorização da qualitização (lacuna da própria autora)

### Rodrigues (2007) como lente — a fronteira quantificação/quantitização

#### Sobre Sandelowski (2001) e Boyatzis (1998) — o conflito

A Rodrigues formaliza uma fronteira que os outros deixam borrada: contar frequências (quantificação) é diferente de transformar dados (quantitização). A Sandelowski em "Do Not Count" (2001) defende que contar é parte do quali — mas em 2000 define quantitizing como transformação. O Boyatzis trata os 5 tipos de scoring como continuum sem marcar onde contar vira transformar. A Rodrigues marca: **quando o código numérico permite análise estatística que o qualitativo não permitiria, cruzou a fronteira**. Presença/ausência exportada pra clustering = quantitização. Frequência num gráfico de barras dentro do NVivo = quantificação.

Isso importa pro Qualia Coding: o plugin faz os dois, mas não distingue. O dendrograma é quantitização (transforma co-ocorrência em distância Jaccard → clustering). A view de frequência de códigos é quantificação (conta, mantém no quali). Explicitar qual é qual seria guardrail epistemológico.

#### Sobre a legitimação de conversão (Onwuegbuzie & Johnson 2006)

A tipologia de 9 legitimações dá framework formal pra avaliar qualidade da transformação de dados. O tipo (e) — legitimação de conversão — é o critério específico: "a quantitização e qualitização produzem meta-inferências com qualidade?" Tudo que discutimos (J-curve, colinearidade, espelho/janela, armadilhas da Sandelowski, assimetria do Nzabonimpa) são aspectos desse tipo de legitimação. É o heading teórico que falta no Foundations.md pra organizar os guardrails.

#### Sobre espelho/janela e double-coding

O inter-rater de 98.4% que Rodrigues alcançou é evidência empírica do mecanismo que discutimos: double-coding transforma espelho em janela. Se o Qualia Coding é ferramenta solo (sem inter-rater), todo analytics é espelho por definição — e a Rodrigues mostra o caminho alternativo.

### Tashakkori & Teddlie (1998) como lente — o ground zero

#### Sobre todos os papers técnicos

Todos usam o vocabulário que nasce aqui. Macia binariza (quantitizing tipo 3). Henry valida a binarização. Driscoll operacionaliza o merge. Boyatzis chama de "quantitative translation" no mesmo ano — vocabulário concorrente que perdeu. Sandelowski (2000) expande e teoriza o que Tashakkori & Teddlie cunharam. Nzabonimpa (2018) testa empiricamente 20 anos depois. A genealogia inteira parte desta p.126.

#### Sobre manifest vs. latent e o said/semi-said

A distinção manifest/latent content (pp.121-123) antecipa em 20 anos a taxonomia said/semi-said/unsaid do Nzabonimpa. Manifest = said (contável). Latent = semi-said (interpretativo). O unsaid (silêncio, omissão) é o que nenhum dos dois cobre — Nzabonimpa adiciona a terceira camada.

#### Sobre profile vs. typology e o Qualia Coding

A distinção é crucial pro plugin: profile (QUAN→QUAL) é qualitização — o que o plugin deveria oferecer pós-clustering. Typology (QUAL→QUAN) é o pipeline inverso — classificar casos qualitativamente e depois validar com analytics. São dois fluxos diferentes que usam as mesmas ferramentas (clustering, fatorial) em direções opostas. O plugin deveria suportar ambos.

#### Sobre a heurística 6-8 códigos e colinearidade

Se 200 unidades geram 10-15 códigos iniciais que se consolidam em 6-8, e o pesquisador tem 40, a colinearidade é praticamente garantida. A heurística de Tashakkori dá base empírica pro warning do plugin: "Seu codebook pode ter códigos redundantes — o dendrograma mostra X pares com phi > 0.7."

### De Lisle (2011) como lente — posicionamento paradigmático dos papers

As 5 stances e os 3 subtipos dão vocabulário pra mapear onde cada referência opera:

| Paper | Subtipo (Johnson et al.) | Stance (Greene) | Evidência |
|---|---|---|---|
| Macia (2015) | Quantitative dominant | A-paradigmatic | Binariza quali pra clustering sem discutir paradigma |
| Morin (2006) | Quantitative dominant | A-paradigmatic | AC como ferramenta técnica, sem discussão epistemológica |
| Henry (2015) | Quantitative dominant | Substantive | Validação empírica guiada pelo problema (prevenção comunitária) |
| Boyatzis (1998) | Ponte (qualquer subtipo) | Pragmatist (a-paradigmatic) | Análise temática como "tradutor" entre paradigmas |
| Jaworska (2009) | N/A (review) | A-paradigmatic | MDS como técnica, sem posicionamento |
| Driscoll (2007) | Quantitative dominant | Substantive | Merge pra análise estatística guiado pelo problema (vacinas) |
| Sandelowski (2001) | Qualitative dominant | Dialectic | Números servem ao quali; tensão é produtiva |
| Nzabonimpa (2018) | Pure mixed | Substantive | Faz os dois com peso igual, guiado pelo problema (educação, gênero) |
| De Lisle (2011) | Qualitative dominant | Complementary strengths | Defende designs quali-led |

**O que a tabela revela:** A maioria dos papers técnicos que lemos é **quantitative dominant e a-paradigmatic** — usam técnicas sem discutir paradigma. Os papers epistemológicos (Sandelowski, De Lisle) são **qualitative dominant com consciência paradigmática**. O Nzabonimpa é o único pure mixed.

**Implicação pra advertência de Giddings:** Se a maioria dos papers aplicados opera no modo quanti-dominant sem consciência paradigmática, Giddings tem um ponto — o mixed methods na prática tende pro positivismo. O Qualia Coding pode reproduzir isso (analytics quantitativos servindo como "fim") ou resistir (analytics servindo ao processo qualitativo de interpretação). É decisão de design.

### Nzabonimpa (2018) como lente

#### Sobre Sandelowski (2000, 2009) — refinamento, não contradição

Sandelowski propôs que quantitização e qualitização se implicam mutuamente — ciclo infinito. A proposição epistemológica continua válida: todo ato de quantitizar envolve julgamento qualitativo, todo ato de qualitizar parte de output numérico. Nzabonimpa não invalida o ciclo — opera em outros níveis. Mostra que: (1) a **prática** é assimétrica (mais software, mais comunidade, mais documentação pro lado quanti — o que confirma o argumento de que qualitização é sub-denominada); (2) existem **limites estruturais** (o semi-said e unsaid não binarizam, o Likert seco não narrativiza — dados que não entram no ciclo). Dentro do escopo do ciclo (o said, dados com gradação), ele opera como Sandelowski descreve.

#### Sobre Boyatzis (1998) — confirma e delimita

Nzabonimpa confirma que scoring tipo (b) (presença/ausência) é mais robusto — decisão empírica de coding for existence > frequency. Mas delimita o que Boyatzis não delimitou: o limite do scoring é o **said**. O semi-said e o unsaid estão fora do alcance do scoring, por mais refinado que seja.

#### Sobre Driscoll (2007) — mesma decisão, mesma razão

Driscoll mencionou que frequências podem ser "prone to confounding by repetitive respondents." Nzabonimpa operacionaliza: reteve 1 por participante sistematicamente. São a mesma solução independente — evidência de convergência metodológica.

#### Sobre o Qualia Coding e a distinção espelho/janela

O semi-said não é capturável por nenhuma ferramenta baseada em texto — é limite estrutural tanto da R-analysis quanto da Q-analysis. Mas o **said** pode ser analisado nos dois níveis: como espelho (R-analysis, padrões do codificador) e como janela (Q-analysis, padrões do fenômeno). A contribuição do Nzabonimpa é mostrar que mesmo o said tem camadas que resistem à transformação.

### A tensão da diluição: Gerrish vs. Sandelowski

Duas posições que parecem opostas mas operam em níveis diferentes:

**Gerrish (1999):** "The challenge to qualitative research must be how to interpret data **without diluting its richness**." A tradução quali→quanti é risco — contar pode achatar a complexidade. Binarizar narrativas em 0s e 1s perde nuance. Default = não traduzir. Traduzir é exceção que precisa de justificativa.

**Sandelowski (2001):** "The desire to move 'beyond numbers' should **not prevent** qualitative researchers from using numbers to get there." A recusa de contar é empobrecimento. Default = usar números quando útil. Não usar é que precisa de justificativa (porque é desperdício).

| | Gerrish | Sandelowski |
|---|---|---|
| **Premissa** | Traduzir pode diluir | Não traduzir empobrece |
| **Risco principal** | Perda de riqueza qualitativa | Subutilização de números no quali |
| **Sobre o Boyatzis** | Bom livro mas assume tradução como desejável sem justificar | Cita Boyatzis positivamente como "quantitative translation" |
| **O que protege** | A integridade do dado qualitativo | A legitimidade do número no quali |
| **Default** | Não traduzir (exceção justificada) | Usar números (recusa justificada) |

**Onde convergem:** A Sandelowski **incorpora** a preocupação da Gerrish. As 4 armadilhas são exatamente o que a Gerrish teme: overcounting analítico = números dominam e riqueza se perde; acontextual counting = contagem sem contexto qualitativo = diluição pura. A Gerrish diz "cuidado, traduzir pode diluir" — a Sandelowski responde "sim, pode — e aqui estão as 4 formas como dilui e como evitar."

**O que nenhuma das duas faz (e que o pipeline resolve):**

A Gerrish teme que a ida pra quanti seja sem volta — uma vez binarizado, o dado perde a riqueza pra sempre. A Sandelowski defende a ida mas, neste paper de 2001, não sistematiza a volta. O framework do ciclo infinito (Sandelowski, Voils & Barroso, 2009, publicado 8 anos depois) é que fecha isso: a quantitização não precisa ser sem volta porque a **qualitização reconstrói significado** a partir do output numérico.

O pipeline completo que estamos documentando resolve a tensão:

```
quali (riqueza original)
  → quanti (quantitização — com guardrails da Sandelowski)
    → quali de novo (qualitização — nomeação de clusters, perfis, interpretação)
```

A riqueza não se perde — se transforma e depois se reconstrói num nível diferente.

A Macia é a prova: binarizou 195 queixas (a Gerrish diria "diluiu!"), clusterizou (mais distância do quali), mas depois **voltou** pros dados qualitativos usando os clusters como lente — e descobriu que o vínculo definia a resposta, não o tipo de problema. O insight final é qualitativo, mais rico do que antes de contar. A contagem não diluiu — **revelou**.

**Semente pro Foundations.md:** Esse debate poderia virar uma seção — "A tensão entre riqueza e tradução" ou "O medo da diluição". Mostrando que: (1) o medo é legítimo (Gerrish), (2) existem guardrails (Sandelowski), (3) a volta é possível (qualitização, ciclo infinito), (4) o pipeline resolve a tensão — não elimina o risco, mas oferece caminho de ida E volta.

---

## Tabela Comparativa

Cresce a cada nova referência lida.

| Dimensão | Macia (2015) | Morin (2006) | Henry et al. (2015) | Boyatzis (1998) | Jaworska (2009) | Sandelowski (2001) |
|----------|-------------|-------------|---------------------|----------------|-----------------|-------------------|
| **Input** | Dados codificados (variáveis estruturadas) | Texto bruto (frequência de palavras) | Dados codificados (grounded theory) + simulação | Dados codificados (análise temática) — 5 tipos de scoring | Matrizes de dissimilaridade (qualquer origem) | Dados qualitativos codificados ou não — argumenta que números já estão lá |
| **Método** | Cluster analysis hierárquica | Análise de Correspondência fatorial | 3 métodos: hierárquico + K-Means + LCA | Scoring + Scaling + Clustering conceitual e empírico | MDS (Classical, Replicated, INDSCAL) | N/A — artigo epistemológico, não técnico |
| **Data transformation** | Binarização (0/1) | Tabela contingência léxica | Binarização de códigos | 5 tipos: nominal, presença/ausência, freq. condicionada, freq. livre, intensidade | Matriz de proximidade/dissimilaridade | Argumenta que toda codificação já é transformação (scoring nominal) |
| **Pergunta central** | "Quem se parece com quem?" | "Quais palavras/temas co-ocorrem?" | "Clustering funciona com binários e N pequeno?" | **"Como traduzir temas sem perder riqueza?"** | **"Quais são as dimensões escondidas?"** | **"Por que contar é legítimo no quali e quando é armadilha?"** |
| **Melhor quando** | Casos com variáveis discretas | Corpus textual grande | Amostras pequenas (N<100) | Qualquer dado temático codificado | Percepção, similaridade subjetiva | Sempre — é justificativa epistemológica transversal |
| **Limitação** | Precisa codificação robusta | Precisa expert | Simulação com 4 variáveis | J-curve; pressupostos de independência | Interpretação subjetiva | Não é método — é argumento. Precisa dos outros pra operacionalizar |
| **Case study** | 195 queixas (21 entrevistas) | 144 textos SERJ + 247 abstracts JSE | Simulação (48k) + 77 líderes | 1000+ gerentes; Mary Simpson | Review: odores, emoções, dor | Blaxter (46 mulheres, doenças); Sandelowski & Jones (12 casais, diagnóstico fetal) |
| **Codificação** | Dedutiva + indutiva | N/A (texto bruto) | Puramente indutiva (56 códigos) | Dedutiva + indutiva + prior-research-driven | N/A (review) | Argumento: toda codificação já implica contagem inconsciente |
| **Unidade de análise** | Evento/queixa (dependência) | Documento | Pessoa (independente) | Decisão explícita do pesquisador | Objeto/estímulo | Trata como decisão crítica mas não sistematiza (Boyatzis sistematiza) |
| **Insight principal** | Vínculo definia resposta, não tipo de problema | SERJ politematico vs. JSE monotematico | Clustering funciona com binários e N pequeno | J-curve; conceitual ≠ empírico; gênero muda clusters | MDS dá nível + padrão; cluster só padrão | Contagem é inconsciente no quali; 4 armadilhas como guardrails; "number play" como ferramenta exploratória |
| **Qualitização implícita** | Nomeação solo → retratos narrativos | Nomeação de metakeys com experts | Co-construção com stakeholders | Mary Simpson: scores → narrativa. Table 6.1: nomes de clusters | Nomeação de dimensões latentes | Table 2: semanas gestacionais → narrativa temporal. Figure 2 (Borkan): display híbrido números + quotes |
| **Tipo de qualitização** | Nomeação de categorias | Interpretação de paisagem | Qualitização colaborativa | Perfil narrativo + nomeação de clusters | Interpretação dimensional | "Number play" — uso exploratório de números pra ver dados de forma nova |
| **Agência da qualitização** | Pesquisador | Pesquisador + experts | Pesquisador + stakeholders | Pesquisador + stakeholders | Pesquisador | Pesquisador (mas defende que leitores também qualitizam ao ler tabelas) |
| **Conexão com Qualia Coding** | Q-analysis (não implementada) | Pré-codificação (exploração) | 3 métodos por N | Guardrails: J-curve, normalização, conceitual vs. empírico | R-analysis (implementado) | 4 armadilhas como guardrails de UX: verbal counting, overcounting, misleading, acontextual |
