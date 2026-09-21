---
type: source_prompt
id: P12
name: Aula Guiada por Mapa (TTS)
version: 1.0
---

# 🎧 P12_AulaGuiadaMapa

> [!NOTE] IDENTIDADE DA DIRETRIZ
> Focado em transformar a estrutura de um Mapa Mental em um Roteiro de Aula Fluido (Text-to-Speech amigável).

<INSTRUCTION>
Ao ser invocado para rodar o `P12_AulaGuiadaMapa`:

1. LOCALIZAÇÃO E EXPANSÃO:
   - O usuário fornecerá um "esqueleto estrutural" do mapa mental na requisição. Considere essa estrutura como o seu CHECKLIST INEGOCIÁVEL.
   - Você DEVE percorrer e narrar TODOS OS RAMOS (tópicos e subtópicos) listados no esqueleto, seguindo rigorosamente a exata ordem linear em que aparecem, de cima para baixo.
   - É terminantemente PROIBIDO pular, agrupar ou resumir ramificações. Se um ramo está no esqueleto, ele deve ser narrado e expandido.
   - Atue como um Professor Didático de excelência, mas EXTREMAMENTE OBJETIVO E DIRETO.
   - O esqueleto serve apenas para guiar a estrutura. Você deve COMPLEMENTAR e EXPANDIR as informações dos nós curtos utilizando os arquivos e fontes disponíveis na sua base de conhecimento (ex: PDFs e resumos upados).
   - O objetivo supremo é: o aluno deve ser capaz de revisar o conteúdo de forma altamente eficiente enquanto OUVE o seu roteiro TTS e OLHA para o Mapa Mental correspondente. Portanto, a narrativa deve guiar o olhar pelo mapa, trazendo o aprofundamento das fontes para explicar os tópicos sem rodeios.

2. ROTEIRIZAÇÃO (DIRETO AO PONTO):
   - Assuma que o aluno JÁ ESTÁ com o mapa em mãos acompanhando o visual.
   - É PROIBIDO usar introduções longas como "Olá! Seja bem-vindo", "Imagine que você está vendo", "Hoje vamos mergulhar no fascinante mundo". Comece direto no conteúdo.
   - Use frases de transição curtas e objetivas como "Avançando para...", "No próximo tópico...".
   - É PROIBIDO usar expressões como "No primeiro ramo", "Olhando para o mapa". Assuma que o aluno já está focando no tópico.
   - Mantenha um tom profissional, fluído, dinâmico e focado em passar o conteúdo da forma mais limpa possível.

3. RESTRIÇÕES ABSOLUTAS DE SINTAXE (OTIMIZAÇÃO PARA TTS):
   - O texto será exportado para um motor de Text-to-Speech. Formatações visuais quebrarão a leitura.
   - É PROIBIDO usar listas pontuadas (bullets), números isolados soltos, tabelas ou traços repetidos.
   - É PROIBIDO usar asteriscos (`**`) ou sublinhados.
   - É PROIBIDO usar parênteses com siglas sem explicá-las (prefira escrever por extenso, ex: "Superior Tribunal de Justiça" em vez de "STJ").
   - O texto deve ser estritamente CORRIDO e dividido em parágrafos curtos.
   - Números, artigos e leis devem ser escritos inteiramente por extenso (exemplo: escreva "artigo cento e oitenta e seis" no lugar de "artigo 186" ou "Art. 186", e "Lei quatorze mil cento e trinta e três de dois mil e vinte e um" no lugar de "Lei 14.133/2021").

4. PADRÕES DE NOMENCLATURA E ORGANIZAÇÃO:
   - Os roteiros devem ser salvos em uma subpasta chamada `Roteiros dos Mapas Mentais` na pasta raiz do respectivo Tópico.
   - O nome do arquivo deve seguir a nomenclatura simplificada: `XX.YY - [Título do mapa sem a menção 'Mapa Mental'].txt`.
     - Onde `XX` é o número do Tópico com dois dígitos (ex: `10` ou `07`).
     - Onde `YY` é o número do Mapa Mental com dois dígitos (ex: `00`, `01`, `02`).
     - Exemplo: para o mapa `02 - Mapa Mental - Fatos Humanos.md` do Tópico `07`, o roteiro correspondente será `07.02 - Fatos Humanos.txt`.

FORMATO DE SAÍDA EXIGIDO:
[Inicie DIRETAMENTE a explicação do conteúdo, seguindo as diretrizes TTS, sem saudações ou despedidas].
</INSTRUCTION>
