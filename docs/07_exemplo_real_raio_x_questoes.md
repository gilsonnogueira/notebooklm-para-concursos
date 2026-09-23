# 🔬 Caso Real: Raio-X de Incidência e DNA da Banca a partir do Acervo de Questões

Este documento apresenta uma **demonstração prática real** de como o **Google NotebookLM** processa e cruza a teoria de uma aula com um **acervo qualificado de questões de concursos anteriores**. 

O caso reproduz uma consulta realizada durante a preparação para o concurso de **Auditor Fiscal (ISS Aracati)**, na disciplina de **Administração Financeira e Orçamentária (AFO)**.

---

## 💡 A Regra de Ouro do Acervo de Questões

> [!IMPORTANT]
> **QUANTO MAIS ROBUSTO E COMPLETO FOR O SEU ACERVO DE QUESTÕES, MAIS CIRÚRGICA SERÁ A RESPOSTA DA IA:**
> 
> O NotebookLM não se baseia em "achismos" ou médias soltas da internet. Ele opera estritamente ancorado nos arquivos fornecidos.
> 
> Quando você alimenta o caderno com um **acervo representativo de questões** (seja extraindo os blocos de questões comentadas dos próprios PDFs teóricos do seu cursinho, seja gerando cadernos direcionados em PDF pelos recursos oficiais do QConcursos, Gran ou Estratégia Questões com filtros de banca, disciplina e ano), a IA consegue:
> 1. **Calcular a Incidência Estatística Real:** Identificar exatamente a porcentagem do tema em relação ao histórico da matéria (ex: *59,4% de todo o acervo de AFO*).
> 2. **Medir a Taxa de Acerto da Concorrência:** Diagnosticar o índice médio de acerto (ex: *77,6%*) e enquadrar o assunto na matriz tática (*Quadrante A - Garantidores de Pontos: proibido errar*).
> 3. **Dissecar o DNA Específico de Cada Banca:** Mostrar como Cebraspe, FGV, FCC e bancas regionais cobram o mesmo artigo de maneiras completamente distintas.

---

## 📸 A Interface em Ação no NotebookLM

Abaixo vemos a tela do caderno em produção no Gemini Notebook, com a consulta disparada e a análise sendo entregue com ancoragem em fontes reais:

![Consulta de Raio-X de Questões no NotebookLM](assets/exemplo_real_raio_x_questoes.png)

---

## 💬 A Consulta Disparada no Chat

O estudante solicitou o cruzamento da **Aula 00** com o banco de dados de questões e relatórios empíricos de provas anteriores:

```text
Focando na Aula 00, me diga como isso é cobrado em provas. Use como referência:
- 01 - Orçamento Público em AFO.pdf
- Relatório Analítico de AFO - Como a Matéria é Cobrada.md
- Raio-X de AFO - Análise Empírica por Banca (Fonte NLM).md
```

*(No padrão N.A.G. de comandos rápidos, essa mesma requisição equivale a: `Use P07 para a Aula 00 cruzando a teoria com o acervo de questões`).*

---

## 📑 Resposta Técnica Completa Entregue pelo NotebookLM

Abaixo está a resposta exata e integral gerada pelo modelo:

# ANÁLISE DE INCIDÊNCIA E PADRÃO DE COBRANÇA EM PROVAS — AULA 00 (ORÇAMENTO PÚBLICO: PPA, LDO E LOA)

### 1. DADOS ESTATÍSTICOS E PESO RELATIVO NO CONCURSO
* **Carro-Chefe da Disciplina:** O tema **Orçamento Público (PPA, LDO e LOA)** é o assunto mais cobrado em AFO, correspondendo a **59,4% de todo o acervo de questões** da matéria (840 questões em uma amostra representativa de 1.415 questões de provas recentes).
* **Índice de Acerto e Enquadramento Estratégico:** A taxa média de acerto dos candidatos situa-se em **77,6%**. Na matriz de planejamento estratégico, enquadra-se no **Quadrante A (Garantidores de Pontos)**: por ter alto volume e taxa de acerto elevada pela concorrência, o candidato não pode errar nenhuma questão deste bloco sob pena de perda imediata de posições.
* **Espécie Normativa Padrão:** As bancas cobram sistematicamente o fato de PPA, LDO e LOA serem **leis ordinárias** (aprovadas por maioria simples), e não leis complementares.

