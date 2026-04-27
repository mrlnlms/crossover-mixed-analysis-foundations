# Data Transformation in Crossover Mixed Analysis

Fundamentação teórica sobre **transformação de dados** no contexto da **crossover mixed analysis** (Onwuegbuzie & Johnson, 2021).

O tema central é a passagem de dados entre mundos: **quantitização** (palavras → números), **qualitização** (números → narrativas), e as implicações ontológicas dessa travessia. Cada método carrega uma ontologia embutida; transformar dados entre eles é cruzar fronteiras ontológicas.

## O que NÃO é

Não é sobre *mixed methods* no sentido convencional (combinar entrevistas com surveys, escolher entre design sequencial ou convergente). Isso é design-level e já tem cobertura ampla na literatura (Creswell, Teddlie, Plano Clark).

É sobre **mixed analysis** — o que acontece dentro da análise quando se pega um dado qualitativo e o transforma em quantitativo, ou vice-versa. Onwuegbuzie & Johnson (2021) chamam essa modalidade de **crossover** e a tratam como "a forma mais integrada" de análise mista, mas a literatura tem pouca cobertura e quase não há ferramentas que a operacionalizem.

## Por que importa

A maior parte da literatura de mixed methods foca no **design**. A análise mista — onde a integração realmente acontece — é muito menos discutida. E a camada **ontológica** que precede tudo (cada método carrega uma worldview embutida: quanti=realista, quali=construtivista) raramente é explicitada.

A travessia ontológica que ocorre na crossover analysis é a contribuição original que este trabalho busca desenvolver.

## Estrutura

```
.
├── README.md
├── Foundations.md          ← documento principal
├── notes/                  ← notas e sessões exploratórias
└── analysis/               ← análises auxiliares
```

Material legado (PDFs e binários) fica fora do versionamento.

## Status

Em re-fundação. Direções identificadas:

- [ ] Seção 0 (ou reformulação da Seção 1) com enquadramento ontológico (Crotty / Herrera Batista)
- [ ] Desenvolver "transformação de dados como travessia ontológica" — contribuição original
- [ ] Revisão editorial do `Foundations.md` (~15-20% de corte previsto)
- [ ] Ponte com data governance — "dados são o novo petróleo" como ontologia realista implícita

## Referências centrais

- Onwuegbuzie, A. J. & Johnson, R. B. (2021). *The Routledge Reviewer's Guide to Mixed Methods Analysis*
- Onwuegbuzie, A. J. (2025). Genealogia da quantitização, taxonomia de tipos de dados qualitativos
- Sandelowski, M. (2000, 2001, 2009). Natureza construída dos dados, mitos anti-número
- Crotty, M. (1998). *The Foundations of Social Research*
- Herrera Batista, M. A. (2021). *The Ontology of Design Research*
- Saldaña, J. (2020). Codificação como interpretação

Lista completa em [`analysis/REFERENCES.md`](./analysis/REFERENCES.md).

## Projetos relacionados

| Projeto | O que faz |
|---------|-----------|
| [Qualia Coding](https://github.com/mrlnlms/qualia-coding) | QDA dentro do Obsidian — analytics implementam o continuum quali→quanti |
| [Qualia Core](https://github.com/mrlnlms/qualia-core) | Motor de análise local-first via API + plugins |

## Licença

CC BY-NC 4.0
