# Timeline Intelectual — Mixed Methods: Data Transformation

Reconstrução da gênese das ideias, não dos arquivos. O inventário (.archaeologist/inventory-*.md) mapeia a timeline dos arquivos. Este documento mapeia a timeline das **ideias e decisões** que geraram o projeto.

Status: em construção. Atualizar conforme mais chats e datas forem resgatados.

---

## Fase 0 — Pré-condições (2023-2024)

### 2023: Migração Notion → Obsidian
- Primeiro plugin Obsidian (RenderYAML) — aprender o ecossistema
- Gap identificado: exibir YAML formatado como display visual

### Jun-Jul 2024: 7 protótipos de QDA em 1 mês
- Necessidade original: **marcador de texto** no Obsidian
- Evolui pra ferramenta de codificação qualitativa
- moxs-qda → qualitative-coding-plugin → mosxqda → editorqda → mqda → managecodes → settingsPlugin
- Decisão arquitetural central: "marcações não alteram o documento" (data.json, CM6 decorations)
- Detalhes: ver `docs/PREHISTORY.md` do plugin

### Mai-Set 2024: CodeMarker v1
- Primeiro plugin "real" — CM6 decorations, data.json, multi-code markers
- Decisão que persiste até hoje: Map<fileId, Marker[]>, separação modelo/visualização

### Set 2024 → Jan 2025: Evolução do plugin
- CodeMarker v2, PDF engine, CSV engine, etc.
- 7 plugins separados que depois se consolidam em Qualia Coding

---

## Fase 1 — O gatilho (Jan-Abr 2025)

### Jan-Mar 2025: Projeto Sicredi (Meiuca Design)
- Último projeto relevante na Meiuca antes de sair
- Discovery para Sicredi PJ (banking corporativo)
- Pipeline: field visits → avaliação heurística → matriz CSD → compilação de insights
- **Aplicação de ACM (Análise de Correspondência Múltipla) em R** sobre repositório de insights
- Repositório: planilha com 200+ achados de pesquisas anteriores, classificados (dores, oportunidades, insights)
- Unidade de análise: o insight (não a pessoa, não o estudo)
- Resultado: 3 territórios de experiência ("Relacionamento Humanizado", "Autoserviço Fluido", "Eficiência Operacional")
- 6 scripts R autorais (Data Cleaning, ACM Insights, Agorad, Perfis de Experiência, Personas, Personas2)
- Entrega aceita, validada com stakeholders

### ~Mar-Abr 2025: Fim do contrato Meiuca
- Contrato acaba na semana seguinte à entrega do Sicredi
- Projeto fresco na cabeça
- Queria escrever o Sicredi como case / artigo
- **Sentia falta de embasamento teórico pra validade do trabalho**
- Inquietação: "é epistemologicamente legítimo aplicar técnica estatística sobre categorias oriundas de análise qualitativa?"

---

## Fase 2 — A pesquisa começa (Mai 2025)

### ~Abr-Mai 2025: Pesquisas iniciais focadas em ACM
- Sem contrato, tempo livre
- Pesquisa focada em fundamentar o case Sicredi
- ACM como método: buscando validação na literatura
- No caminho encontra: conceito de "dados como construídos", dados de segunda ordem/segunda mão
- Desdobra pra Latour (construção de fatos), Bourdieu (campos, capital simbólico)
- Explora mas não conclui — thread em aberto

### 15 Mar 2025: Semente
- `prompts gpt.md` criado — primeiro arquivo do projeto (editado até jun 30)
- Provavelmente prompts de pesquisa sobre ACM e métodos mistos