---

### 2. MAPEAMENTO POR BANCA EXAMINADORA (DNA DAS BANCAS DE CONCURSO)

#### A. CESPE / CEBRASPE
* **Foco Principal:** Letra seca dos artigos 165 a 169 da CF/88 combinada com dispositivos da LRF (LC nº 101/2000) e jurisprudência do STF.
* **Modo de Cobrança:** Questões de Certo/Errado exigindo o domínio literal das competências e vedações orçamentárias:
  * Exige a diferenciação precisa entre as funções de cada peça.
  * Explora a desconexão temporal do PPA (vigência de 4 anos iniciando no 2º ano do mandato).
  * Explora a obrigatoriedade do Anexo de Metas Fiscais e do Anexo de Riscos Fiscais na LDO.
* **Pegadinha Clássica:** Trocar atribuições do Anexo de Metas Fiscais (parâmetros e metas anuais de receitas/despesas/dívida) pelo Anexo de Riscos Fiscais (passivos contingentes), ou afirmar que o PPA é dispensado pela LOA no primeiro ano.

#### B. FGV (Fundação Getulio Vargas)
* **Foco Principal:** **Estudos de caso hipotéticos e situações práticas operacionais**.
* **Modo de Cobrança:** Narrativas longas apresentando prefeitos, governadores ou secretários municipais/estaduais em dilemas de planejamento:
  * Teste de compatibilidade entre as leis: emenda à LDO exige compatibilidade única com o PPA; emenda à LOA exige compatibilidade simultânea com o PPA e a LDO.
  * Situações de perda de prazo no envio de propostas orçamentárias por Poderes autônomos (Judiciário/MP), ativando a consolidação pelo Executivo com base na LOA vigente ajustada pela LDO (art. 99, § 4º da CF).
* **Pegadinha Clássica:** Inverter a hierarquia material, afirmando que a LDO pode modificar diretrizes do PPA em elaboração no mesmo exercício.

#### C. FCC (Fundação Carlos Chagas)
* **Foco Principal:** Literalidade constitucional estrita, classificação das estatais na LOA e detalhamento das exceções aos princípios.
* **Modo de Cobrança:** Cobrança detalhada sobre a tripartição orçamentária da LOA (art. 165, § 5º):
  * Alocação de **empresas estatais dependentes** no Orçamento Fiscal ou da Seguridade Social, reservando o Orçamento de Investimento **exclusivamente para as estatais não dependentes**.
  * Exigência literal da função do Orçamento Fiscal e do Orçamento de Investimento de **reduzir as desigualdades inter-regionais** segundo o critério populacional (art. 165, § 7º).

#### D. BANCAS DIVERSAS (IDECAN, VUNESP, FUNDATEC, INSTITUTO AOCP, LEGALLE)
* **Foco Principal:** Mapeamento de termos correlatos e tabela de associação direta de funções.
* **Regra de Decodificação em Provas:**
  * Falou em *"Diretrizes, Objetivos e Metas (DOM)"*, *"Regionalizado"*, *"Despesas de Capital"* e *"4 anos"* $\rightarrow$ **Plano Plurianual (PPA)**.
  * Falou em *"Metas e Prioridades"*, *"Orienta a LOA"*, *"Elo de Ligação"*, *"Alterações na Legislação Tributária"* e *"Anexo de Metas/Riscos Fiscais"* $\rightarrow$ **Lei de Diretrizes Orçamentárias (LDO)**.
  * Falou em *"Estima Receitas e Fixa Despesas"*, *"Exercício Financeiro (1 ano)"*, *"Orçamento Fiscal, Seguridade e Investimento"* e *"Exclusividade"* $\rightarrow$ **Lei Orçamentária Anual (LOA)**.

