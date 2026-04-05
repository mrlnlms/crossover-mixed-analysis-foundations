# Theory → Product Mapping — Qualia Coding × Mixed Methods Literature

Mapeamento inicial entre a fundamentação teórica (20 referências documentadas no REFERENCES.md) e o produto (obsidian-qualia-coding). Criado em 2026-03-24 como ponto de partida pra análise aprofundada.

## Status: Mapeamento inicial — aprofundar na próxima sessão

Próximos passos: ler ARCHITECTURE.md (55KB) e ROADMAP.md (17KB) do plugin com olhos da teoria. Produzir documento formal feature→fundamentação→gap→reframing.

---

## O que já tem e está fundamentado

| Feature do plugin | Referência que fundamenta | Nota |
|---|---|---|
| Dendrograma hierárquico (R-analysis, Jaccard, silhouette) | Péladeau Cap 5 (validação formal), Henry (funciona com N pequeno), Boyatzis (presença/ausência mais robusto) | Implementação validada pelo criador do QDA Miner |
| MDS scatter 2D/3D | Jaworska (review técnico), Suerdem Cap 4 (hermenêutica visual, semiosis) | Posicionar como hermenêutica visual, não "analytics" |
| Co-occurrence matrix | Macia, Henry, Péladeau — base de toda análise exploratória | Jaccard confirmado como escolha correta pra dados de codificação quali |
| CSV grid com codificação | Saldaña Cap 14 ("playground" do Excel industrializado) | Já vai além do que Saldaña descreve — batch coding, column settings, detail sidebar |
| MCA biplot | Dickinson Cap 3 (temas E participantes juntos), Morin (metakeys) | Verificar implementação: já faz biplot (linhas+colunas no mesmo mapa)? |
| Magnitude coding | Saldaña Cap 14 (sistema ordinal operacionalizado) | Plugin está à frente da teoria — já implementa o que Sandelowski 2009 propôs sem operacionalizar |
| 6 engines (markdown, PDF, CSV, image, audio, video) | Onwuegbuzie Cap 1 (multidata, 5+ fontes) | Conceito de multidata do Onwuegbuzie realizado como feature |
| REFI-QDA export/import | Ecossistema validado (Atlas.ti, NVivo, MAXQDA) | Interoperabilidade como ponte entre ferramentas |
| Codebook hierárquico | Boyatzis (conceitual vs. empírico), Tashakkori (6-8 códigos consolidados) | Plugin oferece ambos: hierarquia manual (conceitual) + dendrograma (empírico) |
| Frequência, dashboard, word cloud | Sandelowski 2001 (números no quali — com guardrails) | Precisa de guardrails: J-curve warning, N<25 sem porcentagens |
| Chi-square independence test | Macia (validação clusters × variáveis excluídas) | Fundamentado pela prática da Macia |
| Decision tree | Routledge Cap 6 (CHAID — não documentamos em detalhe) | Feature que vai além do nosso corpus teórico atual |
| Sequential analysis (lag, polar, evolution) | DIME Level 2 (temporal) — Onwuegbuzie 2025 | Plugin opera em nível que a maioria dos papers nem discute |
| Code relations (code-level e segment-level) | Saldaña: Causation Coding (triplet antecedente→mediador→resultado) | Infraestrutura pra Causation Coding já existe |
| Research Board | Não encontramos referência direta — é inovação de produto | Pode ser posicionado como ferramenta de qualitização colaborativa (Henry) |

## O que a teoria revela como gap no plugin

| Gap | Referência que fundamenta | Impacto | Prioridade sugerida |
|---|---|---|---|
| Q-analysis (agrupar participantes/documentos, não códigos) | Macia, Henry, Péladeau (R vs Q formal) — todos os papers técnicos fazem Q, o plugin só faz R | Abre pipeline inteiro dos papers: tipologias, segmentação, perfis comparativos | Alta |
| Warning de colinearidade (phi > 0.7 entre códigos) | Driscoll (nomeou), discussão espelho/janela | Pesquisador pode interpretar artefato de codificação como padrão do fenômeno | Média |
| Distinção espelho/janela explícita na UI | Contribuição original, Suerdem, Péladeau | Pesquisador precisa saber se está vendo seus padrões ou os do fenômeno | Média |
| Normalização por tamanho de documento | Boyatzis (J-curve), Sandelowski 2001 (acontextual counting) | Frequência bruta não comparável entre docs de tamanhos diferentes | Média |
| "So what?" prompts pós-analytics | Saldaña Cap 14 (prática reflexiva, analytic memos) | Facilitar qualitização do output — o fim é interpretação, não número | Baixa |
| Codebook evolution (MDS entre rounds) | Suerdem (círculo hermenêutico iterativo) | Ver como codebook amadurece ao longo da análise | Baixa |
| Coding for existence mode (1 por código por doc) | Nzabonimpa (existence > frequency), Boyatzis (presença/ausência mais robusto) | Evitar que respondentes prolixos dominem a análise | Média |
| Inter-rater comparison | Rodrigues (double-coding 98.4%), discussão espelho→janela | Único mecanismo que transforma espelho em janela | Baixa (complexo) |