### 26 Mai 2025: **O MOMENTO FUNDADOR**
- Chat GPT com SciSpace: [Pesquisas em IHC → quantitização de dados](https://chatgpt.com/c/6833e25e-8d04-800c-b51b-ec24d29c1b8f)
- Começa com "pesquisas de ponta em IHC" — não com métodos mistos!
- Progressão: IHC → abordagens quanti em IHC → "como combinar quali e quanti?" → descreve o caso Sicredi → GPT responde: **"isso é chamado de quantitativização de dados qualitativos"**
- O conceito é **nomeado pela primeira vez** pra Marlon
- GPT apresenta quantitativização E qualitização juntas, com tabela comparativa, exemplos, designs (sequencial, convergente)
- Marlon constrói prompt final = programa de pesquisa que geraria o Foundations.md
- Termo usado pelo GPT: "quantitativização" (variante brasileira de "quantitização"/quantitizing)
- Arquivo salvo: `MOSx/2025-05-26 - Pesquisas em IHC.md`

### 24 Mai 2025: Chat Perplexity — spec técnico de analytics
- [Perplexity: Integrating Qualitative Coding with Advanced Quant](https://www.perplexity.ai/search/perfeito-excelente-ajuste-voce-m1094aUJRYmpy7D3J5By7w)
- **Anterior** ao chat fundador do GPT (26 mai) e aos áudios NotebookLM (24-25 mai)
- Foco: quais análises quanti/estruturais integram com codificação qualitativa de Saldaña
- Lista técnica: MDS, ACM, cluster, co-ocorrência, EFA, SNA, LDA, Markov, séries temporais, multinível, regressão, Jaccard/Gower/Coseno
- Pede: ferramentas open-source baseadas em Markdown/Obsidian (cita Quadro plugin e qc CLI Python)
- **Revela que a busca começou pelo lado técnico/produto** (quais análises implementar no plugin), não pelo lado teórico (é legítimo?)
- A inquietação teórica (Sicredi, legitimidade) só aparece 2 dias depois no chat GPT

### 24-25 Mai 2025: Primeiros áudios NotebookLM
- 2 podcasts sobre o livro do Saldaña (The Coding Manual for Qualitative Researchers)
- Notebook: [Quantitizar o Quali - Codigos to Counts](https://notebooklm.google.com/notebook/50772739-c5e7-4dc9-a6a9-ca99a6f24cac?authuser=1)
- Motivação: entender codificação qualitativa a fundo pra requisitos do plugin
- Fio condutor: análise quantitativa dos dados qualitativos codificados

### 27 Mai 2025: O projeto nasce
- Pasta criada: "2025-05-27 Mixed Methods - Data Transformation"
- Nome vem do conceito de transformação de dados (Caracelli & Greene, 1993 → Sandelowski, 2000)

### 28 Mai - 6 Jun 2025: Núcleo intenso (2 semanas)
- 60+ arquivos: papers, áudios, screenshots, projeto MAXQDA, fundamentação teórica
- Levantamento bibliográfico pesado: Macia, Henry, Morin, Boyatzis, Sandelowski, Tashakkori, Onwuegbuzie
- Escrita iterativa do Foundations.md com suporte de IA (GPT, Qwen, outros)
- Ver inventário completo pra detalhes por arquivo

### 29 Mai 2025: Memo de sensibilização teórica (Qwen)
- Documenta a gênese: trajetória designer→researcher, inquietações, encontro com ACM
- Declara 2 temas: (1) conversão de dados, (2) natureza do insight
- Declara Grounded Theory como método
- A pergunta fundadora explicitada: "é epistemologicamente legítimo aplicar uma técnica estatística sobre categorias oriundas de análise qualitativa?"

---

## Fase 3 — Cauda longa e pausa (Jun 2025 - Jan 2026)

### Jun-Jul 2025: Atividade decrescente
- Foundations.md editado (jun 5-6)
- Nota índice criada (jun 27)
- Screenshots (jul 4), PDF exportado (jul 5), último doc síntese (jul 7)

### Ago 2025: Última edição
- Nota índice editada pela última vez (ago 9)

### Set 2025 - Jan 2026: Pausa (~6 meses)
- Sem atividade no projeto Mixed Methods
- Plugin Qualia Coding continua evoluindo (6 engines, analytics, Research Board)

---

## Fase 4 — Retomada (Fev-Mar 2026)

### 20 Fev 2026: Notas de pesquisa do Routledge
- Leitura do handbook Onwuegbuzie & Johnson (2021) focando em fundamentar analytics do plugin
- Cap 2 (FATM), inter-respondent matrix, conexão com Document-Code Matrix do plugin

### 7 Mar 2026: Propostas de organização
- Documento com opções de nome pra repo GitHub
- Descrição lúcida: "O Foundations.md é a exploração teórica, o Qualia é a exploração prática. Mesmo impulso, duas formas."

### 24-25 Mar 2026: Sessão de análise (esta sessão)
- 20 referências documentadas no REFERENCES.md
- 10 contribuições originais identificadas
- Mapeamento teoria→produto (THEORY-PRODUCT-MAPPING.md)
- Inventário completo com 67+ itens
- Primeiro cruzamento sistemático dos 3 fios (plugin + profissional + teórico)

---

## Threads em aberto

### Dados de segunda ordem / segunda mão
- Surgiu no caminho da pesquisa (~abr-mai 2025)
- Conecta com Latour (construção de fatos) e Bourdieu (campos)
- Não concluído — Marlon não chegou num entendimento claro
- Conexão: repositório Sicredi = dados de terceira ordem (experiência → insight → classificação)

### O conceito de "insight"
- Declarado no memo (mai 29, 2025) como segundo tema de investigação
- Nunca explorado no Foundations.md
- "O termo funciona mais como um placeholder genérico do que como um conceito operativo"
- Pode ser a contribuição mais original — sub-teorizado na literatura

### Chats com IAs a resgatar
- GPT: chat fundador resgatado (26 mai 2025). Outros chats do período mai-jun 2025 a localizar
- Qwen: memo de sensibilização (29 mai 2025). Outros possíveis
- Outros modelos utilizados no período

---

## A convergência dos 3 fios

```
Fio 1: Plugin (2023→)
  RenderYAML → 7 protótipos → CodeMarker → Qualia Coding
  Motivação: necessidade prática de marcador de texto

Fio 2: Profissional (2025.01-03)
  Sicredi → ACM em repositório de insights → territórios de experiência
  Motivação: entregar pesquisa de qualidade na consultoria

Fio 3: Teórico (2025.03-05→)
  Inquietação pós-Sicredi → pesquisa de validação → descobre campo inteiro
  Motivação: "será que é legítimo?"

         ↓ convergem em ↓

Sessão 2026-03-24/25: primeiro cruzamento sistemático
  20 refs documentadas × plugin existente × caso Sicredi
  → REFERENCES.md + THEORY-PRODUCT-MAPPING.md + contribuições originais
```

O momento fundador (26 mai 2025) é onde o Fio 2 (Sicredi) encontra o Fio 3 (teoria): "isso é chamado de quantitativização." O Fio 1 (plugin) já existia independentemente e só converge formalmente nesta sessão (mar 2026).
