# 🏛️ Ecossistema N.A.G. (Narrative Anchor & Guide) para Concursos Públicos
### Metodologia Aberta de Engenharia de Estudos, Ingestão Automatizada e IA Fundamentada (NotebookLM + Método MIT + Anki)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-brightgreen.svg)](https://www.python.org/)
[![Google NotebookLM](https://img.shields.io/badge/Google-NotebookLM-orange.svg)](https://notebooklm.google.com/)
[![Anki Integration](https://img.shields.io/badge/Anki-Spaced%20Repetition-lightblue.svg)](https://apps.ankiweb.net/)

---

## ⚡ Quick Start (Comece em 3 Minutos)

Para começar a usar a metodologia imediatamente no seu material de estudo:

1. **Abra o NotebookLM:** Acesse [notebooklm.google.com](https://notebooklm.google.com) e crie um caderno para a sua disciplina (ex: `Direito Tributário`).
2. **Carregue suas Fontes Reais:** Suba os PDFs da sua aula (teoria, slides, questões da banca ou transcrição).
3. **Configure as Regras do Caderno:** Copie o conteúdo de [`system/SYSTEM_PROMPT.md`](system/SYSTEM_PROMPT.md) nas configurações de persona/instruções do caderno.
4. **Execute seu Primeiro Ciclo no Chat:**
   ```text
   Use P01 com FRAMEWORK_FFCC_JURIDICO para a Aula 01.
   ```
Pronto! Você receberá uma dissecação estruturada em tabelas Markdown nativas, livre de alucinações e focada nas pegadinhas da banca.

---

## 📌 O Que é o Ecossistema N.A.G.?

O **Ecossistema N.A.G. (Narrative Anchor & Guide)** é um framework metodológico e técnico desenvolvido para estudantes de **concursos públicos de alta performance** (Carreiras Fiscais, Controle, Jurídicas e Policiais).

A metodologia combate os dois maiores gargalos da preparação moderna:
1. **Sobrecarga Operacional e Fragmentação:** O tempo perdido baixando, renomeando, procurando e organizando centenas de PDFs, videoaulas e questões.
2. **Passivismo e Ilusão de Competência com IA:** O risco de usar modelos genéricos de IA (como chatbots comuns) que sofrem do fenômeno científico **"Lost in the Middle"** (Liu et al., 2024), alucinando artigos de lei ou gerando resumos superficiais que dão uma falsa sensação de domínio.

O N.A.G. ancora todo o aprendizado em um **universo estritamente fechado de fontes reais (*source-grounded memory*)** no **Google NotebookLM**, acionado pelo **Ciclo Ultradiano de 90 Minutos do Método MIT** e finalizando com retenção biológica de longo prazo no **Anki**.

---

## ⚖️ Aviso Legal, Ética e Conformidade

> [!IMPORTANT]
> **COMPLIANCE & RESPEITO AOS DIREITOS AUTORAIS:**
> 1. Os procedimentos e rotinas deste ecossistema **NÃO realizam pirataria nem quebram mecanismos de proteção contra cópia (DRM)**.
> 2. As plataformas de cursos preparatórios mencionadas (**Gran Cursos Online** e **Estratégia Concursos**) **permitem expressamente o download de videoaulas e PDFs para alunos regularmente matriculados** para fins de estudo offline.
> 3. O papel da automação é estritamente de **assistência de organização pessoal**: substitui rotinas repetitivas que o próprio aluno faria manualmente, catalogando os arquivos com uma taxonomia sistemática.
> 4. **Nenhum material didático protegido é compartilhado neste repositório.** Apenas scripts de organização, instruções metodológicas (prompts) e templates de documentação são fornecidos.

---

## 🗺️ O Fluxo Operacional Completo (Ponta a Ponta)

```mermaid
flowchart TD
    subgraph INGESTAO ["1. Ingestão Autorizada & Higienização"]
        A1["Material Oficial do Cursinho<br>(Gran / Estratégia)"] --> A2["Download Padronizado<br>(Organização por Pastas de Aula)"]
        A2 --> A3["Tarjamento & Sanitização<br>(Remoção de CPF/Nome via PyMuPDF)"]
        A2 --> A4["Pipeline de Áudio & Legendas<br>(FFmpeg 16kHz + Whisper)"]
        A4 --> A5["Legenda Embutida MOV_TEXT no MP4<br>+ Aula XX - Transcrição.md"]
    end

    subgraph ESTRUTURACAO ["2. Banco de Questões Sem Distração"]
        B1["Questões Oficiais da Banca"] --> B2["Filtragem Temática Cirúrgica<br>(Disciplina + Assunto + Banca)"]
        B2 --> B3["Caderno de Questões Limpo<br>(Markdown / PDF para Resolução Cega)"]
        A3 & A5 & B3 --> B4["Índice Geral da Matéria<br>(Índice Geral - Disciplina.md)"]
    end

    subgraph MEMORIA ["3. Orquestração no NotebookLM (Live Sync)"]
        B4 --> C1["Google Drive Desktop"]
        C1 --> C2["Consulta ao SQLite do Drive<br>(Extração do Cloud ID Imutável)"]
        C2 --> C3["NotebookLM CLI (source add-drive)<br>(Vínculo Permanente sem Upload Estático)"]
    end

    subgraph COGNICAO ["4. O Ciclo Ultradiano MIT (90 Minutos)"]
        C3 --> D1["Min -5 a 0: Bússola da Banca (P07)"]
        D1 --> D2["Min 00-30: Dissecação Conceitual (P01 + FFCC da Matéria)"]
        D2 --> D3["Pausa Fisiológica (5 min sem telas)"]
        D3 --> D4["Min 35-55: Feynman Reverso às Cegas & Auditoria (P16)"]
        D4 --> D5["Pausa Fisiológica (5 min sem telas)"]
        D5 --> D6["Min 60-80: Active Recall sob Fadiga (P05/P06)"]
        D6 --> D7["Min 80-90: Kit de Consolidação & Repasse (P17)"]
        D7 --> D8["Importação Pipe-Delimited no Anki"]
    end
```

---

## 📚 Guias Operacionais Detalhados (`docs/`)

Para aprofundar em cada etapa técnica da engenharia de estudos, consulte os manuais específicos:

* 📄 **[Guia 01 — Preparação do Ambiente e Ingestão de Materiais](docs/01_preparacao_e_ingestao.md)**: Setup de pastas, Gran vs. Estratégia, extração de áudio mono 16kHz, transcrição com Whisper, embutimento de legendas `mov_text` em contêiner MP4 e tarjamento de dados pessoais.
* 🎯 **[Guia 02 — Banco de Questões por Tópico e Estudo Sem Distrações](docs/02_banco_questoes_sem_distracao.md)**: Como extrair questões por tópicos do edital, compilar em cadernos limpos em Markdown para resolução às cegas e auditar erros com a técnica dos *5-Whys*.
* ☁️ **[Guia 03 — Orquestração Google Drive & NotebookLM CLI](docs/03_orquestracao_drive_notebooklm.md)**: Por que nunca fazer upload manual de arquivos no navegador, como extrair os Cloud IDs persistentes do Google Drive e manter um *Live Sync* permanente.
* 🚀 **[Guia 04 — O Protocolo Diário de 90 Minutos (Ciclo Ultradiano MIT)](docs/04_guia_operacional_mit_90min.md)**: O roteiro minucioso minuto a minuto da sessão de estudo, regras de pausas sem tela, auditoria rígida de 5 pontos e consolidação biológica no sono NREM.

---

## 🧠 O Ciclo Ultradiano de 90 Minutos (Método MIT)

Em vez de resumos passivos que geram 83% de esquecimento após poucos minutos, a sessão é estruturada em blocos de alta fricção neural:

| Bloco | Tempo | Módulo N.A.G. | Ação Cognitiva e Comportamental |
| :--- | :--- | :--- | :--- |
| **Passo 4.0** | **-5 a 0 min** | **`P07` (Raio-X da Banca)** | Mapeia as tendências estatísticas, os 3 artigos mais cobrados e as cascas de banana da banca antes de abrir a aula. |
| **Bloco 1** | **00–30 min** | **`P01` + `FFCC`** | Identificação dos 5 conceitos centrais e decomposição da Lei Seca em tabelas estruturadas. **Sem cópia manual.** |
| *Pausa* | *5 min* | **Descompressão** | **Zero telas.** Água e caminhada curta para permitir alívio da memória de trabalho. |
| **Bloco 2** | **35–55 min** | **`P16` (Feynman Reverso)** | O NotebookLM faz a provocação técnica. O estudante redige a explicação **sem consultar notas**. A IA executa a **Auditoria Corretiva de 5 Pontos**. |
| *Pausa* | *5 min* | **Descompressão** | **Zero telas.** |
| **Bloco 3** | **60–80 min** | **`P05` / `P06`** | **Active Recall sob fadiga:** Resolução cega de questões e dissecação minuciosa de cada alternativa incorreta (*5-Whys*). |
| **Bloco 4** | **80–90 min** | **`P17` (Kit Consolidação)** | Geração automática da Folha Resumo (1 página), Tabela de Erros, Cronograma D+1..D+30 e bloco delimitado em `|` para o **Anki**. |

---

## 📑 A Biblioteca de Prompts de Elite (P01 a P18)

Cada arquivo em `prompts/` é um agente instrucional modular calibrado para o motor de raciocínio do NotebookLM:

| Código | Arquivo | Fase Pedagógica | Função Tática |
| :---: | :--- | :--- | :--- |
| **`P01`** | [`PROMPT_P01_DetalharAula.md`](prompts/PROMPT_P01_DetalharAula.md) | Compreensão | Dissecação profunda da aula, modelos mentais e Lei Seca estruturada em tabelas. |
| **`P02`** | [`PROMPT_P02_AnalisePreditiva.md`](prompts/PROMPT_P02_AnalisePreditiva.md) | Estratégia | Cruzamento preditivo entre a teoria da aula e o histórico da banca examinadora. |
| **`P03`** | [`PROMPT_P03_GarimpoBizus.md`](prompts/PROMPT_P03_GarimpoBizus.md) | Memorização | Mineração de mnemônicos, diferenciações conceituais finas e bizus de aprovação. |
| **`P04`** | [`PROMPT_P04_TutorTecnico.md`](prompts/PROMPT_P04_TutorTecnico.md) | Tutoria | Esclarecimento de dúvidas complexas através de questionamento socrático. |
| **`P05`** | [`PROMPT_P05_SimuladorQuestoes.md`](prompts/PROMPT_P05_SimuladorQuestoes.md) | Teste Ativo | Geração de questões inéditas de nível difícil no padrão exato da banca. |
| **`P06`** | [`PROMPT_P06_ResolucaoCirurgica.md`](prompts/PROMPT_P06_ResolucaoCirurgica.md) | Auditoria | Engenharia reversa de questões reais com dissecação de alternativas (*5-Whys*). |
| **`P07`** | [`PROMPT_P07_RaioX.md`](prompts/PROMPT_P07_RaioX.md) | Radar Prévio | Mapeamento do perfil estatístico da banca e armadilhas frequentes antes da aula. |
| **`P08`** | [`PROMPT_P08_SlidesExam.md`](prompts/PROMPT_P08_SlidesExam.md) | Auditoria | Confronto entre os pontos destacados em slides e o texto oficial da lei. |
| **`P09`** | [`PROMPT_P09_Flashcards.md`](prompts/PROMPT_P09_Flashcards.md) | Repetição | Criação de flashcards conceituais atômicos no formato Pergunta / Resposta. |
| **`P10`** | [`PROMPT_P10_QuizBanca.md`](prompts/PROMPT_P10_QuizBanca.md) | Simulação | Bateria rápida de múltipla escolha com temporizador e julgamento rígido. |
| **`P11`** | [`PROMPT_P11_Markmap.md`](prompts/PROMPT_P11_Markmap.md) | Visualização | Renderização da hierarquia da matéria em mapas mentais com sintaxe Markmap pura. |
| **`P12`** | [`PROMPT_P12_AulaGuiadaMapa.md`](prompts/PROMPT_P12_AulaGuiadaMapa.md) | Navegação | Roteiro estruturado de estudo conduzido através de nós de mapas conceituais. |
| **`P13`** | [`PROMPT_P13_MotorCognitivo.md`](prompts/PROMPT_P13_MotorCognitivo.md) | Diagnóstico | Avaliação de retenção e identificação de pontos cegos de memorização. |
| **`P14`** | [`PROMPT_P14_NarrarLei.md`](prompts/PROMPT_P14_NarrarLei.md) | Áudio/Voz | Roteiro para narração e memorização auditiva rítmica de artigos de lei. |
| **`P15`** | [`PROMPT_P15_QuizCompilado.md`](prompts/PROMPT_P15_QuizCompilado.md) | Simulado | Compilação de simulados temáticos com gabaritos detalhados e fundamentados. |
| **`P16`** | [`PROMPT_P16_FeynmanReverso.md`](prompts/PROMPT_P16_FeynmanReverso.md) | **[Método MIT]** | Explicação prática às cegas submetida à **Auditoria Corretiva de 5 Pontos**. |
| **`P17`** | [`PROMPT_P17_KitConsolidacao.md`](prompts/PROMPT_P17_KitConsolidacao.md) | **[Método MIT]** | Fechamento da sessão: Folha Resumo, Tabela de Erros, Cronograma e Anki CSV. |
| **`P18`** | [`PROMPT_P18_SintesePreditiva.md`](prompts/PROMPT_P18_SintesePreditiva.md) | **[Método MIT]** | Matriz acumuladora de armadilhas da banca para revisão de véspera de prova (D-1). |

---

## 🎯 Frameworks Analíticos por Disciplina (FFCC)

Para calibrar o olhar analítico da IA sem misturar critérios de áreas diferentes, carregue apenas a lente correspondente à disciplina estudada:

* [`FRAMEWORK_FFCC_JURIDICO.md`](frameworks/FRAMEWORK_FFCC_JURIDICO.md): Constitucional, Administrativo, Previdenciário e Legislação Institucional.
* [`FRAMEWORK_FFCC_TRIBUTARIO_ADUANEIRO.md`](frameworks/FRAMEWORK_FFCC_TRIBUTARIO_ADUANEIRO.md): Direito Tributário, Legislação Tributária e Aduaneira.
* [`FRAMEWORK_FFCC_CONTABIL.md`](frameworks/FRAMEWORK_FFCC_CONTABIL.md): Contabilidade Geral, Avançada, Custos, Auditoria e Pronunciamentos CPC/NBC.
* [`FRAMEWORK_FFCC_EXATAS.md`](frameworks/FRAMEWORK_FFCC_EXATAS.md): Raciocínio Lógico, Matemática Financeira e Estatística Descritiva/Inferencial.
* [`FRAMEWORK_FFCC_DADOS.md`](frameworks/FRAMEWORK_FFCC_DADOS.md): Fluência em Dados, Bancos Relacionais, SQL, Data Warehouse e Governança de TI.
* [`FRAMEWORK_FFCC_GESTAO.md`](frameworks/FRAMEWORK_FFCC_GESTAO.md): Administração Pública, Gestão de Pessoas, Materiais, Processos (BPM) e Projetos.

### Sintaxe de Execução Rápida no Chat:
```text
Use P01 com FFCC_TRIBUTARIO_ADUANEIRO para a Aula 03 - Imunidades Tributárias.
Use P16 com FFCC_CONTABIL para a Aula 04 - CPC 00 (Estrutura Conceitual).
Use P06 com FFCC_DADOS para a questão sobre Comandos DDL vs DML em SQL.
```

---

## 📊 Regra de Formatação Visual e Compatibilidade

Para garantir legibilidade absoluta em qualquer leitor moderno (**GitHub**, **Obsidian**, **Joplin**, **Typora**):
1. **Tabelas Nativas GFM Obrigatórias:** Comparações e matrizes utilizam barras verticais e alinhamentos (`| Coluna 1 | Coluna 2 |` e `| :--- | :--- |`). Caixas de texto em ASCII (`┌─┬─┐`) são proibidas.
2. **Diagramas Vetoriais em Mermaid.js:** Fluxogramas e linhas do tempo utilizam exclusivamente o padrão ` ```mermaid `.

---

## 🤝 Comunidade e Contribuições

Contribuições com novos frameworks por área, sugestões de automação de estudos e refinamento de prompts para bancas específicas são muito bem-vindas via *Pull Request* ou *Issues*.

Distribuído sob a licença **MIT**. Consulte [`LICENSE`](LICENSE) para mais informações.
