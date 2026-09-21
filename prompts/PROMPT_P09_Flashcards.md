---
type: source_prompt
id: P09
name: Flashcards Active Recall
version: 2.0
---

# 🗂️ P09_Flashcards

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Instrução para uso no Estúdio do NotebookLM. Gera cartões atômicos de memorização ativa com altíssimas restrições de sintaxe.

<INSTRUCTION>
Ao ser invocado para gerar Flashcards (`P09`):

1. ESCOPO ATÔMICO:
   - Cada cartão deve testar apenas um detalhe, prazo ou requisito isolado.
   - Varie os formatos: Oclusão (Cloze com `[...]`), Afirmativas para julgamento (C/E), minicasos de duas linhas ou perguntas diretas.

2. ⚠️ RESTRIÇÕES CRÍTICAS DE INTERFACE (PROIBIÇÕES ABSOLUTAS):
   - PROIBIDO usar asteriscos (`**`) para negrito na saída. A interface do Estúdio não renderiza.
   - PROIBIDO usar colchetes `[ ]` na Face da Resposta.
   - PROIBIDO usar parênteses `( )` para envolver texto na Face da Resposta.
   - O ÚNICO uso de colchetes permitido é para indicar a lacuna `[...]` na Face da Pergunta.
   - PROIBIDO usar os rótulos textuais "Frente", "Verso", "Pergunta", "Resposta".

3. ANATOMIA EXIGIDA DA RESPOSTA:
A face da resposta deve ser limpa e seguir esta ordem exata:
- Resposta objetiva direta - Fundamentação legal curta.
- ⚠️ [Pegadinha explicada baseada nos comentários dos alunos]
- 📊 Nível [Alto/Médio/Baixo, inferido do índice de erros]
</INSTRUCTION>
