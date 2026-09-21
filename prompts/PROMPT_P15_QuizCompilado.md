---
type: source_prompt
id: P15
name: Quiz de Compilados e Aulões
version: 1.0
---

# 🎯 P15_QuizCompilado

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Instrução para uso no Estúdio do NotebookLM. Analisa materiais compilados por tópicos/aulas (Degravações, Slides, Transcrições ou Originais de revisões como Treinamento Intensivo, Hora da Verdade, Reta Final), identifica a aula solicitada, isola todas as suas questões e gera um Quiz Interativo no Estúdio mantendo 100% da integridade do texto original.

<INSTRUCTION>
Ao ser invocado para gerar Quiz de Aula/Tópico Específico em Arquivo Compilado (`P15`):

1. LOCALIZAÇÃO E ANCORAGEM NO MATERIAL COMPILADO:
   - Consulte o arquivo indicado pelo usuário (ex: Degravação, Slides, Transcrição ou Original de Treinamento Intensivo, Reta Final, Hora da Verdade).
   - Analise o índice/sumário ou a estrutura interna do arquivo para localizar exatamente o bloco/tópico referente à aula solicitada (ex: "Aula 02 - Ilicitude e Culpabilidade").
   - Delimite o escopo estritamente do início ao fim dessa aula específica dentro do documento.

2. PRESERVAÇÃO RIGOROSA DA INTEGRIDADE DAS QUESTÕES (VERBATIM):
   - Identifique TODAS as questões pertencentes àquela aula.
   - PROIBIDO resumir, parafrasear ou alterar o enunciado ou as alternativas.
   - Mantenha o cabeçalho original da questão (Banca/Órgão/Ano, ex: `(FCC/TJ-AL/TÉCNICO JUDICIÁRIO/2024)`).
   - Preserve o enunciado completo e TODAS as alternativas de resposta originais (A, B, C, D, E).

3. RESTRIÇÕES DE INTERFACE DO QUIZ NO ESTÚDIO (DICA / HINT):
   - A interface de Quiz do Estúdio possui um campo de "Dica" (Hint).
   - PROIBIDO utilizar asteriscos (`**`) para negrito dentro do Hint.
   - Use APENAS ícones para estruturar e destacar a Dica:
     💡 [Pista sutil ou preceito chave para guiar o raciocínio. Máx. 2 linhas.]
     ⚠️ [Fundamento legal direto e alerta de armadilha/pegadinha. Máx. 2 linhas.]

4. CRIÇÃO OBRIGATÓRIA DE ARTEFATO NO ESTÚDIO:
   - Ao receber a aula (ex: "Aula 02 - Ilicitude e Culpabilidade" no arquivo "Treinamento Intensivo - Tópico 08 - Degravação.pdf"), processe a aula de forma autocontida sem truncamento.
   - Você DEVE gerar o resultado criando um novo ARTEFATO NO ESTÚDIO DO NOTEBOOKLM (Estúdio > App / Quiz Interativo).
   - PROIBIDO emitir as questões soltas no corpo do chat da conversa.

5. 🚫 PROIBIÇÃO ABSOLUTA DE MAPA MENTAL / MARKMAP:
   - PROIBIDO gerar sintaxe Markmap, YAML (`markmap:`), tags HTML `<span>`, listas com `<!-- fold -->` ou qualquer diagrama visual.
   - A resposta DEVE ser exclusivamente a criação de um Artefato de Quiz Interativo no Estúdio.
</INSTRUCTION>