---

### 3. AS 6 ARMADILHAS/PEGADINHAS MAIS FREQUENTES DAS BANCAS

| Armadilha | O Erro Induzido pela Banca nas Questões | A Regra Técnica Correta |
| :--- | :--- | :--- |
| **1. Troca de Funções das Peças** | Afirmar que a LDO fixa despesas, ou que o PPA estima receitas, ou que a LOA define objetivos regionais de 4 anos. | PPA planeja (DOM / 4 anos); LDO orienta e define metas anuais; LOA estima receita e fixa despesa anual. |
| **2. Reserva de Lei Complementar** | Afirmar que PPA, LDO e LOA são aprovados por Lei Complementar (maioria absoluta). | PPA, LDO e LOA são **leis ordinárias** (maioria simples). Apenas as normas gerais de prazos e vigência do art. 165, § 9º exigem LC. |
| **3. Enquadramento de Estatais na LOA** | Incluir todas as empresas estatais no Orçamento de Investimento das Estatais. | Estatais **dependentes** integram o **Orçamento Fiscal ou da Seguridade Social**. O Orçamento de Investimento é restrito às estatais **não dependentes**. |
| **4. Redução de Desigualdades (Art. 165, § 7º)** | Afirmar que o Orçamento da Seguridade Social tem a função de reduzir desigualdades inter-regionais. | A função de reduzir desigualdades inter-regionais cabe **exclusivamente ao Orçamento Fiscal e ao Orçamento de Investimento**. |
| **5. Exceções à Exclusividade (Art. 165, § 8º)** | Afirmar que a LOA pode conter autorização para abertura de "créditos especiais" ou "créditos extraordinários". | A ressalva constitucional autoriza **apenas créditos suplementares** e **contratação de operações de crédito (inclusive ARO)**. |
| **6. Troca de Anexos da LRF na LDO** | Afirmar que o Anexo de Riscos Fiscais fixa as metas anuais de resultado primário e dívida pública. | **Metas anuais** (receitas, despesas, primário, nominal e dívida) constam no **Anexo de Metas Fiscais**. Riscos e passivos contingentes constam no **Anexo de Riscos Fiscais**. |

---

### 4. MATRIZ SÍNTESE PARA RESOLUÇÃO RÁPIDA DE QUESTÕES

* **PPA** $\rightarrow$ **P-L-A-N-E-J-A** $\rightarrow$ D-O-M (Diretrizes, Objetivos, Metas) \| 4 Anos \| Despesas de Capital e Continuadas.
* **LDO** $\rightarrow$ **L-I-G-A** $\rightarrow$ M-P (Metas e Prioridades) \| Orienta a LOA \| Regra do Recesso (17/07).
* **LOA** $\rightarrow$ **E-X-E-C-U-T-A** $\rightarrow$ Estima Receita / Fixa Despesa \| 1 Ano \| Tripartição (Fiscal, Seguridade, Investimento).

* **Regra de Ouro dos Investimentos Plurianuais (Art. 167, § 1º):** Nenhum investimento cuja execução ultrapasse um exercício financeiro pode ser iniciado sem prévia inclusão no PPA (ou lei que autorize), sob pena de **crime de responsabilidade**.
* **Regra de Ouro do Recesso Parlamentar (Art. 57, § 2º):** A sessão legislativa de julho **não será interrompida** sem a aprovação do projeto de **LDO** (a vedação não se aplica ao PPA nem à LOA).
---

## 🎯 Parte 2: Investigação do Perfil da Banca Específica (FCPC) e Mapa Global da Disciplina