## O reframing necessário (existe mas com narrativa errada)

| Feature atual | Narrativa atual (inferida) | Narrativa fundamentada |
|---|---|---|
| "Analytics" (20 views) | Análise quantitativa de dados qualitativos | **Ferramentas de qualitização** — meios quantitativos a serviço de fins qualitativos (Onwuegbuzie & Leech Cap 13) |
| Dendrograma | Clustering de códigos | **Hermenêutica visual do codebook** — revela dimensões latentes pra refinar codificação (Suerdem) |
| MDS | Mapa de similaridade | **Mapa das dimensões conceituais** — responde "quais são os eixos que organizam meus códigos?" (Jaworska) |
| MCA biplot | Análise de correspondência | **Biplot: ponte trans-paradigmática** — temas E documentos juntos, opera pré-linguisticamente (Dickinson) |
| Co-occurrence matrix | Matriz de co-ocorrência | **Espelho da codificação** — mostra como o pesquisador organizou os dados, não necessariamente o fenômeno |
| Magnitude coding | Intensidade dos códigos | **Alternativa ordinal à binarização** — preserva gradações que 0/1 elimina, reduz perda de 1/3-2/3 da variância (Cohen 1983 via Sandelowski 2009) |
| CSV grid | Planilha com codificação | **Playground de integração** — números e narrativas lado a lado (Saldaña), ferramenta de crossover analysis |
| Research Board | Canvas de síntese | **Ferramenta de qualitização colaborativa** — onde output quantitativo vira interpretação (Henry: stakeholders co-constroem significado) |

## Features já implementadas com fundamentação no Routledge (não documentadas nesta sessão)

O Routledge handbook tem 24 capítulos. Documentamos 6 nesta sessão (Caps 1, 3, 4, 5, 13, 14). O plugin implementa features fundamentadas em capítulos que **não passamos aqui** por serem mais avançados ou fora dos métodos mais básicos que priorizamos. A teoria existe — só não foi discutida ainda.

1. **MCA biplot** — Dickinson Cap 3 (documentado). Feature rara em software QDA. Verificar implementação.
2. **Magnitude coding** — Saldaña Cap 14 (documentado) + Sandelowski 2009. Já implementado.
3. **Decision tree (CHAID)** — Routledge Cap 6 (Collins, não documentado). Fundamentação existe no livro, não passamos por ela.
4. **Sequential analysis (lag, polar, evolution)** — Routledge Cap 12 (Anguera et al., diachronic analysis, não documentado). Fundamentação existe, não discutimos.
5. **Chi-square automatic interaction detection** — Routledge Cap 6 (não documentado). Idem.
6. **6 engines** — conceito de multidata do Onwuegbuzie (Cap 1, documentado). Nenhum outro QDA open-source cobre 6 formatos com codebook unificado.

**Nota original (24/mar/2026):** O gap real do plugin é **Q-analysis** — agrupar participantes/documentos por perfil de códigos. Esse sim foi ponto cego no desenvolvimento.

---

## Gap analysis expandida: os 6 modos de Cattell (adicionado 5/abr/2026)

Análise a partir da leitura do código-fonte (`evolutionMode.ts`, `evolution.ts`, `analyticsViewContext.ts`) pela lente dos 6 modos de fatoração de Cattell (1952) e da distinção espelho/janela (CONCEPTUAL-SYNTHESIS.md).

### O diagnóstico

O plugin tem **20 analytics views**. Todas operam no mesmo modo: **R-mode sobre estado atual (snapshot)**. Nenhuma implementa Q, P, O, T ou S.

| Modo (Cattell) | O que pergunta | Status no plugin | Gradiente espelho/janela |
|---|---|---|---|
| **R** (variáveis × pessoas) | Quais códigos covariam? | **20 views implementadas** — dendrograma, MDS, ACM, co-ocorrência, chi-square, decision tree, etc. | Mais espelho — coocorrência pode refletir hábito do codificador |
| **Q** (pessoas × variáveis) | Quais participantes/documentos se parecem? | **Não implementado** (gap identificado 24/mar) | Mais janela — participantes são independentes do codificador |
| **P** (variáveis × ocasiões, 1 pessoa) | Como a codificação de UM pesquisador evolui ao longo do tempo? | **Não implementado** | Espelho puro (por design) — documenta aprendizado do codificador |
| **O** (pessoas × ocasiões) | Como participantes mudam ao longo do tempo? | **Não implementado** | Janela pura — mudança longitudinal é do fenômeno |
| **T** (ocasiões × variáveis) | Quais períodos se parecem em termos de codificação? | **Não implementado** | Ambíguo — ciclo do fenômeno ou da equipe |
| **S** (pessoas × variáveis, 1 ocasião) | O que diferencia participantes agora? | **Não implementado** | Mais janela — discriminação entre participantes |

