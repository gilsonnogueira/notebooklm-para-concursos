# 🧠 Arquitetura de Skills por Disciplina (`book-to-skill`)

> **Metodologia de Alta Performance para NotebookLM & Estudos de Concursos**  
> **Substitui definitivamente os antigos frameworks genéricos estáticos (FFCC) por Skills Especializadas e Modulares por Matéria.**

---

## 🎖️ Créditos e Reconhecimento

Esta arquitetura modular de Skills por Disciplina é fundamentada e adaptada diretamente da metodologia do projeto:

👉 **[virgiliojr94/book-to-skill](https://github.com/virgiliojr94/book-to-skill.git)** — *Criado por Virgílio Jr.*

O conceito central do `book-to-skill` é transformar qualquer fonte de conhecimento extensa (livros, manuais, apostilas e cursos preparatórios) em uma **Skill Cognitiva Atômica e Operacional**, permitindo que o NotebookLM ou qualquer agente de IA atue com o modelo mental do especialista e do examinador sobre aquela matéria específica.

---

## 🔄 Por que Substituir os Antigos Frameworks Estáticos (FFCC)?

| Aspecto | Frameworks Antigos (FFCC) | Skills por Disciplina (`book-to-skill`) |
| :--- | :--- | :--- |
| **Escopo** | Genérico (6 grandes áreas fixas). | **Atômico por matéria** (Tributário, Constitucional, TI, Contabilidade, etc.). |
| **Alinhamento ao Edital** | Abstrato, sem tópicos específicos. | **100% ancorado nos eixos e tópicos do edital** do concurso. |
| **Instrumentos de Apoio** | Apenas 4 quadrantes conceituais. | **Cheatsheet (fórmulas/prazos), Patterns (bancas), Glossário e Capítulos.** |
| **Psicologia da Banca** | Menções pontuais. | **Mapeamento de vícios, distratores e pegadinhas reais da banca.** |
| **Manutenção e Expansão** | Arquivos rígidos de difícil adaptação. | **Modular, expansível e gerável a partir de qualquer material.** |

---

## 🏛️ Anatomia Canônica de uma Skill (`book-to-skill`)

Cada disciplina é representada por uma estrutura modular padronizada:

```text
skills/
└── nome-da-disciplina/
    ├── SKILL.md            # DNA da matéria, eixos do edital, modelos mentais e catálogo
    ├── cheatsheet.md       # Fórmulas, tabelas de prazos, mnemônicos e distinções rápidas
    ├── patterns.md         # Padrões da banca, armadilhas frequentes e taxa de incidência
    ├── glossary.md         # Termos técnicos, léxico em latim e definições canônicas
    └── chapters/           # Dissecação modular por tópico/capítulo do edital
        ├── topico_01_nome.md
        ├── topico_02_nome.md
        └── ...
```

### Componentes Principais:

1. **`SKILL.md` (Arquivo Central de Injeção):**
   - Frontmatter YAML com metadados da disciplina.
   - Visão geral e alinhamento com os eixos temáticos do concurso.
   - Modelos mentais do examinador para a disciplina.
   - Protocolos cognitivos integrados (`P01` a `P20`).
   - Mapeamento das fontes carregadas no caderno do NotebookLM.

2. **`cheatsheet.md` (Resumo Tático de Reta Final):**
   - Prazos decadenciais, prescricionais e processuais.
   - Fórmulas matemáticas, lançamentos contábeis ou comandos de banco de dados.
   - Tabelas comparativas de institutos facilmente confundidos.
   - Mnemônicos com pergunta-gatilho de prova.

3. **`patterns.md` (Raio-X da Banca Examinadora):**
   - Perfil da banca examinadora (Cebraspe, FGV, FCC, etc.) para aquela disciplina.
   - Os 5 principais vetores de distorção de enunciados.
   - Matriz Gravidade / Tendência / Frequência dos tópicos.

4. **`glossary.md` (Léxico da Disciplina):**
   - Definições literais e canônicas para evitar alucinações terminológicas.

---

## 🔀 Como Utilizar no NotebookLM (Sintaxe em Duas Camadas)

Para orquestrar suas sessões de estudo com a máxima densidade, combine o **Prompt Operacional de Saída (`PXX`)** com a **Skill da Disciplina**:

```text
Use [PROMPT_PXX] com [SKILL_<DISCIPLINA>] para [TÓPICO / CONCEITO].
```

### Exemplos Práticos:

* **Direito Tributário:**
  ```text
  Use P01 com a Skill de Direito Tributário para o Tópico 03 - Tributos Municipais (IPTU, ITBI e ISSQN).
  ```

* **Contabilidade Geral e Custos:**
  ```text
  Use P06 com a Skill de Contabilidade para a questão sobre Demonstração dos Fluxos de Caixa (Método Indireto).
  ```

* **Fluência em Dados / Informática:**
  ```text
  Use P02 com a Skill de Tecnologia e Dados para o Tópico de Window Functions e Subqueries em SQL.
  ```

* **Direito Administrativo:**
  ```text
  Use P16 com a Skill de Direito Administrativo para o tema de Atos Administrativos e Teoria dos Motivos Determinantes.
  ```

* **Reta Final e Revisão Acumulada:**
  ```text
  Use P18 com a Skill de Legislação de Trânsito para gerar a Matriz de Armadilhas do CTB.
  ```

---

## 🛠️ Como Criar uma Nova Skill para a sua Disciplina

Para converter um livro digital, apostila ou módulo do seu cursinho em uma skill oficial, utilize o arquivo modelo [`TEMPLATE_SKILL_DISCIPLINA.md`](TEMPLATE_SKILL_DISCIPLINA.md) disponível nesta pasta.