Neste segundo momento, o estudante explora o acervo para além de uma única aula: ele questiona o NotebookLM sobre a **banca organizadora específica do certame (FCPC / UFC)**, buscando identificar seu estilo de cobrança, presença no acervo e bancas de perfil semelhante para ampliar o leque de treino.

---

### 💬 Consulta 1: Identificação da Banca e Mapeamento de Similares

```text
Qual a banca do concurso de Aracati? No banco de questões encontrou ela? Consegue traçar um perfil dela? Que bancas se aproximam mais do perfil dela?
```
*(No padrão N.A.G., equivale a: `Use P07 para diagnosticar a banca FCPC e mapear bancas análogas no acervo de AFO`).*

#### 📑 Resposta Entregue pelo NotebookLM:

A banca organizadora do concurso do ISS Aracati (Edital nº 02/2026) é a **Fundação Cearense de Pesquisa e Cultura (FCPC)**, instituição vinculada à **Universidade Federal do Ceará (UFC)**.

#### 1. PRESENÇA NO BANCO DE QUESTÕES
A FCPC está presente no acervo de questões de AFO e Direito Financeiro do curso. O banco reúne questões aplicadas pela FCPC em certames de nível superior da própria UFC, cobrando temas como créditos adicionais e estágios da despesa pública.

#### 2. PERFIL ANALÍTICO DA BANCA FCPC
* **Formato e Estilo de Prova:** Trata-se de uma banca de perfil acadêmico/universitário que adota o modelo tradicional de múltipla escolha com 5 alternativas (A, B, C, D, E).
* **Uso de Situações Hipotéticas Práticas:** A FCPC costuma elaborar enunciados baseados em casos concretos da gestão pública (como a contratação de obras e reformas em unidades públicas, medições de contratos e necessidades emergenciais de orçamento).
* **Cobrança Focada na Legislação Seca:** As questões exigem o domínio direto dos textos normativos fundamentais: a **Lei Federal nº 4.320/1964**, os artigos 165 a 169 da **Constituição Federal de 1988** e a **Lei de Responsabilidade Fiscal (LC nº 101/2000)**.
* **Objetividade e Inflexão Técnica:** Exige a correta identificação de conceitos e institutos orçamentários (como modalidades de empenho, fontes de recursos para créditos adicionais e enquadramento de despesas) de forma direta e sem divagações doutrinárias.

#### 3. BANCAS COM PERFIL ANÁLOGO / SEMELHANTE
* **Bancas Universitárias e Acadêmicas (IV-UFG, UFU-MG, COMVEST-UFAM, COPESE-UFT, FUMARC):** Possuem a mesma matriz de elaboração, utilizando questões de múltipla escolha voltadas ao conhecimento prático-normativo e à aplicação da legislação em casos institucionais.
* **Bancas Tradicionais de Lei Seca (VUNESP e FCC):** Guardam forte semelhança quanto ao rigor técnico de cobrança da Lei nº 4.320/1964 e da CF/88, testando a literalidade dos artigos e a classificação das finanças públicas em itens de múltipla escolha.
* **Bancas Regionais de Múltipla Escolha (FUNDATEC, IDECAN e INSTITUTO AOCP):** Apresentam padrão de enunciado similar para concursos municipais e estaduais, cobrando a mecânica dos instrumentos de planejamento (PPA, LDO e LOA) e regras de execução financeira.

---

### 💬 Consulta 2: Mapa Global de Incidência e Previsão de Cobrança

Em seguida, o estudante aprofunda para saber onde investir a maior carga horária de estudos:

```text
Então dentro da disciplina AFO você acredita que ela cobrará mais qual assunto? Como seria a cobrança?
```

#### 📑 Resposta Entregue pelo NotebookLM:

O assunto de maior incidência em **Administração Financeira e Orçamentária (AFO)** para o concurso do **ISS Aracati-CE** será **Orçamento Público no Brasil (PPA, LDO e LOA sob a regência da CF/88)**, representando **59,4% do volume total de questões da matéria**, seguido pela **Lei de Responsabilidade Fiscal (34,2%)** e pelo **Ciclo Orçamentário (19,2%)**.

