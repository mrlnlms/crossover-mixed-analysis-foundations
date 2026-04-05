# Costura conceitual: von Foerster + Latour + Knorr-Cetina + Péladeau

Síntese teórica que conecta a proposta de mixed analysis (R-analysis + Q-analysis sobre corpus codificado) com os teóricos que fundamentam epistemologicamente a abordagem. Articulada em sessão de discussão sobre a genealogia do projeto (abril/2026), a partir do corpo de conversas registrado no AI Interaction Analysis.

---

## A proposta em uma frase

**Mixed analysis é operar R-analysis e Q-analysis sobre o mesmo corpus codificado, alternando a unidade de análise. Cada modo é uma observação de segunda ordem sobre o outro. O pesquisador não está fora do sistema — seus códigos são parte do dado. A geometria que emerge (ACM, MDS, clusters) não é "a verdade" — é uma inscrição a mais na cadeia de Latour. Mas é uma inscrição que revela padrões invisíveis ao olho qualitativo puro: coocorrências não-óbvias, agrupamentos não-intencionais, vazios significativos.**

---

## A intuição original (4/jun/2025)

Em conversa no Claude.ai ("Data Classification and Types", 62 msgs), a proposta aparece pela primeira vez como solução pra um problema prático:

> "eu inverto colocando os trechos de segmentos codificados como unidade de análise [...] e transpose a variável pessoa antes unidade como coluna/variável"

O problema: N pequeno (5-16 documentos) inviabiliza ACM com documentos como unidade. A solução: usar fragmentos codificados como linhas (~200-300 = N robusto), com documento/participante como variável suplementar. Na época, não havia nome pra isso.

---

## Os teóricos e o que cada um fundamenta

### Heinz von Foerster — Cibernética de Segunda Ordem

**O que dá**: a linguagem pra entender *o que muda epistemologicamente* quando se inverte a unidade de análise — e o mecanismo pelo qual o ciclo R↔Q refina o conhecimento.

A distinção fundamental de von Foerster é entre **ordens de observação**:

- **Observação de 1ª ordem**: olha pro fenômeno. "O que os participantes disseram?" → codificação. O pesquisador acha que está abrindo uma janela.
- **Observação de 2ª ordem**: olha pro observador observando. "Como eu codifiquei o que disseram?" → R-analysis sobre os códigos. Agora está vendo um espelho — mas um espelho *produtivo*, porque revela padrões que não sabia que tinha.

Princípio central: **"Não vemos que não vemos."** Toda observação de 1ª ordem tem pontos cegos — o observador não vê o que não vê. A observação de 2ª ordem revela esses pontos cegos. Na ACM: os **vazios** no biplot são os pontos cegos da codificação.

A cibernética de segunda ordem não dissolve a distinção espelho/janela. Ela a **fundamenta**:

- **R-analysis é observação de 2ª ordem por natureza** — observa a codificação, não o fenômeno. É espelho. Mas é um espelho que mostra pontos cegos.
- **Q-analysis reintroduz o fenômeno** — agrupa participantes, não códigos. Devolve a 1ª ordem. É o movimento de volta pra janela.
- **Alternar R↔Q é alternar entre ordens de observação.** Cada passagem revela pontos cegos da outra.

E von Foerster vai além: o sistema **muda** a cada observação. Quando o pesquisador roda R-analysis, vê um padrão, volta e recodifica — o corpus mudou. A próxima R-analysis vai dar diferente. Cada observação perturba o sistema observado, porque o observador é parte dele.

**O ciclo operacional na prática do Qualia Coding:**

1. Codifica (1ª ordem — acha que abre janela)
2. Roda R-analysis (2ª ordem — espelho, revela padrões do codificador + pontos cegos)
3. Volta aos dados com essa consciência, recodifica (1ª ordem informada pela 2ª)
4. Roda Q-analysis (testa se a codificação captura algo do fenômeno — participantes se agrupam de forma reconhecível?)
5. Se sim: espelho virou janela. Se não: mais uma volta no ciclo.

Von Foerster diria que a janela nunca é pura — sempre tem espelho misturado. Mas o ciclo R→Q→recodificação→R é o mecanismo que **maximiza janela e minimiza espelho** a cada iteração. Sem nunca chegar em janela pura — porque o observador nunca sai do sistema. A convergência é assintótica, não absoluta.