### O que o plugin tem perto (mas não é)

**Evolution Mode**: mostra **onde** cada código aparece dentro do documento (posição por linha, 0%-100%). É distribuição **espacial** intra-documento, não evolução temporal. Eixo X = posição no texto. Mais janela — reflete a narrativa do participante.

**Temporal Mode**: mostra **quando** cada código foi criado (`createdAt` timestamp). Curva cumulativa ao longo do tempo. É o mais perto de P-mode — mas não compara rodadas de codificação. Mostra timeline, não evolução comparativa. Se o pesquisador codifica tudo numa sessão, o gráfico não revela nada sobre evolução.

**Lag Sequential + Polar Coordinates**: análise de sequência entre códigos. Mais perto de análise temporal mas opera sobre a ordem no texto, não sobre tempo de codificação.

### O que P-mode real precisaria

A infraestrutura parcial já existe — `createdAt` nos markers. O que falta:

1. **Agrupamento por sessão/rodada**: se o pesquisador codifica em dias diferentes, agrupar markers por data e tratar cada dia como uma "ocasião"
2. **Co-ocorrência por rodada**: calcular a matriz de co-ocorrência separadamente pra cada rodada
3. **Diff entre rodadas**: quais códigos foram adicionados, removidos, renomeados entre T1 e T2
4. **MDS/dendrograma comparativo**: como a geometria da co-ocorrência mudou — overlay de dois MDS, um por rodada
5. **Métricas de estabilização**: a partir de qual rodada o codebook parou de mudar significativamente (convergência assintótica de von Foerster medida empiricamente)

### Implicação epistemológica

**O pesquisador não sabe em que modo está operando.** Olha pro dendrograma e acha que está vendo o fenômeno (janela). Pode estar vendo seu próprio padrão de codificação (espelho). Nenhuma view diz "isso é R-mode — mostra como seus códigos se organizam, não necessariamente como o fenômeno se organiza".

As 20 views existentes são **sofisticadas** — o plugin opera nos Levels 1-3 do DIME, cobre técnicas que a maioria dos papers nem discute. Mas operam todas na mesma perspectiva. É como ter 20 lentes diferentes num microscópio que só aponta pra uma direção. Girar o microscópio (Q-mode, P-mode) mostraria coisas que as 20 lentes não podem ver da posição atual.

### Prioridade dos gaps por impacto epistemológico

1. **Q-mode (alta)**: é o mecanismo que transforma espelho em janela. Sem ele, o pesquisador não tem como testar se a codificação captura o fenômeno.
2. **P-mode (alta)**: documenta evolução do codificador. Usa infraestrutura existente (`createdAt`). Implementa o ciclo hermenêutico do Suerdem e a convergência assintótica de von Foerster.
3. **Indicador espelho/janela na UI (média)**: não é um modo novo — é uma camada de consciência sobre os modos existentes. "Essa view tende a refletir seu padrão de codificação" vs. "essa view tende a refletir o fenômeno".
4. **O-mode (baixa por ora)**: requer dados longitudinais (mesmo participante em múltiplos momentos) — raro em UX research convencional.
5. **T-mode (baixa por ora)**: requer corpus temporal extenso — mais aplicável a projetos longitudinais.
6. **S-mode (baixa)**: variante de Q-mode pra snapshot — implementar junto com Q.

---

## Posicionamento do plugin no framework DIME

| Nível DIME | O que o plugin oferece |
|---|---|
| **Level 1 — DIME** | D: dashboard, frequência, word cloud. I: chi-square, decision tree. M: (não aplicável). E: dendrograma, MDS, MCA, co-ocorrência |
| **Level 2 — Spatial + Time** | Time: sequential analysis, evolution over time, lag. Spatial: não implementado |
| **Level 3 — Cross-sectional + Longitudinal** | Parcial: source comparison permite cross-sectional. Longitudinal via sequential analysis |
| **Level 4 — Retrospective + Prospective** | Retrospective por natureza (codifica dados já existentes) |

O plugin opera nos **Levels 1-3 do DIME** — mais sofisticado que a maioria dos papers que documentamos (que operam só no Level 1). E cobre 3 dos 4 tipos DIME (D, I, E — falta M/Measurement).

## Referências a investigar pra gaps do plugin

- **Routledge Cap 6** (CHAID) — fundamentar decision tree que já existe
- **Routledge Cap 2** (EFA) — exploratory factor analysis como alternativa ao PCA/MCA
- **Routledge Cap 12** (Diachronic analysis) — fundamentar sequential analysis que já existe
- **Caracelli & Greene (1993)** — ground zero do conceito de transformação
- **Hathcoat & Meixner (2015)** — qualitização como arte (nomear fator latente)
