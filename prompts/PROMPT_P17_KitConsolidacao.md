---
type: source_prompt
id: P17
name: Kit de Repasse e Consolidação (Método MIT)
version: 1.0
---

# 📦 P17_KitConsolidacao (Método MIT — Fechamento da Sessão de 90 Minutos)

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Este arquivo é acionado nos últimos 10 minutos da sessão ultradiana (minuto 80 a 90). Ele audita todo o histórico da sessão de estudos e gera o **Kit Oficial de Repasse e Consolidação**, desenhado para blindar o conhecimento contra a Curva do Esquecimento de Ebbinghaus e alimentar sistemas de repetição espaçada (Anki).

<INSTRUCTION>
Ao ser invocado pelo comando `P17` ou `P17 [Tópico/Aula]`:

Varra todo o histórico da sessão recente e as fontes do caderno para produzir ESTRITAMENTE os 5 artefatos estruturados abaixo, sem saudações e sem introduções prolixas:

---

## 📄 ARTEFATO 1: FOLHA RESUMO CIRÚRGICA (Máx. 1 Página)
- **PROIBIDO GERAR RESUMO GENÉRICO:** Sintetize unicamente:
  - Os **5 Conceitos Centrais** que sustentam o tema.
  - As lacunas exatas e falhas conceituais que o aluno cometeu durante o teste de Feynman (`P16`) ou nas questões de raciocínio.
  - As regras de exceção e prazos que não podem ser esquecidos.

---

## 📊 ARTEFATO 2: TABELA DE ERROS TÍPICOS E CONFUSÃO COGNITIVA
Estruture uma tabela Markdown comparando o erro com a regra correta:

| Erro / Pegadinha Típica da Banca | Conduta / Interpretação Correta | Fundamentação Legal / Jurisprudencial | Fonte no Caderno (Página / Vídeo) |
|---|---|---|---|
| [O que o candidato errou ou o que a banca induz] | [A regra exata e aplicação correta] | [Art. X da Lei Y ou Súmula Z] | [Ex: Aula 02 - Original.pdf, p. 18] |

---

## 🎯 ARTEFATO 3: 10 QUESTÕES DE REVISÃO ALVO (Prática Intercalada)
- Gere 10 novas questões curtas e densas (estilo Certo/Errado ou Múltipla Escolha com foco cirúrgico), ordenadas por dificuldade crescente (Básico → Intermediário → Especialista).
- As questões DEVEM focar exclusivamente nos calcanhares de Aquiles detectados na sessão.
- Forneça o gabarito comentado apenas ao final de todas as 10 questões, em bloco colapsado ou recuado.

---

## 📅 ARTEFATO 4: CRONOGRAMA DE 7 A 30 DIAS (Repetição Espaçada / FSRS)
Indique a cadência ótima de reativação neural com base na retenção desejada (10% a 20% do horizonte até a prova):

- **D+1 (Amanhã - 10 min):** Resolver as 5 primeiras questões do Artefato 3 sem olhar notas.
- **D+3 (3 dias - 15 min):** Explicar os 5 conceitos centrais em voz alta (Feynman puro) e checar a Tabela de Erros.
- **D+7 (7 dias - 20 min):** Resolver as 5 questões restantes do Artefato 3 e refazer questões da banca no QConcursos.
- **D+21 (Revisão Mensal - 15 min):** Rodar flashcards do Anki gerados no Artefato 5.

---

## 🗂️ ARTEFATO 5: BLOCO DE FLASHCARDS DELIMITADO PARA O ANKI (CSV)
Gere um bloco de código contendo cards atômicos de pergunta e resposta separados rigorosamente pelo delimitador `|` (pipe), prontos para importação direta no Anki:

```text
Pergunta frontal clara (Active Recall) | Resposta no verso com fundamentação exata e dispositivo legal
[Pergunta sobre distinção ou pegadinha] | [Resposta direta sem rodeios + Art. X]
```

- **Regra dos Cards:** Mínimo de 10 e máximo de 20 cards atômicos. Proibido cards longos ou vagos. Devem conter apenas lacunas reais, prazos, exceções e os erros mapeados no Artefato 2.

---

### REGRAS FINAIS DE EXECUÇÃO:
- **Zero Ruído:** Inicie imediatamente no título `## ARTEFATO 1`.
- **Encerramento no Ponto Final:** Conclua no fechamento do bloco de código do Anki, sem mensagens adicionais.
</INSTRUCTION>
