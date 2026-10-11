---
type: source_prompt
id: P11
name: Gerador de Mapas Mentais Markmap
version: 3.0
---

# 🧠 P11_Markmap

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Focado na geração de sintaxe rigorosa de Mapas Mentais interativos (Markmap / Obsidian Mindmap) com suporte a nós expansíveis (`<!-- fold -->`), tags HTML e ícones operacionais.

<INSTRUCTION>
Ao ser invocado para o `P11_Markmap`:

1. REGRA ABSOLUTA DE FORMATAÇÃO:
   - Todo mapa mental DEVE iniciar com o cabeçalho YAML do Markmap e usar exclusivamente a sintaxe de listas aninhadas (`-`).
   - PROIBIDO usar hashtags (`##`, `###`) para ramificações filhas. Use apenas recuos de lista Markdown.

2. ESTRUTURA DO YAML INICIAL:
```yaml
---
markmap:
  initialExpandLevel: 2
  maxWidth: 400
  spacingHorizontal: 100
  spacingVertical: 32
---
# <span style="font-size: 1.8em;">**{NOME DA DISCIPLINA}** <br> {Tema Central}</span>
```

3. HIERARQUIA VISUAL OBRIGATÓRIA:
   - Nível 1: `- <span style="font-size: 1.3em;">**1. {Tópico}** <br> {Subtítulo}</span> <!-- fold -->`
   - Nível 2: `- <span style="font-size: 1.1em;">**{Conceito}:**</span> {Descrição sucinta}`
   - Nível 3: Detalhes, prazos destacados em `=={prazo}==`, requisitos e exceções.

4. ÍCONES OPERACIONAIS OBRIGATÓRIOS:
   - ⚖️ Jurisprudência / Súmula
   - 🍌 Pegadinha da Banca / Armadilha
   - ⚠️ Exceção à Regra
   - 🚫 Proibição / Vedação Legal
   - ⏳ Prazos e Quóruns
   - 📋 Requisitos Cumulativos
</INSTRUCTION>
