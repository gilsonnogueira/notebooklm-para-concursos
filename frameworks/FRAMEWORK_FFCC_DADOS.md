---
type: framework
id: FFCC_DADOS
name: Framework FFCC Fluência em Dados e Tecnologia Fiscal
version: 1.0
---

# 💻 FRAMEWORK FFCC: FLUÊNCIA EM DADOS & TECNOLOGIA
## Espinha Dorsal Analítica para Bancos de Dados, SQL, Ciência de Dados e Governança

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Este framework é a lente analítica obrigatória para dissecar questões e conceitos de **Fluência em Dados**, **Bancos de Dados Relacionais e Não-Relacionais (NoSQL)**, **SQL**, **Data Warehouse / Big Data / ETL**, **Python / R** e **Governança de Dados (LGPD/DAMA-DMBOK)**.
> Todo conceito ou script deve ser estruturado nos 4 quadrantes abaixo:

---

## 1. FORM (Forma) — Sintaxe, Notação e Modelagem Estrutural
*A representação sintática e a arquitetura formal dos dados.*
- **Sintaxe Formal / Comandos:**
  - *SQL:* `SELECT`, `FROM`, `WHERE`, `GROUP BY`, `HAVING`, `ORDER BY`, `WINDOW FUNCTIONS` (`OVER (PARTITION BY ... ORDER BY ...)`).
  - *Comandos DDL vs. DML vs. DQL vs. DCL vs. TCL.*
- **Modelagem Conceitual e Lógica:**
  - Diagrama Entidade-Relacionamento (DER), cardinalidades (1:1, 1:N, N:N).
  - Esquema Dimensional: Modelo Estrela (*Star Schema*) vs. Floco de Neve (*Snowflake Schema*). Tabelas Fato vs. Dimensão.

---

## 2. FUNCTION (Função) — Propósito da Operação & Papel na Auditoria Fiscal
*A utilidade da instrução técnica e o objetivo analítico.*
- **Objetivo da Consulta / Pipeline:**
  - Extração, Carga e Transformação (ETL/ELT).
  - Identificação de fraudes, triangulações de notas fiscais (SPED) ou inconsistências tributárias em grandes volumes de dados.
- **Paradigma de Armazenamento:**
  - OLTP (processamento transacional diário, normalizado) vs. OLAP (processamento analítico, desnormalizado, Data Warehouse).
  - Governança: Garantia de privacidade (LGPD: bases legais, anonimização, titular de dados) e qualidade dos dados (DAMA-DMBOK).

---

## 3. CONTENT (Conteúdo) — Operadores, Parâmetros e Complexidade de Execução
*Os detalhes técnicos, regras de junção e métricas de desempenho.*
- **Álgebra Relacional e Junções (JOINs):**
  - Diferença estrita de retorno: `INNER JOIN`, `LEFT OUTER JOIN`, `RIGHT OUTER JOIN`, `FULL OUTER JOIN` e `CROSS JOIN`.
  - Tratamento de valores nulos (`NULL`) em agregações (`COUNT(*)`, `COUNT(coluna)`, `SUM()`, `AVG()`).
- **Normalização de Dados:**
  - 1FN (valores atômicos, sem atributos multivalorados).
  - 2FN (1FN + dependência funcional total da chave primária).
  - 3FN (2FN + ausência de dependência transitiva).
- **Métricas de Aprendizado de Máquina (Machine Learning):**
  - Matriz de Confusão: Verdadeiro Positivo, Falso Positivo, Falso Negativo, Verdadeiro Negativo.
  - Acurácia, Precisão, Sensibilidade/Recall, F1-Score e Curva ROC / AUC.

---

## 4. CONTEXT (Contexto) — Comportamento de Execução & Armadilhas FGV
*O resultado exato da consulta e as pegadinhas clássicas do examinador.*
- **Padrão de Armadilha FGV em SQL:**
  - Questões que mostram duas tabelas com 5 linhas e pedem o número exato de linhas retornadas após um `LEFT JOIN` com `WHERE` filtrando a tabela da direita (convertendo o `LEFT JOIN` em `INNER JOIN` disfarçado).
  - Uso de cláusula `WHERE` em vez de `HAVING` para filtrar funções agregadas (gera erro de compilação SQL).
  - Diferença entre `RANK()`, `DENSE_RANK()` e `ROW_NUMBER()`.
- **Interpretação Semântica:** Como a ordem física de execução no motor difere da ordem escrita (`FROM` ➔ `WHERE` ➔ `GROUP BY` ➔ `HAVING` ➔ `SELECT` ➔ `ORDER BY` ➔ `LIMIT`).
