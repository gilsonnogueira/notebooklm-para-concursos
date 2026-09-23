# 🎯 Guia 02 — Banco de Questões por Tópico e Estudo Sem Distrações

A resolução de questões de provas anteriores da banca examinadora (FGV, Cebraspe, FCC, etc.) é o pilar central da preparação para concursos públicos de alto rendimento. Este guia descreve como estruturar um banco de questões limpo, categorizado por tópico do edital, ideal para resolução cega e sem interferências cognitivas.

---

## 1. As Questões dos Próprios PDFs das Aulas (Ponto de Partida Natural)

Antes de procurar qualquer fonte externa de questões, lembre-se: **os próprios PDFs de teoria (Estratégia e Gran) já vêm com uma lista extensa de questões comentadas ao final de cada aula**.

* **Por que isso é tão valioso?**
  * O professor já selecionou as questões mais representativas do tema.
  * Ao subir o PDF da aula no NotebookLM, a IA já tem acesso imediato a essa bateria de questões para traçar o **perfil estatístico de cobrança da banca**, mapear pegadinhas frequentes e entender o DNA do examinador sem que você precise fazer nada a mais.

---

## 2. Fornecendo Mais Questões ao NotebookLM (Filtro Cirúrgico)

Para matérias de peso elevado ou tópicos muito recorrentes, é altamente recomendável complementar o caderno com um volume maior de questões oficiais recentes.

Você pode extrair blocos de questões oficiais utilizando os filtros avançados das plataformas:
* **Filtros Essenciais:** `Disciplina` + `Assunto do Tópico` + `Banca Examinadora` + `Órgão/Cargo` + `Ano Mais Recente`.

### A. QConcursos: O Recurso Oficial de Impressão de Cadernos
No site do QConcursos, após aplicar os filtros desejados, você pode gerar um caderno limpo de questões utilizando o recurso nativo de impressão:

1. **Clique no ícone da Impressora** na barra superior da lista de questões:
   
   ![Ícone de Imprimir no QConcursos](assets/qc_botao_imprimir.png)

2. **Selecione a opção "Salvar como PDF" (Save as PDF)** no navegador:
   
   ![Salvar como PDF no diálogo de impressão](assets/qc_salvar_como_pdf.png)

* **Vantagem Imediata:** Você gera um documento PDF oficial, limpo, diagramado com enunciado e alternativas, perfeito para imprimir ou resolver no tablet/leitor digital sem nenhuma distração de comentários, curtidas ou fóruns.

---

### B. Sistemas Integrados de Questões (Estratégia Questões & Gran Questões)

Tanto o **Estratégia Concursos** quanto o **Gran Cursos Online** possuem plataformas integradas de questões completas incluídas nas assinaturas:

![Interface do Estratégia Questões](assets/estrategia_questoes_banco.png)

* **Estratégia Questões:** Permite criar cadernos e simulados filtrados por aula do curso ou tema do edital, com filtros avançados de banca, cargo e ano, além de opções de exportação.
* **Gran Questões:** Permite montar listas direcionadas por disciplina e assunto, acompanhar percentual de acerto e exportar simulados em formato limpo.

Ambos os ecossistemas permitem que o estudante monte baterias customizadas de 20 a 50 questões focadas estritamente na banca do concurso.

---

## 3. O Princípio da Fricção Cognitiva: Por que Estudar Sem Distrações?

A maioria dos candidatos comete um erro crítico ao resolver questões diretamente na tela:
1. Respondem a uma questão no site.
2. Em caso de dúvida ou erro, abrem imediatamente a aba de comentários antes mesmo de refletir sobre o motivo da falha.
3. Têm a sensação de aprendizado momentâneo (**ilusão de fluência**), mas esquecem a regra na semana seguinte porque não houve esforço neural de recuperação.

**A Abordagem N.A.G.:**
* O concurseiro resolve blocos de 15 a 20 questões em **silêncio cognitivo**, no papel ou em caderno digital limpo, simulando a pressão real do dia da prova.
* Apenas após concluir a bateria, os erros são auditados com profundidade.

---

## 4. O Fluxo de Trabalho com Questões

```mermaid
flowchart TD
    A["Questões da Própria Aula (PDF)<br>ou Caderno Filtrado (QC / Gran / Estratégia)"] --> B["Resolução Cega em Bloco<br>(Simulado no Papel ou Leitor Digital)"]
    B --> C["Identificação dos Erros e Dúvidas"]
    C --> D["Auditoria Cirúrgica no NotebookLM<br>(Prompt P06 - Análise dos 5-Whys)"]
    D --> E["Consolidação no Anki<br>(Prompt P17 - Cartão com a Causa do Erro)"]
```

---

## 5. Como Dissecar os Erros no NotebookLM (`P06`)

Quando você errar ou hesitar em uma questão do seu material, não recorra a explicações rasas. Invoque o `P06` no chat do caderno:

```text
Use P06 para a questão sobre Suspensão da Exigibilidade do Crédito Tributário.
```

O NotebookLM aplica a metodologia dos **5-Whys (Cinco Porquês)**:
1. **Identifica a Causa Raiz do Erro:** Mostra se a falha decorreu de distração na leitura ("pode" vs. "deve"), desconhecimento de prazo literal ou indução por pegadinha da banca.
2. **Dissecação das Alternativas Falsas:** Explica cirurgicamente por que cada item errado é incorreto.
3. **Ancoragem na Lei Seca:** Aponta o artigo de lei exato, súmula vinculante ou jurisprudência que encerra a controvérsia.

---

## 6. Caso Real: Cruzando a Teoria com o Acervo de Questões no NotebookLM

> [!TIP]
> **A REGRA DE OURO DO ACERVO DE QUESTÕES:**
> Quanto mais amplo, categorizado e atualizado for o acervo de questões disponibilizado no caderno, mais cirúrgica será a análise estatística e diagnóstica da IA.

Ao fornecer cadernos completos de questões (comentadas nos PDFs ou geradas pelas ferramentas oficiais do QC e Estratégia/Gran), o NotebookLM consegue calcular a incidência real da matéria, mapear a taxa de acerto da concorrência e traçar o DNA de cobrança específico de bancas como **Cebraspe, FGV e FCC**.

Veja a demonstração real completa com prints da interface e a resposta entregue pela IA em:
👉 **[`docs/07_exemplo_real_raio_x_questoes.md`](07_exemplo_real_raio_x_questoes.md)**.
