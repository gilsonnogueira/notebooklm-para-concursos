---
type: index
id: MASTER
name: Tabela de Roteamento Central N.A.G.
version: 5.0
---

# 🗺️ 000_MASTER_INDEX

> [!NOTE]
> Este arquivo é a espinha dorsal de roteamento do ecossistema N.A.G. Ele informa ao NotebookLM e ao agente quais módulos operacionais existem (`P01` a `P20`), a finalidade de cada um e como acoplar as **Skills de Disciplina** no padrão [book-to-skill](https://github.com/virgiliojr94/book-to-skill.git).

---

## 🧭 Catálogo de Prompts Operacionais Ativos

| ID | Arquivo | Finalidade Cognitiva |
|---|---|---|
| **P01** | `PROMPT_P01_DetalharAula.md` | Dissecação e fichamento exaustivo da aula (Pareto 80/20, Analogia Operacional, Tabela de Confusão e Lei Seca). |
| **P02** | `PROMPT_P02_AnalisePreditiva.md` | Engenharia reversa de distratores, mapeamento de vetores de distorção e índice de vulnerabilidade da banca. |
| **P03** | `PROMPT_P03_GarimpoBizus.md` | Extração de Mnemônicos e bizus com pergunta-âncora de prova e gatilho de aplicação imediata. |
| **P04** | `PROMPT_P04_TutorTecnico.md` | Tutoria técnica profunda, desconstrução em primeiros princípios e contraste de correntes/jurisprudência. |
| **P05** | `PROMPT_P05_SimuladorQuestoes.md` | Geração de questões inéditas simulando o DNA da banca com calibragem cirúrgica de distratores. |
| **P06** | `PROMPT_P06_ResolucaoCirurgica.md` | Dissecação passo a passo com diagnóstico de causa raiz do erro e regra de ouro inviolável. |
| **P07** | `PROMPT_P07_RaioX.md` | Análise macro do comportamento da banca via Matriz Gravidade-Tendência-Frequência (GTF). |
| **P08** | `PROMPT_P08_SlidesExam.md` | Geração de roteiro de slides por núcleos conceituais para uso no Estúdio. |
| **P09** | `PROMPT_P09_Flashcards.md` | Geração de Flashcards atômicos (1 fato = 1 card) com suporte a oclusão Cloze `[...]` e exportação Anki. |
| **P10** | `PROMPT_P10_QuizBanca.md` | Quiz interativo em 3 níveis progressivos (Literalidade, Doutrina, Caso Prático/Jurisprudência). |
| **P11** | `PROMPT_P11_Markmap.md` | Geração de sintaxe rigorosa de Mapas Mentais Markmap / Obsidian Mindmap. |
| **P12** | `PROMPT_P12_AulaGuiadaMapa.md` | Roteiro de aula narrada em áudio fluido expandindo a hierarquia de um Mapa Mental. |
| **P13** | `PROMPT_P13_MotorCognitivo.md` | Motor cognitivo central N.A.G. (Zero ruído, BLUF absoluto e crivos de autoavaliação/evals). |
| **P14** | `PROMPT_P14_NarrarLei.md` | Roteiro de áudio falado (TTS) para leitura dinâmica de lei seca comentada. |
| **P15** | `PROMPT_P15_QuizCompilado.md` | Extração de questões diretamente de exemplos orais de aulões e revisões. |
| **P16** | `PROMPT_P16_FeynmanReverso.md` | Arguição socrática rigorosa, teste de casos limites e quebra de ilusão de competência (Método MIT). |
| **P17** | `PROMPT_P17_KitConsolidacao.md` | Kit triplo de fechamento da sessão de 90 min (One-Pager, Matriz de Erros e Top 5 Cards Cloze). |
| **P18** | `PROMPT_P18_SintesePreditiva.md` | Síntese preditiva global acumulada da matéria com Matriz de Armadilhas para reta final. |
| **P19** | `PROMPT_P19_RelatorioInterativo.md` | Hub de Relatório Interativo com síntese, tabelas GFM, mapas mentais e quizzes embutidos. |
| **P20** | `PROMPT_P20_CadernoTatico.md` | Dashboard Estratégico Executivo All-in-One por aula com KPIs, Heatmap e metadados empíricos. |

---

## 🏛️ Skills Especializadas de Disciplina (Padrão Book-to-Skill)

> **Créditos Metodológicos:** A arquitetura de substituição dos antigos frameworks estáticos (FFCC) por Skills atômicas por matéria é baseada no projeto [virgiliojr94/book-to-skill](https://github.com/virgiliojr94/book-to-skill.git).

Em vez de frameworks teóricos rígidos, o sistema opera com **Skills Dinâmicas da Disciplina**. Cada matéria possui seu próprio conjunto modular (`SKILL.md`, `cheatsheet.md`, `patterns.md`, `glossary.md` e `chapters/`).

### Invocação em Duas Camadas:
```text
Use [PROMPT_PXX] com a [SKILL_<DISCIPLINA>] para [TÓPICO / CONCEITO].
```

---

## ⚙️ Guias de Orquestração
- **GUIDE Central:** `GUIDE_CombiningPrompts.md` — Motor de combinação em duas camadas.
- **Sistema Unificado:** `SYSTEM_PROMPT.md` — Instruções mestras para colar no NotebookLM.
- **Persona Enxuta:** `PERSONA_NOTEBOOKLM.txt` — Instrução compacta para cadernos com fonte indexada.
