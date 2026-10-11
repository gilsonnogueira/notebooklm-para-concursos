---
type: source_prompt
id: P10
name: Quiz Interativo em 3 Níveis de Profundidade
version: 3.0
---

# 🎯 P10_QuizBanca

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Focado na geração de quizzes interativos com desafio progressivo em 3 níveis (Literalidade, Doutrina e Jurisprudência Aplicada), simulando a mente do examinador sênior.

<INSTRUCTION>
Ao ser invocado para o `P10_QuizBanca`:

1. ESTRUTURA DO DESAFIO PROGRESSIVO (3 NÍVEIS):
   Gere uma bateria de 3 a 5 questões organizadas em graus crescentes de complexidade cognitiva:
   - **Nível 1 (Básico / Literalidade):** Cobrança direta de artigo de lei, prazos e definições legais expressas.
   - **Nível 2 (Intermediário / Doutrina & Interpretação):** Cobrança de classificações, teorias e distinções conceituais.
   - **Nível 3 (Avançado / Caso Prático & Jurisprudência):** Situação hipotética com aplicação de Súmula Vinculante ou tese fixada pelos Tribunais Superiores.

2. SAÍDA EXIGIDA PARA CADA QUESTÃO:

```markdown
### 🧩 QUESTÃO [N] — [NÍVEL 1 / 2 / 3: TIPO DE COBRANÇA]

**Enunciado:**
[Enunciado completo no estilo da banca]

A) [Alternativa]
B) [Alternativa]
C) [Alternativa]
D) [Alternativa]
E) [Alternativa]

💡 **Dica do Examinador (Oculta/Para reflexão):** [Pista estratégica sobre o conceito em jogo]

<details>
<summary><b>🔍 Revelar Gabarito e Comentário</b></summary>

**Gabarito Oficial:** [Letra Correta]
- **Fundamentação:** [Base legal, artigo e jurisprudência]
- **Por que não são as outras:** [Erro objetivo de cada distrator]
- **Armadilha Evitada:** [A casca de banana embutida no enunciado]
</details>
```
</INSTRUCTION>
