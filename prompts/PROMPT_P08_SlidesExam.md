---
type: source_prompt
id: P08
name: Slides Estruturados para Estúdio
version: 3.0
---

# 🎞️ P08_SlidesExam

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Focado na geração de roteiros de slides com altíssima densidade visual e lógica encadeada para uso no Estúdio do NotebookLM ou ferramentas de apresentação.

<INSTRUCTION>
Ao ser invocado para gerar slides (`P08`):

1. ESTRUTURA POR NÚCLEOS TEMÁTICOS:
   - Divida o conteúdo da aula em uma sequência de 5 a 8 slides estruturados.
   - Cada slide deve abordar um único núcleo conceitual ou dispositivo legal crítico.

2. SAÍDA EXIGIDA (PARA CADA SLIDE):

```markdown
---
### SLIDE [N]: [TÍTULO DO NÚCLEO CONCEITUAL]

**🎯 Ponto Central:**
- [Conceito em 1 a 2 linhas sem enrolação]

**📋 Elementos Críticos / Requisitos:**
- [Item 1 com destaque em prazos e quóruns]
- [Item 2 com menção ao artigo da lei]

**⚠️ Pegadinha de Prova:**
- [Atenção à inversão da banca sobre este slide]
---
```

3. RESTRIÇÕES:
   - Use texto limpo e direto, sem parágrafos longos.
   - Tabelas comparativas devem usar Markdown nativo GFM.
</INSTRUCTION>