#### 1. MAPA DE INCIDÊNCIA TEMÁTICA DA DISCIPLINA AFO

Analisando a estrutura empírica da matéria em provas recentes para cargos fiscais e de controle, a distribuição percentual dos tópicos organiza-se da seguinte forma:

| Posição | Macro-Assunto | Volume de Questões | Participação | Taxa Média de Acerto | Enquadramento Estratégico |
| :---: | :--- | :--- | :--- | :--- | :--- |
| **1º** | **Orçamento Público no Brasil (CF/88)** | 840 q | **59,4%** | 77,6% | **Garantidor de Pontos** (Inadmissível errar) |
| **2º** | **Lei de Responsabilidade Fiscal (LC 101/00)** | 484 q | **34,2%** | 73,5% | **Pilar Obrigatório** (Normas e Limites) |
| **3º** | **Ciclo Orçamentário e Processo** | 272 q | **19,2%** | 77,9% | **Alto Custo-Benefício** |
| **4º** | **Despesa Pública e Classificações** | 256 q | **18,1%** | 67,9% | 🚨 **Casca de Banana** (Maior taxa de erro: 32,1%) |
| **5º** | **Estágios da Receita e da Despesa** | 251 q | **17,7%** | 77,1% | **Mecânica Operacional** |
| **6º** | **Programação Orçamentária e Financeira** | 121 q | **8,6%** | 75,8% | **Execução Financeira** |
| **7º** | **Receita Pública e Classificações** | 116 q | **8,2%** | 71,8% | **Relevância Fiscal** |
| **8º** | **Princípios Orçamentários** | 114 q | **8,1%** | 75,3% | **Dogmática e Exceções** |

---

#### 2. O PERFIL DE COBRANÇA DA BANCA FCPC (UNIVERSIDADE FEDERAL DO CEARÁ)

A **Fundação Cearense de Pesquisa e Cultura (FCPC)** possui um perfil de elaboração **acadêmico-operacional**, caracterizado por:
1. **Modelagem de Múltipla Escolha (A, B, C, D, E):** Questões com enunciados diretos ou estruturados sobre situações práticas da Administração Pública.
2. **Estudos de Caso e Situações Hipotéticas Práticas:** A FCPC costuma simular problemas vivenciados por secretários municipais ou diretores de autarquias/universidades (ex: necessidade de aditamentos contratuais em reformas de prédios públicos, insuficiência de dotações em medições de obras e urgências fiscais).
3. **Cobrança Focada na Legislação Seca Aplicada:** Combina a regra literal da **Lei nº 4.320/1964**, dos **Arts. 165 a 169 da CF/88** e da **LC nº 101/2000 (LRF)** com a correta solução jurídica para a historinha do enunciado.

---

#### 3. COMO CADA ASSUNTO SERÁ COBRADO NA PROVA