### Bruno Latour — Inscrições em cascata

**O que dá**: a linguagem pra entender *o que acontece com os dados a cada transformação*.

Cada camada é uma inscrição em cascata — um "móvel imutável" que pode circular entre contextos mantendo certas propriedades:

1. **Primeira inscrição**: Experiência vivida → fala do participante
2. **Segunda inscrição**: Fala → transcrição
3. **Terceira inscrição**: Transcrição → segmento codificado (seleção + código do pesquisador)
4. **Quarta inscrição**: Segmentos → matriz binária (codificação vira dado tabular)
5. **Quinta inscrição**: Matriz → mapa geométrico (ACM, MDS, biplot)

Nenhuma é "o dado" — todas são traduções. E a inversão R↔Q é mais uma tradução, que revela aspectos diferentes do mesmo corpus sem destruir os anteriores.

**Conexão com quantitizar/qualitizar**: As cadeias de Latour são a operacionalização do ciclo. Quantitizar = subir da inscrição 3 pra 4 e 5 (códigos viram matriz viram geometria). Qualitizar = descer da 5 pra 3 (interpretar clusters, voltar aos segmentos originais, narrar). O ciclo completo é percorrer a cadeia nas duas direções.

### Karin Knorr-Cetina — Objetos epistêmicos

**O que dá**: a linguagem pra entender *por que isso não converge* — e por que isso é produtivo, não um defeito.

Objetos epistêmicos são caracterizados por:
1. **Sempre em processo** — nunca totalmente conhecidos
2. **Geradores de perguntas** — quanto mais se sabe, mais se quer saber
3. **"Lack of completeness of being"** — falta ontológica fundamental

Os códigos qualitativos são objetos epistêmicos. R-mode gera perguntas sobre estrutura semântica ("por que esses códigos se agrupam?"). Q-mode gera perguntas sobre perfis ("por que esses participantes se parecem?"). Cruzar os dois gera perguntas sobre como perfis habitam a estrutura ("esse participante está nesse cluster semântico — o que isso revela?"). E cada resposta gera mais perguntas. Mise en abyme — pesquisa sobre pesquisa sobre pesquisa, espelhos infinitos.

Isso não é falha do método. É a natureza dos objetos epistêmicos — e é o que torna a análise produtiva. O loop recursivo não fecha, mas cada volta revela algo novo.

### Normand Péladeau — R-mode e Q-mode (terminologia formal)

**O que dá**: os **nomes formais** pro que foi proposto intuitivamente.

