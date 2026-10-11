---
type: source_prompt
id: P09
name: Flashcards Atômicos e Cloze para Anki
version: 4.0
---

# 🗂️ P09_Flashcards

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Focado na geração de Flashcards de memorização ativa (Active Recall) com granularidade atômica, compatíveis tanto com o Estúdio do NotebookLM quanto com importação direta no Anki.

<INSTRUCTION>
Ao ser invocado para gerar Flashcards (`P09`):

1. PRINCÍPIO DA ATOMICIDADE ESTRITA (1 FATO = 1 CARD):
   - Cada flashcard DEVE testar apenas uma única informação, prazo, artigo ou exceção isolada.
   - NUNCA crie perguntas que exijam listar 4 ou 5 requisitos de uma vez (gera sobrecarga cognitiva e bloqueio na revisão).

2. SINTAXE DUPLA SUPORTADA:
   - Forneça os flashcards em dois formatos integrados:
     - **Formato A: Pergunta Direta Atômica (Frente / Verso)**
     - **Formato B: Oclusão de Texto (Cloze Deletion `[...]`)** ideal para prazos, verbos e competências.

3. ⚠️ RESTRIÇÕES CRÍTICAS DE INTERFACE E EXPORTAÇÃO:
   - PROIBIDO usar asteriscos (`**`) para negrito dentro do texto exportável do Estúdio.
   - O único uso de colchetes permitido na Pergunta é para indicar a lacuna de oclusão `[...]`.
   - PROIBIDO usar parênteses desnecessários ou rótulos artificiais como "Frente:", "Verso:".

4. FORMATO DE SAÍDA EXIGIDO:

```text
CARD [N] - [TIPO: DIRETO ou CLOZE]
[Pergunta Atômica Direta OU Frase com Lacuna [...]]
---
[Resposta Objetiva Direta com Artigo/Súmula]
⚠️ Pegadinha: [Atenção ao detalhe que a banca troca]
📊 Risco de Prova: [Alto / Médio / Crítico]
```

5. BLOCO ADICIONAL PARA IMPORTAÇÃO NO ANKI (TAB-DELIMITED):
Ao final da lista, gere um bloco de código de texto puro separado por ponto-e-vírgula ou tabulação (`Pergunta;Resposta;Tag`) para que o estudante possa copiar e colar direto no Anki via importação de arquivo de texto.
</INSTRUCTION>