##### A. Orçamento Público na CF/88 (PPA, LDO e LOA)
* **Forma de Cobrança:** A banca apresentará um caso em que o Município de Aracati precisa realizar determinada política pública e perguntará em qual lei orçamentária a ação deve ser inserida.
* **Pontos de Teste do Examinador:**
  * **PPA (Art. 165, § 1º):** Exigência de que despesas de capital (investimentos), suas decorrentes (custeio do investimento) e programas continuados constem no PPA de forma **regionalizada**. Pegadinha: afirmar que investimentos de execução em apenas um exercício financeiro exigem PPA (somente os que ultrapassam um exercício exigem inclusão obrigatória, art. 167, § 1º).
  * **LDO (Art. 165, § 2º):** Foco na seleção de **metas e prioridades anuais**, orientação da LOA, diretrizes de política fiscal e regras sobre alterações na legislação tributária. Pegadinha: afirmar que a LDO cria ou aumenta tributos (ela apenas dispõe sobre as alterações que ocorrerão por lei própria).
  * **LOA (Art. 165, § 5º):** Estrutura da tripartição orçamentária (**Fiscal, Seguridade e Investimento das estatais**). Exigência de que as **estatais dependentes** integrem o Orçamento Fiscal ou da Seguridade Social, enquanto o Orçamento de Investimento é restrito às **estatais independentes** (e cobre apenas despesas de investimento).
  * **Princípio da Exclusividade e Exceções (Art. 165, § 8º):** A LOA não pode conter matéria estranha, **salvo autorização para abertura de créditos suplementares e contratação de operações de crédito (inclusive ARO)**.
  * **Prazos do ADCT (Art. 35, § 2º):** PPA e LOA (envio até 31/08; devolução até 22/12) e LDO (envio até 15/04; devolução até 17/07). Regra do recesso: o recesso parlamentar de julho só é vedado caso a **LDO** não seja aprovada.

##### B. Créditos Adicionais e Lei nº 4.320/1964 (Foco Prático FCPC)
* **Forma de Cobrança:** A FCPC elaborará um estudo de caso apresentando um órgão municipal que iniciou a execução de um contrato e constatou a necessidade de ajustar o orçamento.
* **Pontos de Teste do Examinador:**
  * **Tipologia:** Diferenciar se a situação exige **Crédito Suplementar** (reforço de dotação preexistente insuficiente), **Crédito Especial** (criação de dotação para despesa sem previsão orçamentária) ou **Crédito Extraordinário** (despesas imprevisíveis e urgentes, como calamidade pública ou guerra, aberto por decreto/medida provisória).
  * **Requisitos e Fontes de Custeio (Art. 43 da Lei 4.320/64):** Identificação das fontes disponíveis para abertura: **Superávit Financeiro** do balanço patrimonial do exercício anterior, **Excesso de Arrecadação** do exercício em curso, **Anulação Parcial ou Total de Dotações** e **Operações de Crédito** autorizadas.

##### C. Lei de Responsabilidade Fiscal (LC nº 101/2000)
* **Forma de Cobrança:** Questões situacionais envolvendo os mecanismos de ajuste e transparência fiscal do município.
* **Pontos de Teste do Examinador:**
  * **Anexos da LDO (Art. 4º da LRF):** O candidato deve separar o **Anexo de Metas Fiscais** (fixação de metas trienais de receita, despesa, resultado primário, nominal e montante da dívida) do **Anexo de Riscos Fiscais** (avaliação de passivos contingentes e eventos incertos).
  * **Limitação de Empenho (Contingenciamento - Art. 9º):** Caso a arrecadação de receitas comprometa o cumprimento das metas do AMF ao final de um bimestre, os Poderes devem promover a limitação de empenho nos 30 dias seguintes segundo os critérios da LDO.
  * **Despesa com Pessoal (Arts. 18 a 23):** Conceito da Receita Corrente Líquida (RCL), limites percentuais para o município (54% Executivo, 6% Legislativo = 60% Total) e prazos de recondução em caso de estouro do limite máximo.

##### D. Despesa Pública e Suas Classificações (O Divisor de Águas)
* **Forma de Cobrança:** Questões de enquadramento contábil e orçamentário de gastos municipais.
* **Pontos de Teste do Examinador:**
  * **Categoria Econômica (Despesas Correntes vs. Despesas de Capital):** Diferença entre despesas de custeio/pessoal e investimentos públicos.
  * **Investimentos vs. Inversões Financeiras (A Pegadinha Clássica):** 
    * **Investimentos:** Obras públicas, aquisição de instalações e equipamentos novos (que geram expansão da capacidade produtiva).
    * **Inversões Financeiras:** Aquisição de imóveis ou bens **já em uso**, aquisição de títulos representativos de capital de empresas já em funcionamento e concessão de empréstimos.