Péladeau (2021, Cap 5 do Routledge Reviewer's Guide to Mixed Methods Analysis) é o primeiro na literatura de mixed methods a usar explicitamente:
- **R-mode**: clustering de variáveis/códigos — "quais códigos andam juntos?"
- **Q-mode**: clustering de casos/participantes — "quais participantes se parecem?"

Cita Henry et al. (2015) como exemplo de Q-mode e traz um Example 2 de R-mode com concept mapping. É a distinção espelho/janela formalizada.

Relevância adicional: Péladeau é criador de software QDA (QDA Miner/WordStat) — não é só acadêmico, é quem implementa. A terminologia vem de quem constrói ferramentas.

---

---

## Contribuição original: a distinção espelho/janela

A distinção espelho/janela não vem de nenhum dos teóricos diretamente. Não foi encontrada na literatura varrida (20 referências documentadas no REFERENCES.md, sessão de 24/mar/2026). É contribuição do projeto — um vocabulário aplicado que emerge da costura entre os teóricos.

### O que é

Quando o pesquisador roda R-analysis (dendrograma, MDS, ACM sobre códigos), o output pode ser duas coisas:

- **Espelho**: revela como **o pesquisador** organizou os dados. Se sempre aplica MEDO junto com EVITAÇÃO, eles aparecem juntos no cluster — não porque o fenômeno os une, mas porque o padrão de codificação os une. É reflexo do codificador.

- **Janela**: revela algo sobre **o fenômeno**. Se MEDO e EVITAÇÃO aparecem juntos porque os participantes realmente os vivem juntos, o cluster captura algo real — algo que existia nos dados antes da codificação.

O output visual é **idêntico**. O dendrograma é o mesmo. A geometria do MDS é a mesma. A diferença é epistemológica, não visual. Não dá pra saber qual é qual olhando pro gráfico.

### Como cada teórico ilumina uma faceta

**Von Foerster** fundamenta a distinção: R-analysis é observação de 2ª ordem (espelho por natureza); Q-analysis reintroduz a 1ª ordem (movimento em direção à janela). O ciclo R→Q→recodificação→R é o mecanismo de calibração — cada volta maximiza janela e minimiza espelho. A janela nunca é pura (o observador nunca sai do sistema), mas a convergência é assintótica.

**Latour** explica por que espelho é a condição default: cada inscrição em cascata transforma o dado. O código já não é a fala — é tradução. A ACM opera sobre traduções, não sobre o fenômeno. Janela é conquistada com rigor, não presumida.

**Knorr-Cetina** explica por que a ambiguidade é produtiva: códigos são objetos epistêmicos incompletos. Espelho gera perguntas sobre o codificador ("por que eu sempre junto esses dois?"). Janela gera perguntas sobre o fenômeno ("por que essas experiências coocorrem?"). Ambas as perguntas são válidas e úteis.

**Péladeau** oferece o mecanismo operacional: Q-analysis (agrupar participantes) testa se a codificação captura algo do fenômeno. Se os perfis emergentes são reconhecíveis como "tipos" reais, a codificação é mais janela que espelho. Se não fazem sentido, é espelho puro.

**Suerdem** (Cap 4 do Routledge) traz o processo concreto: **iteração como calibração espelho→janela**. O círculo hermenêutico — codifica, roda MDS, vê que algo não bate, volta, recodifica, roda de novo — é o mecanismo que gradualmente move o output de espelho pra janela.

### Indicadores operacionais

- **Colinearidade** (phi > 0.7 entre códigos): sinal de espelho — códigos podem estar medindo a mesma coisa porque o codificador os aplica juntos por hábito, não porque o fenômeno os une (Driscoll)
- **Inter-rater agreement**: o único mecanismo que transforma espelho em janela de forma verificável — se outro codificador produz padrões similares, a codificação captura algo além do codificador individual (Rodrigues: double-coding 98.4%)
- **Vazios no biplot**: pontos cegos da codificação (von Foerster: "não vemos que não vemos") — o que ninguém codificou pode ser tão revelador quanto o que foi codificado

---

## A síntese: como os teóricos se articulam

| Teórico | Pergunta que responde | Aplicação na proposta |
|---|---|---|
| **Von Foerster** | O que muda epistemologicamente ao inverter? | R = observação de 2ª ordem (espelho); Q = retorno à 1ª ordem (janela). O ciclo R→Q→recodificação→R calibra espelho→janela assintoticamente |
| **Latour** | O que acontece com os dados a cada transformação? | Cada camada é inscrição em cascata; quantitizar = subir a cadeia, qualitizar = descer. Espelho é default (tudo é tradução); janela é conquista |
| **Knorr-Cetina** | Por que a análise não converge? | Códigos são objetos epistêmicos incompletos; espelho e janela geram perguntas diferentes mas igualmente produtivas; o loop é recurso, não defeito |
| **Péladeau** | Como isso se chama formalmente? | R-mode (códigos) e Q-mode (participantes); Q-analysis testa se a codificação é espelho ou janela |
| **Suerdem** | Qual o mecanismo de calibração? | Círculo hermenêutico iterativo — cada volta de codificação+análise move o output de espelho pra janela |
| **Espelho/janela** | *(contribuição original)* | Vocabulário aplicado que nomeia o que os teóricos descrevem sem nomear: a ambiguidade epistemológica do output da R-analysis sobre codificação qualitativa |

A proposta de **Fragment-Based Correspondence Analysis** (nomeada na mesma conversa de 4/jun/2025) é a operacionalização concreta: fragmentos como linhas (R-mode granular), participante como variável suplementar (Q-mode projetado), ACM como motor geométrico. O Qualia Coding é a ferramenta que implementa R-mode; Q-mode é o gap identificado no THEORY-PRODUCT-MAPPING.md.

---

## Violação dos pressupostos como informação epistemológica

A literatura de mixed methods trata a violação dos pressupostos estatísticos como **problema técnico a resolver** — binariza com Dice (Macia), valida com N pequeno (Henry), escolhe medida de similaridade adequada (Péladeau). Mas ninguém para pra perguntar: o que significa, epistemologicamente, que a independência não existe aqui?

A posição que emerge desta costura: **quando ferramentas estatísticas multivariadas (ACM, MDS, cluster) são aplicadas sobre output de codificação qualitativa, os pressupostos são sistematicamente violados — e essa violação não é defeito metodológico, é informação epistemológica.**

### Pressupostos violados e o que cada violação revela

| Pressuposto violado | Natureza da violação | O que revela (via teóricos) |
|---|---|---|
| **Independência das observações** | Códigos do mesmo pesquisador não são independentes — são produtos da mesma estrutura cognitiva. Segmentos do mesmo participante compartilham contexto e linguagem. Achados de um repositório vêm das mesmas pesquisas sobre os mesmos usuários. | **Von Foerster**: observador está no sistema. A não-independência é informação sobre o codificador — é o espelho operando. |
| **Homogeneidade das categorias** | Codificação múltipla (3-10 códigos por segmento) cria matriz esparsa onde a maioria é zero. Categorias não são mutuamente exclusivas. A binarização resolve tecnicamente mas achata a riqueza semântica. | **Latour**: cada inscrição transforma. A esparsidade reflete a complexidade do fenômeno, não falha de design. A binarização é mais uma tradução na cadeia — perde gradações. |
| **N suficiente por categoria** | Códigos raros (aplicados 1-2 vezes) distorcem o biplot. Na Sicredi, "Associado Porte Micro" tinha 1 caso. Códigos raros puxam o espaço geométrico inteiro. | **Knorr-Cetina**: objetos epistêmicos são incompletos. Códigos raros podem ser os mais reveladores — capturam o que quase escapou da atenção. Limpar "outliers" pode ser eliminar o achado mais importante. |
| **Estabilidade dos dados** | Códigos evoluem durante a análise. O que era FRUSTRAÇÃO vira FRUSTRAÇÃO_OPERACIONAL e FRUSTRAÇÃO_SISTÊMICA. O dado muda enquanto é analisado. | **Von Foerster**: cada observação perturba o sistema. A evolução documenta aprendizado. Congelar códigos satisfaz a estatística mas destrói informação epistemológica. |

### A implicação central

A violação dos pressupostos é **o mecanismo pelo qual a R-analysis tende a ser espelho**. Se os pressupostos fossem satisfeitos (observações independentes, categorias estáveis, N grande), a geometria refletiria mais o fenômeno — mais janela. Como não são, reflete mais o codificador — mais espelho.

Mas isso não invalida a análise. **É informação de segunda ordem**: o pesquisador aprendendo sobre seu próprio processo de conhecer.

E o ciclo R→Q→recodificação→R ganha mecanismo concreto: cada volta de recodificação tende a **aumentar a satisfação dos pressupostos** — códigos mais precisos = menos co-aplicação habitual (mais independência), vocabulário mais maduro (mais estabilidade), categorias consolidadas (mais N por categoria). A convergência assintótica de von Foerster tem operacionalização estatística: é a progressiva satisfação dos pressupostos via refinamento da codificação.

---

## Nota sobre a trajetória

Esta costura conceitual não emergiu de estudo teórico deliberado. A sequência foi:

1. **Prática instrumental**: construir plugin QDA no Obsidian (mosxqda, jun/2024) — necessidade de entender como MaxQDA e NVivo funcionam, pra identificar requisitos e tornar a ferramenta flexível. Experiência prévia com MaxQDA, Dovetail.
2. **Prática analítica**: aplicar ACM em repositório real de UX (Sicredi, abr/2025) — intuição de que funciona, mas sem fundamentação.
3. **Dúvida de validade**: "estou inventando algo maluco?" (mai/2025) — a busca por legitimação.
4. **Fundamentação**: GT Mixed Analysis (mai-jun/2025) — descobre que se chama quantitizar/qualitizar, que tem 30 anos de literatura, que a inversão da unidade de análise resolve N pequeno.
5. **Buraco de coelho**: von Foerster, Latour, Knorr-Cetina (4/jun/2025, conversa "Data Classification and Types") — a teoria que chegou depois ilumina retroativamente tudo que veio antes.
6. **Formalização**: Péladeau R-mode/Q-mode (24/mar/2026) — nomes formais pro que foi proposto intuitivamente.
7. **Articulação**: esta síntese (5/abr/2026) — costura explícita entre os teóricos, nomeação da distinção espelho/janela, violação dos pressupostos como informação.

O plugin puxou o estudo de domínio (QDA, métodos de codificação). A Sicredi deu a dúvida de validade. A teoria veio depois — mas ao chegar, reorganizou tudo retroativamente. A ferramenta existia antes da teoria que a fundamenta.

---

## Origem

- **Conversa fundadora**: "Data Classification and Types" (Claude.ai, 4/jun/2025, 62 msgs) — mise en abyme, von Foerster, Knorr-Cetina, Latour, a inversão da unidade de análise, o plugin, Fragment-Based CA
- **Formalização**: "wiggly-sprouting-cupcake" (Claude Code, 24/mar/2026) — Péladeau R-mode/Q-mode, mapeamento teoria→produto, 20 referências documentadas
- **Articulação desta síntese**: Sessão de discussão sobre genealogia do projeto (5/abr/2026), cruzando corpo de 123 conversas do GT Mixed Analysis + 443 conversas do Qualia Coding

---

## Contexto de mercado: por que ninguém fez isso antes

O QDAS Competitive Landscape (docs/pm/competitors/_landscape.md, mar/2026) mapeia 20+ ferramentas em 6 tiers. Esse mapa explica por que a costura conceitual deste documento não existe na prática:

### O mercado é bifurcado e nenhum lado cruza

**Tier 1 — Academic QDAS (NVivo, ATLAS.ti, MAXQDA):** Ferramentas de 25-35 anos. Implementam codificação, coocorrência, frequência. MAXQDA é o único com analytics estatísticos sérios (Analytics Pro), mas opera no paradigma clássico: documento = unidade, pesquisador = externo, pressupostos = assumidos. Nenhum deles expõe ao pesquisador a distinção espelho/janela ou questiona o status epistemológico do output. São caixas pretas metodológicas.

**Tier 3 — AI-Native (Dovetail, Marvin, CoLoop):** Velocidade sobre rigor. Auto-coding, auto-tagging. O oposto do que esta costura propõe — aqui o pesquisador é removido do ciclo, não posicionado como observador de segunda ordem.

**Tier 4 — Open Source (Taguette, QualCoder, Quadro):** Acessíveis mas limitados. Taguette é text-only sem analytics. QualCoder adicionou AI mas não tem visualização geométrica. Quadro (Obsidian) usa Graph View — não ACM, MDS, ou clusters.

### O que nenhuma ferramenta faz

1. **R-analysis E Q-analysis no mesmo ambiente** — todas implementam uma ou nenhuma. MAXQDA tem Analytics Pro (o mais perto), mas não alterna entre modos com o mesmo corpus.

2. **Exposição dos pressupostos** — nenhuma ferramenta avisa que independência não existe quando códigos são do mesmo pesquisador. Nenhuma mostra colinearidade entre códigos. O pesquisador roda o dendrograma e assume que é janela.

3. **Ciclo codificação→análise→recodificação instrumentado** — todas permitem recodificar, mas nenhuma instrumenta o ciclo como mecanismo epistemológico. Não existe "compare o MDS da rodada 1 com o da rodada 2" (a evolução do codebook que Suerdem propõe).

4. **Dados de segunda ordem como input** — repositórios de insights (como o da Sicredi) não são input reconhecido pelas ferramentas. Elas esperam transcrições, fieldnotes, documentos primários. Não existe campo pra "camada de mediação" ou "nível de interpretação".

### Por que a convergência é rara

O landscape revela o problema estrutural: quem constrói software QDA vem da computação (resolve problemas técnicos). Quem usa vem da academia (quer rigor metodológico). Quem teoriza sobre epistemologia da pesquisa não programa. As três comunidades não se misturam.

O Péladeau é exceção — criador do QDA Miner E autor de capítulo sobre cluster analysis. Não por acaso, é dele que vem a terminologia R-mode/Q-mode. Mas mesmo ele trata os pressupostos como condição técnica, não como informação epistemológica.

A posição do Qualia Coding no mapa estratégico ("PKM + multimedia", Obsidian-native) coloca o plugin fora dos tiers convencionais. E a fundamentação teórica deste documento coloca a proposta fora do que qualquer tier oferece: **não é QDA com analytics, é mixed analysis como observação de segunda ordem instrumentada em software**.

---

## Extensão: taxonomia epistemológica de mixed analysis (esboço)

A seção sobre violação dos pressupostos trata ACM/MDS/cluster como grupo. Mas cada técnica estatística, quando aplicada sobre codificação qualitativa, tem uma **assinatura epistemológica própria** — revela um tipo diferente de informação de segunda ordem.

R/Q-analysis (Péladeau) é uma dimensão: *quem* é a unidade. A técnica é outra dimensão, ortogonal. O cruzamento gera uma matriz onde cada célula tem pressupostos violados diferentes, informação de segunda ordem diferente, e gradiente espelho/janela diferente.

### A matriz (esboço — cada célula precisa de desenvolvimento)

| | R-mode (códigos como unidade) | Q-mode (participantes como unidade) |
|---|---|---|
| **ACM** (geométrica) | Como meus códigos se organizam no espaço? Pressupostos: independência, homogeneidade. Tende a espelho (geometria da codificação). | Como os participantes habitam o espaço dos meus códigos? Mais janela (participantes são mais independentes entre si que códigos). |
| **Cluster** (classificatória) | Quais códigos "andam juntos"? Pressupostos: medida de similaridade adequada, N por cluster. Espelho se clusters refletem hábito de co-aplicação. | Quais participantes se parecem? Mais janela — perfis reconhecíveis testam se a codificação captura algo do fenômeno. |
| **Chi-quadrado** (inferencial) | Essa associação entre códigos é confiável? Pressupostos: frequência esperada ≥5, independência. Violação massiva com códigos raros. A "significância" pode ser artefato do codificador. | Essa diferença entre perfis é confiável? Menos violação — participantes são unidades mais independentes. Resultado mais próximo de janela. |
| **MDS** (espacial) | Quais as dimensões latentes da minha codificação? Pressupostos: distâncias métricas. Hermenêutica visual (Suerdem). Espelho produtivo — revela eixos inconscientes do codificador. | Quais dimensões diferenciam os participantes? Mais janela — se participantes se posicionam de forma reconhecível, as dimensões capturam algo real. |
| **Sequential/lag** (temporal) | Em que ordem os códigos aparecem na narrativa? Pressupostos: ordem temporal significativa. Pode capturar estrutura narrativa do participante OU ordem de leitura do codificador. | Como participantes sequenciam experiências? Mais janela — a temporalidade é do participante, não do codificador. |
| **Decision tree** (preditiva) | Que código prediz a presença de outro? Pressupostos: splits significativos, categorias preditoras. Pode modelar a lógica do codificador, não a do fenômeno. | Que característica prediz o perfil de codificação? Mais janela — se uma variável demográfica prediz o cluster, é achado sobre o fenômeno. |
| **Frequência** (descritiva) | Quase sem pressupostos formais, mas a violação mais sutil: contagens brutas não são comparáveis entre documentos de tamanhos diferentes. Mede frequência do fenômeno ou extensão do documento? | Frequência por participante é mais comparável — desde que normalizada por volume de fala. |

### O que a matriz propõe

**As técnicas não são intercambiáveis epistemologicamente.** A literatura de mixed methods trata a escolha de técnica como decisão metodológica ("use ACM ou cluster, depende da pergunta"). A proposta aqui é que cada técnica, quando aplicada sobre codificação qualitativa, revela um **tipo diferente de informação sobre a relação observador-observado**. Escolher a técnica não é só escolha metodológica — é escolha epistemológica.

E o gradiente espelho/janela varia por célula: R-mode + ACM é quase espelho puro. Q-mode + chi-quadrado é quase janela. O pesquisador que sabe em qual célula está operando pode interpretar o output com consciência epistemológica do que está vendo — em vez de tratar tudo como "achado" genérico.

### Escopo ampliado: qualquer base categorizada por humanos

A distinção R/Q não é exclusiva de codificação qualitativa. Aplica-se a **qualquer matriz retangular onde humanos categorizaram registros**:

- Repositório de insights de UX (caso Sicredi: linhas = achados, colunas = tipo/produto/jornada)
- Biblioteca (linhas = livros, colunas = descritores/tags)
- Base de tickets (linhas = tickets, colunas = severidade/módulo/tipo)
- Corpus de artigos (linhas = artigos, colunas = keywords)
- CRM com tags (linhas = leads, colunas = tags do vendedor)
- Survey aberta codificada (linhas = respondentes, colunas = temas)

Em todos esses casos, o mesmo gradiente espelho/janela existe: o dendrograma dos descritores de uma biblioteca é espelho (padrão do catalogador) ou janela (estrutura do acervo)? A ACM dos tipos de bugs é espelho (taxonomia do QA) ou janela (padrões reais do software)?

É por isso que von Foerster, Latour e Knorr-Cetina fundamentam a costura — eles não falam de QDA. Falam de **qualquer sistema onde humanos categorizam e depois analisam suas próprias categorizações**. A aplicação a codificação qualitativa é um caso particular, não o caso geral.

### Genealogia dos métodos: origem e tradição epistemológica

A distinção R-mode/Q-mode vem da **análise fatorial**, anos 1930-50:

| Origem | Período | Contribuição | Domínio |
|---|---|---|---|
| **Stephenson** | 1935-53 | Q Methodology — inversão da unidade de análise como paradigma (fatorar pessoas, não variáveis) | Psicologia subjetiva |
| **Cattell** | 1952 | Formaliza R-mode/Q-mode como 2 dos 6 modos de fatoração (+ P, O, S, T pra dimensão temporal) | Psicometria |
| **Benzécri** | 1960s-70s | ACM com biplot — R e Q simultâneos no mesmo espaço. Anti-pressupostos: "o modelo segue os dados, não o contrário" | Escola francesa de dados |
| **Péladeau** | 2021 | Primeira vez que R-mode/Q-mode aparece formalmente na literatura de mixed methods | Mixed methods + software QDA |

Cada método estatístico usado em mixed analysis vem de um domínio diferente, com epistemologia própria. Quando migra pra análise sobre dados categorizados por humanos, os pressupostos quebram de formas específicas à tradição de origem:

| Método | Origem | Tradição | O que pergunta (R-mode) | O que pergunta (Q-mode) | Gradiente espelho/janela |
|---|---|---|---|---|---|
| **ACM** | Benzécri 1960s | Escola francesa — geometria > probabilidade, anti-pressupostos | Como categorias se organizam no espaço? | Como registros habitam o espaço das categorias? | A que **menos sofre** com a violação — Benzécri já recusava pressupostos distribucionais. Biplot mostra R e Q juntos. |
| **Chi-quadrado** | Pearson 1900 | Inferência clássica — significância, p-valor, hipótese nula | Essa associação entre categorias é mais forte que o acaso? | A distribuição de categorias difere entre grupos? | A que **mais sofre** — depende de independência que não existe quando um humano categorizou. A "significância" pode medir consistência do categorizador. |
| **Cluster** | Sokal & Sneath 1963 (taxonomia biológica) | Classificação — agrupar por similaridade | Quais categorias formam famílias? | Quais registros se parecem? | **Intermediário** — classificação é robusta mas validação (silhouette) assume independência. |
| **MDS** | Torgerson 1952, Shepard 1962 | Psicofísica — distâncias percebidas, espaço latente | Quais as dimensões latentes da categorização? | Em que eixos os registros diferem? | **Robusto** — opera sobre distâncias/similaridades, não sobre frequências. Suerdem: "hermenêutica visual". |
| **Sequential/Lag** | Bakeman & Gottman 1997, Sackett 1979 | Etologia — observação comportamental, sequências | Categoria A é seguida por B mais que o acaso? | Registros diferentes sequenciam categorias de forma diferente? | **Mais perto do contexto** — desenhado pra observação comportamental. Ambiguidade: sequência da narrativa (janela) vs. ordem de leitura do codificador (espelho). |
| **Decision tree** | Kass 1980 (CHAID) | Marketing/segmentação — predição de outcome | Que categoria prediz a presença de outra? | Que atributo do registro prediz seu perfil de categorização? | **Q-mode mais janela** — se uma variável externa (demográfica, temporal) prediz o perfil, é achado sobre o fenômeno, não artefato. |
| **Frequência** | Descritiva básica | Contagem | Quantas vezes cada categoria aparece? | Quantas categorias cada registro recebe? | **A violação mais sutil** — contagens brutas não são comparáveis entre registros de tamanhos diferentes (documentos longos vs. curtos, entrevistas de 15min vs. 1h). |

### O padrão emergente

O gradiente espelho/janela varia por **quatro dimensões ortogonais**:

1. **Unidade de análise** (R/Q/P/O/T/S — Cattell 1952) — R tende mais a espelho, Q tende mais a janela, P é espelho puro por design (evolução do codificador), O é janela pura (trajetória do participante)
2. **Técnica** — cada uma tem pressupostos diferentes e portanto violações diferentes
3. **Tradição epistemológica de origem** — métodos vindos da observação (MDS, sequential) tendem a ser mais janela; métodos vindos da inferência (chi-quadrado) tendem a ser mais espelho quando pressupostos quebram; métodos vindos da classificação (cluster) ficam no meio; métodos vindos da escola francesa (ACM) são os mais resilientes porque foram desenhados pra operar sem pressupostos distribucionais
4. **Filosofia de pesquisa do pesquisador** (Tables 1-3, Onwuegbuzie 2025) — a ontologia, epistemologia e axiologia do pesquisador determinam como ele interpreta o output. Um pragmatista assume janela por default. Um radical constructivista (von Foerster) assume espelho. Um dialectical pluralist busca integrar ambos

### Status

Esboço. Cada célula da matriz técnica × R/Q precisa de desenvolvimento individual:
- Pressupostos formais da técnica na tradição de origem
- Natureza específica da violação em contexto de dados categorizados por humanos
- O que a violação revela (via qual teórico)
- Gradiente espelho/janela fundamentado
- Indicadores operacionais (como saber em que ponto do gradiente o pesquisador/analista está)

Trabalho pra desenvolver com calma — é potencialmente um documento em si (EPISTEMOLOGICAL-TAXONOMY.md).

---

## Branches abertas

Contribuições originais a ser desenvolvidas:

1. **O paradoxo da auto-referência**: "estou vendo apenas uma representação de mim mesmo, meus códigos e estrutura de pensamento.. não?" — von Foerster dá o frame, mas a aplicação concreta a repositórios de UX research é original

2. **Dados de segunda ordem**: quando a ACM opera sobre achados pré-categorizados (caso Sicredi: 215 achados de múltiplas pesquisas), há 5 camadas de mediação — como isso afeta validade? Conexão com Latour (cascading inscriptions) e a literatura sobre dados secundários/meta-análise

3. **A distinção espelho/janela como conceito nomeado**: não encontrada na literatura varrida (20 refs). Nomeia a ambiguidade epistemológica que os teóricos descrevem sem nomear. Possível contribuição original — investigar se existe formulação equivalente em outras tradições (reflexividade em etnografia? validade interna em grounded theory?)

4. **Violação dos pressupostos como informação epistemológica**: a posição de que as violações não são problema técnico mas informação de segunda ordem não foi encontrada articulada na literatura de mixed methods. Formalizar a tabela pressuposto→violação→informação como framework

5. **O ciclo R→Q→recodificação como satisfação progressiva dos pressupostos**: a operacionalização estatística da convergência assintótica de von Foerster. Cada volta melhora independência (códigos mais precisos), estabilidade (vocabulário maduro), suficiência (categorias consolidadas). Testável empiricamente com dados do Qualia Coding

6. **Conexão com Tables 1-3 de Onwuegbuzie (2025) — a coluna que falta**: o framework 5W1H do Onwuegbuzie responde "deve quantitizar?" pra ~40 filosofias. O que falta é um sétimo W: **"What does it mean?"** — dado que quantitizou, o que o output significa à luz da filosofia do pesquisador? A resposta depende da célula da taxonomia epistemológica (técnica × modo × tradição × filosofia). A conexão fundacional: **von Foerster é radical constructivist** — a filosofia que Onwuegbuzie classifica como "rarely embraced" pra quantitizar é exatamente a que fundamenta a costura conceitual deste projeto. Não é quantitizar *apesar* do constructivism — é quantitizar *com consciência* constructivista do que o output significa.

7. **Meta-análise do JMMR como validação empírica**: o corpus de 346 artigos do JMMR (1997-2024, Onwuegbuzie 2025: 55 mencionam quantitizing) poderia ser codificado com a taxonomia epistemológica como codebook — que técnica, que modo (R/Q), que tratamento dos pressupostos, que postura espelho/janela, que filosofia. Resultado provável: maioria opera R-mode sem saber, trata output como janela sem questionar, opera sob pragmatismo implícito. Seria evidência empírica do ponto cego estrutural. Mixed analysis sobre mixed analysis — mise en abyme como método.
