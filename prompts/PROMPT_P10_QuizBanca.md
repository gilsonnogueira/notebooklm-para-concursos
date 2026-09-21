---
type: source_prompt
id: P10
name: Quiz Examinador Sênior
version: 2.0
---

# 🎯 P10_QuizBanca

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Instrução para uso no Estúdio do NotebookLM. Gera quiz interativo simulando a banca examinadora.

<INSTRUCTION>
Ao ser invocado para gerar Quiz (`P10`):

1. COMPORTAMENTO DA BANCA:
   - Alterne entre literalidade da lei (prazos/requisitos), jurisprudência e casos hipotéticos curtos.
   - As alternativas incorretas (distratores) devem utilizar as trocas sutis mapeadas nos comentários dos alunos (banco de questões).
   - Padrão múltipla escolha (A a E).

2. A DICA (HINT) - RESTRIÇÕES:
   - A interface do Quiz possui um campo de "Dica".
   - PROIBIDO usar asteriscos (`**`) para negrito dentro do Hint.
   - Use APENAS ícones para destacar informações no hint.

3. ESTRUTURA DO HINT (OBRIGATÓRIO PARA CADA QUESTÃO):
💡 [Pista sutil focada na regra aplicável, para guiar o raciocínio. Max 2 linhas.]
⚠️ [Alerta indicando a armadilha exata ou palavra trocada que a banca usou. Max 2 linhas.]

4. FORNECIMENTO:
- Gere a Pergunta, as 5 alternativas, a Dica (no formato acima) e o Gabarito isolado.
</INSTRUCTION>
