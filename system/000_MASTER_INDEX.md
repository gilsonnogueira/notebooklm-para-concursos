---
type: index
id: MASTER
name: Tabela de Roteamento
version: 4.0
---

# 🗺️ 000_MASTER_INDEX

> [!NOTE]
> Este arquivo é a espinha dorsal do ecossistema N.A.G. Ele informa ao NotebookLM quais módulos operacionais existem ("P01" a "P14") e para que servem.

## Catálogo de Fontes Ativas (Prompts)

| ID | Arquivo | Finalidade Cognitiva |
|---|---|---|
| **P01** | `PROMPT_P01_DetalharAula.md` | Dissecação extrema de uma aula (teoria, transcrição, slides). Resumo denso. |
| **P02** | `PROMPT_P02_AnalisePreditiva.md` | Mapeamento de armadilhas e pegadinhas reais cruzadas com a banca examinadora. |
| **P03** | `PROMPT_P03_GarimpoBizus.md` | Extração de Mnemônicos e "pulos do gato" dos comentários dos alunos. |
| **P04** | `PROMPT_P04_TutorTecnico.md` | Resolução de dúvidas profundas. Aprofundamento teórico denso. |
| **P05** | `PROMPT_P05_SimuladorQuestoes.md` | Geração de questões inéditas simulando o DNA e as armadilhas da banca. |
| **P06** | `PROMPT_P06_ResolucaoCirurgica.md` | Dissecação passo-a-passo de uma questão específica (análise item a item). |
| **P07** | `PROMPT_P07_RaioX.md` | Análise macro do comportamento da banca sobre um assunto (incidência). |
| **P08** | `PROMPT_P08_SlidesExam.md` | Geração de conteúdo para slides por núcleo temático (Estúdio). |
| **P09** | `PROMPT_P09_Flashcards.md` | Geração de Flashcards atômicos com alta restrição de sintaxe (Estúdio). |
| **P10** | `PROMPT_P10_QuizBanca.md` | Geração de Quiz interativo estilo examinador sênior com dicas (Estúdio). |
| **P11** | `PROMPT_P11_Markmap.md` | Geração de formato sintático para exportar Mapas Mentais ao Obsidian. |
| **P12** | `PROMPT_P12_AulaGuiadaMapa.md` | Gera um roteiro de aula em áudio (fluido) expandindo tópicos de um Mapa Mental. |
| **P13** | `PROMPT_P13_MotorCognitivo.md` | Motor Cognitivo e Metodológico de Alta Performance (Zero ruído, BLUF, Evals). |
| **P14** | `PROMPT_P14_NarrarLei.md` | Geração de Roteiro de Áudio Fluido (TTS Universal) de Lei Seca e Comentários. |
| **P15** | `PROMPT_P15_QuizCompilado.md` | Extração e geração de Quiz no Estúdio a partir de aulões/compilados por aula (verbatim). |
| **P16** | `PROMPT_P16_FeynmanReverso.md` | Feynman Reverso e Auditoria Socrática Rígida (Método MIT — Passos 2 e 4). |
| **P17** | `PROMPT_P17_KitConsolidacao.md` | Kit Oficial de Repasse e Consolidação da Sessão de 90m (Folha Resumo, Tabela de Erros, Anki). |
| **P18** | `PROMPT_P18_SintesePreditiva.md` | Síntese Preditiva Acumulada da Disciplina (Matriz de Armadilhas da Reta Final). |

## Frameworks Analíticos Especializados (FFCC Core)
Espinhas dorsais analíticas em 4 quadrantes (Forma, Função, Conteúdo, Contexto) específicas por grande área:
- **Tributário e Aduaneiro**: `FRAMEWORK_FFCC_TRIBUTARIO_ADUANEIRO.md` (Direito Tributário, Legislação Tributária e Aduaneira, Reforma Tributária).
- **Contábil e Custos**: `FRAMEWORK_FFCC_CONTABIL.md` (Contabilidade Geral, Avançada, Custos e Pronunciamentos CPC).
- **Ciências Exatas**: `FRAMEWORK_FFCC_EXATAS.md` (Raciocínio Lógico-Matemático, Matemática Financeira e Estatística).
- **Fluência em Dados**: `FRAMEWORK_FFCC_DADOS.md` (SQL, Modelagem Relacional/Dimensional, Big Data, Machine Learning e Governança).
- **Jurídico Clássico**: `FRAMEWORK_FFCC_JURIDICO.md` (Direito Constitucional, Administrativo, Previdenciário e Servidores Públicos).
- **Gestão e Governança**: `FRAMEWORK_FFCC_GESTAO.md` (Administração Geral, Pública, Gestão de Processos e Materiais).

## Guias e Orquestração
- **Guia de Mapas**: `Guia_Criacao_Mapas_Mentais.md` - Arquiteto de Mapas Mentais (Markmap / Obsidian).
- **GUIDE**: `GUIDE_CombiningPrompts.md` - Motor de combinação. Invocado quando múltiplos módulos são acionados simultaneamente.
