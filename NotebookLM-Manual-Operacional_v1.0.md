# NotebookLM — Manual Operacional (Pro)  
Versão: v1.0 (pipeline universal + protocolo de uso com meta prompts)  
Uso: documento-base para upload e reutilização em qualquer projeto

---

## Sumário
1. [Como usar este manual (rápido)](#como-usar-este-manual-rápido)  
2. [Protocolo de uso comigo (blocos + validação por rodada)](#protocolo-de-uso-comigo-blocos--validação-por-rodada)  
3. [Pipeline Cronológico Universal (visão em 1 página)](#pipeline-cronológico-universal-visão-em-1-página)  
4. [Matriz de decisão (qual serviço usar quando)](#matriz-de-decisão-qual-serviço-usar-quando)  
5. [Serviços e funcionalidades (manual de consulta rápida)](#serviços-e-funcionalidades-manual-de-consulta-rápida)  
   - [S1. Fontes (PDF/URL/YouTube/Texto colado)](#s1-fontes-pdfurlyoutubetexto-colado)  
   - [S2. Deep Research](#s2-deep-research)  
   - [S3. Organização (notebooks, módulos, fontes ativas)](#s3-organização-notebooks-módulos-fontes-ativas)  
   - [S4. Conversa (Chat + instruções do notebook)](#s4-conversa-chat--instruções-do-notebook)  
   - [S5. Mapa mental](#s5-mapa-mental)  
   - [S6. Relatórios (Reports)](#s6-relatórios-reports)  
   - [S7. Flashcards](#s7-flashcards)  
   - [S8. Quiz/Teste](#s8-quizteste)  
   - [S9. Resumo em áudio (Audio Overview)](#s9-resumo-em-áudio-audio-overview)  
   - [S10. Resumo em vídeo (Video Overview)](#s10-resumo-em-vídeo-video-overview)  
   - [S11. Data Tables (Tabelas de dados)](#s11-data-tables-tabelas-de-dados)  
   - [S12. Apresentação de slides (Slide Deck)](#s12-apresentação-de-slides-slide-deck)  
   - [S13. Infográfico](#s13-infográfico)  
   - [S14. Notas, compartilhamento e governança](#s14-notas-compartilhamento-e-governança)  
6. [Biblioteca de meta prompts (templates por serviço)](#biblioteca-de-meta-prompts-templates-por-serviço)  
7. [Checklist final do projeto](#checklist-final-do-projeto)  
8. [Apêndice: Limites do Pro (referência rápida)](#apêndice-limites-do-pro-referência-rápida)

---

## Como usar este manual (rápido)

**Objetivo:** aplicar um processo “fonte → estrutura → retenção → entrega” com o NotebookLM, reduzindo mistura de assunto e extrapolações.

**Regra-mãe:** “Somente fontes; se não constar nas fontes, declarar explicitamente.”

**Como aplicar:**
1) Use o [Pipeline Cronológico Universal](#pipeline-cronológico-universal-visão-em-1-página).  
2) Para cada etapa, siga: **Entrada → Passos → Saída → Critérios de aprovação → Checklist**.  
3) Se o tema for amplo, rode por **módulos** (capítulos/assuntos) antes de síntese final.

---

## Protocolo de uso comigo (blocos + validação por rodada)

### A. O que você vai me enviar (template padrão)
Copie e cole, preenchendo:

**[BRIEF]**
1) Tema (1 linha):  
2) Objetivo final: (aprender / revisão / relatório / apresentação / decisão)  
3) Público/uso: (eu / equipe / clientes)  
4) Escopo (inclui):  
5) Fora do escopo (exclui):  
6) Entregáveis desejados (ordem):  

**[FONTES]**
- Tipos: (PDF/URL/YouTube/texto colado/Deep Research)  
- Quantidade aproximada:  
- Existem módulos/capítulos? (sim/não)  

**[RESTRIÇÕES]**
- “Somente fontes” (sim/não)  
- Linguagem: (PT-BR / EN)  
- Nível: (básico / intermediário / avançado)  
- Formato preferido: (tópicos / texto corrido / tabela)  

### B. Como eu vou responder (sempre em blocos)
**BLOCO 1 — Diagnóstico e riscos**
- O que o assunto parece exigir (ex.: estrutura, comparação, retenção)  
- Riscos prováveis (mistura, fonte ruidosa, tema amplo)  
- Pré-testes recomendados (2–3)

**BLOCO 2 — Opções de pipeline (2 a 4 opções)**
- Opção A (recomendada): ordem de serviços + por quê  
- Opção B/C: alternativas + trade-offs  
- Cada opção vem com checklist e critérios de aprovação

**BLOCO 3 — Decisão**
- Você escolhe qual opção executar e quais serviços usar.

**BLOCO 4 — Meta prompts (rodada a rodada)**
- Eu gero o meta prompt **somente do próximo serviço escolhido**.  
- Você valida (ou ajusta).  
- Só então avançamos para o serviço seguinte.

> Observação operacional: nem todo assunto deve usar todos os serviços. Este protocolo existe para você decidir com base em risco/benefício.

---

## Pipeline Cronológico Universal (visão em 1 página)

**Ordem recomendada (completa):**  
1) Brief do projeto  
2) Fontes (ingestão em lotes + nomeação)  
3) Deep Research (opcional; apenas se tema amplo/instável)  
4) Organização por módulos + fontes ativas  
5) Chat (instruções + formato + regra “não consta nas fontes”)  
6) Mapa mental por módulo  
7) Relatório por módulo (e depois síntese)  
8) Flashcards por módulo  
9) Quiz por módulo  
10) Áudio por módulo  
11) Vídeo por processo/módulo  
12) Data Tables (comparativos/extrações)  
13) Slides (módulos → deck final)  
14) Infográfico (síntese final em 1 peça)  
15) Notas/compartilhamento/governança

---

## Matriz de decisão (qual serviço usar quando)

### Se o objetivo é entender e estruturar
- Mapa mental + Relatório  
- (Se tema amplo) Deep Research → Mapa mental → Relatório

### Se o objetivo é memorizar e revisar
- Flashcards + Quiz + Áudio (por módulo)

### Se o objetivo é comparar ou extrair dados
- Data Tables (com coluna “Fonte/Evidência”) → exportar para Sheets

### Se o objetivo é apresentar
- Relatório (base) → Slides (storyline) → Infográfico (resumo em 1 página)

### Se o objetivo é ensino (aula)
- Relatório (script) → Áudio/Vídeo → Quiz (fixação)

---

# Serviços e funcionalidades (manual de consulta rápida)

## S1. Fontes (PDF/URL/YouTube/Texto colado)

**Objetivo:** criar uma base de conhecimento confiável para todo o resto.

**Entradas:** PDF local, URL, YouTube, texto colado.

**Passo a passo**
1) Crie o notebook: `PROJETO — Tema — AAAA-MM`.  
2) Adicione fontes em lotes pequenos (5–15).  
3) Renomeie cada fonte: `Módulo — Tipo — Origem — Data`.  
4) Faça checagem rápida:
   - PDF: texto selecionável?  
   - URL: conteúdo aparece completo?  
   - YouTube: transcrição existe e é boa?  
   - Texto colado: inclua metadados (origem/data).

**Saída:** base de fontes + nomes padronizados.

**Quando usar:** sempre.

**Quando evitar / riscos**
- Muitas fontes heterogêneas cedo → mistura em outputs.  
- PDFs escaneados → extração fraca.  
- URLs dinâmicas/paywall → texto incompleto.

**Critério de aprovação**
- Você consegue pedir “liste 10 termos e indique em quais fontes aparecem” e a resposta faz sentido.

**Checklist**
- [ ] Fontes em lotes  
- [ ] Nomes padronizados  
- [ ] Qualidade validada (PDF/URL/YouTube)

---

## S2. Deep Research

**Objetivo:** mapear território e criar um “índice” do assunto.

**Entrada:** perguntas-mãe + restrições de confiabilidade.

**Passo a passo**
1) Defina 3–7 perguntas-mãe.  
2) Gere o Deep Research (em 1–2 blocos: fundamentos/aplicações).  
3) Extraia: taxonomia, glossário, trilha de módulos, fontes primárias recomendadas.  
4) Transforme o resultado em plano (S3).

**Saída:** relatório-índice.

**Quando usar**
- Tema amplo, instável ou sem estrutura clara.

**Quando evitar**
- Quando você quer fidelidade estrita a um material fechado (livro/curso) sem “puxar” para fora do escopo.

**Critério de aprovação**
- As principais afirmações podem ser validadas depois com fontes primárias no notebook.

**Checklist**
- [ ] Perguntas-mãe definidas  
- [ ] Resultado usado como índice, não como verdade final

---

## S3. Organização (notebooks, módulos, fontes ativas)

**Objetivo:** reduzir mistura e controlar escopo.

**Passo a passo**
1) Defina módulos (M1, M2, M3…).  
2) Prefixe fontes com M1/M2.  
3) Regra: outputs primeiro por módulo; síntese final por último.  
4) Use “fontes ativas” reduzidas para outputs sensíveis (flashcards/quiz/áudio/vídeo).

**Saída:** arquitetura limpa do projeto.

**Quando usar:** sempre.

**Critério de aprovação**
- Ao gerar flashcards do M1, não surgem conceitos do M3.

**Checklist**
- [ ] Módulos definidos  
- [ ] Fontes rotuladas  
- [ ] Outputs por módulo antes do global

---

## S4. Conversa (Chat + instruções do notebook)

**Objetivo:** controlar formato, tom e aderência às fontes.

**Configuração padrão (recomendada)**
- “Responda somente com base nas fontes selecionadas.”
- “Se não constar nas fontes, diga ‘não consta nas fontes’.”
- “Estruture: (1) resposta direta, (2) evidências, (3) próximos passos.”

**Quando usar:** sempre.

**Riscos**
- Perguntas fora das fontes geram resposta genérica.

**Critério de aprovação**
- Respostas repetíveis e ancoradas, com evidências claras.

**Checklist**
- [ ] Regra “não consta nas fontes” ativa  
- [ ] Formato padrão definido

---

## S5. Mapa mental

**Objetivo:** visão macro e hierarquia.

**Passo a passo**
1) Selecione apenas fontes do módulo.  
2) Gere 1 mapa por módulo.  
3) Revise se há mistura.

**Quando usar:** conteúdo com estrutura/hierarquia.

**Quando evitar:** listas puras ou tabelas (use Data Tables).

**Checklist**
- [ ] 1 mapa por módulo  
- [ ] Sem mistura de módulo

---

## S6. Relatórios (Reports)

**Objetivo:** produzir documento estruturado e “publicável”.

**Templates padrão**
1) Briefing executivo (1–2 páginas)  
2) Guia de estudo (seções + exercícios)  
3) Explainer técnico (conceito → exemplo → trade-offs → checklist)

**Passo a passo**
1) Gere relatório por módulo.  
2) Gere relatório de síntese final.  
3) Exija “sem conclusões novas” se não houver evidência.

**Risco:** extrapolação no final.

**Checklist**
- [ ] Relatório por módulo  
- [ ] Síntese final  
- [ ] Evidência exigida

---

## S7. Flashcards

**Objetivo:** retenção e recall.

**Regras**
- Um conceito por card  
- Por módulo  
- Quantidade travada por rodada

**Frente/verso**
- Frente: pergunta objetiva  
- Verso: resposta curta + exemplo (se houver)

**Checklist**
- [ ] Por módulo  
- [ ] Quantidade travada  
- [ ] Um conceito por card

---

## S8. Quiz/Teste

**Objetivo:** medir lacunas e fixar aprendizado.

**Regras**
- Primeiro por módulo  
- Cumulativo só no final  
- Fontes ativas reduzidas

**Checklist**
- [ ] Quiz por módulo  
- [ ] Cumulativo apenas no fim

---

## S9. Resumo em áudio (Audio Overview)

**Objetivo:** consumo em formato aula falada.

**Regras**
- Prompt curto e restritivo primeiro  
- Por módulo  
- Final sem “novidade” (apenas recapitulação)

**Checklist**
- [ ] Áudio por módulo  
- [ ] Sem extrapolar no final

---

## S10. Resumo em vídeo (Video Overview)

**Objetivo:** síntese visual narrada (processos, comparações).

**Regras**
- Fazer após mapa mental ou relatório (para dar estrutura)  
- Exigir ancoragem nas fontes (quando possível)

**Checklist**
- [ ] Vídeo por processo/módulo  
- [ ] Escopo travado

---

## S11. Data Tables (Tabelas de dados)

**Objetivo:** transformar fontes em tabelas estruturadas e exportáveis para Sheets.

**Quando usar (alto valor)**
- Comparativos, cronologias, action items, métricas, extração de resultados.

**Regras de qualidade**
- Defina colunas antes  
- Coluna “Fonte/Evidência” obrigatória  
- Uma tabela por pergunta (evita mistura)

**Checklist**
- [ ] Colunas definidas  
- [ ] Evidência por linha  
- [ ] Exportação quando necessário

---

## S12. Apresentação de slides (Slide Deck)

**Objetivo:** narrativa visual (apresentação).

**Ordem recomendada**
Mapa mental → Relatório → (Data Tables se houver dados) → Slides

**Regras**
- Deck por módulo primeiro  
- Deck final depois  
- Se houver brandbook, usar como fonte (brand styling)

**Checklist**
- [ ] Storyline (3 mensagens-chave)  
- [ ] Deck por módulo  
- [ ] Identidade visual (se houver)

---

## S13. Infográfico

**Objetivo:** síntese visual em 1 peça.

**Regras**
- 1 tese  
- 3–7 blocos visuais  
- Não inventar números/estatísticas sem fonte

**Checklist**
- [ ] 1 tese  
- [ ] Poucos blocos  
- [ ] Evidência checada

---

## S14. Notas, compartilhamento e governança

**Objetivo:** rastreabilidade e controle do que está validado.

**Governança (tags)**
- VALIDADO: ancorado e revisado  
- EM TESTE: precisa checar  
- DESCARTAR: mistura/erro/fora do escopo

**Checklist**
- [ ] Tags aplicadas  
- [ ] Decisões registradas

---

# Biblioteca de meta prompts (templates por serviço)

> Uso: copie, substitua variáveis e rode **por módulo** quando o tema for amplo.  
> Variáveis: `{TEMA}`, `{MÓDULO}`, `{OBJETIVO}`, `{FORMATO}`, `{PUBLICO}`, `{RESTRICOES}`

## MP0 — Meta prompt padrão do notebook (Chat)
**Cole nas instruções do notebook:**
“Você deve responder somente com base nas fontes selecionadas.  
Se a informação não estiver nas fontes, diga exatamente: ‘não consta nas fontes’.  
Formato obrigatório: (1) resposta direta, (2) evidências (fonte + trecho/indicação), (3) próximos passos práticos.  
Evite conclusões novas no final. Não invente números, datas ou afirmações.”

---

## MP1 — Deep Research (índice do tema)
“Faça Deep Research sobre `{TEMA}` com foco em `{OBJETIVO}`.  
Entregue: (1) taxonomia (categorias), (2) glossário, (3) 10 perguntas-mãe, (4) trilha de módulos recomendada, (5) lista de fontes primárias ideais (docs oficiais, papers, standards).  
Se algo for incerto, marque como hipótese e diga o que faltaria para confirmar.”

---

## MP2 — Mapa mental (por módulo)
“Crie um mapa mental do `{MÓDULO}` com base apenas nas fontes selecionadas.  
Estruture em 3 níveis (macro → meso → micro).  
Não misture conceitos de outros módulos; se houver conexão, cite explicitamente a fonte.”

---

## MP3 — Relatório (Briefing executivo)
“Escreva um briefing executivo sobre `{MÓDULO}` para `{PUBLICO}`.  
Formato: 1) objetivo, 2) conceitos-chave, 3) implicações práticas, 4) riscos/limitações nas fontes, 5) checklist de execução.  
Somente fontes; se não constar, diga ‘não consta nas fontes’.”

---

## MP4 — Flashcards (quantidade travada)
“Gere `{N}` flashcards do `{MÓDULO}`.  
Regras: 1 conceito por card; frente = pergunta objetiva; verso = resposta curta + exemplo (se houver).  
Não inclua conteúdo fora das fontes.”

---

## MP5 — Quiz (por módulo)
“Crie um quiz do `{MÓDULO}` com `{N}` perguntas no nível `{NIVEL}`.  
Inclua: múltipla escolha + 2 questões abertas.  
As perguntas devem ser respondíveis pelas fontes. Se não houver base, não crie a pergunta.”

---

## MP6 — Audio Overview (restritivo)
“Gere um Audio Overview do `{MÓDULO}` apenas com base nas fontes selecionadas.  
Estrutura: (1) conceitos essenciais, (2) exemplos das fontes, (3) erros comuns citados, (4) recapitulação final SEM ideias novas.  
Se algo não estiver explícito, diga ‘não consta nas fontes’.”

---

## MP7 — Video Overview (processo/visual)
“Gere um Video Overview do `{MÓDULO}` focado em `{OBJETIVO}`.  
Use apenas conteúdo das fontes e organize em cenas curtas com títulos.  
Inclua, quando possível, números/termos citados nas fontes.  
Não invente estatísticas; se faltar, declare ‘não consta nas fontes’.”

---

## MP8 — Data Table (esquema + evidência)
“Crie uma Data Table com colunas: `{COLUNAS}`.  
Regras: 1 linha = 1 item; preencher somente com informações das fontes; incluir coluna ‘Fonte/Evidência’ com nome da fonte e um trecho curto que comprove.  
Se a evidência não existir, não preencha a linha.”

---

## MP9 — Slide Deck (storyline + brand styling opcional)
“Crie um Slide Deck sobre `{MÓDULO}` para `{PUBLICO}`.  
Storyline: 1) problema, 2) abordagem, 3) recomendações/ações.  
Pouco texto, mais estrutura visual.  
Se houver brandbook nas fontes, aplique cores/tipografia/estilo consistentes.  
Não inclua afirmações sem base nas fontes.”

---

## MP10 — Infográfico (síntese)
“Crie um infográfico do `{MÓDULO}` com 1 tese central e 3–7 blocos visuais.  
Cada bloco deve refletir algo explícito nas fontes.  
Se precisar de número e não houver base, declare ‘não consta nas fontes’ (não inventar).”

---

# Checklist final do projeto

- [ ] Brief (6 linhas) finalizado  
- [ ] Fontes em lotes + nomeação padronizada  
- [ ] (Opcional) Deep Research usado como índice  
- [ ] Módulos definidos e fontes rotuladas  
- [ ] Instruções do notebook (MP0) aplicadas  
- [ ] Mapa mental por módulo  
- [ ] Relatório por módulo + síntese  
- [ ] Flashcards por módulo  
- [ ] Quiz por módulo  
- [ ] Áudio por módulo  
- [ ] Vídeo por processo/módulo (quando fizer sentido)  
- [ ] Data Tables com evidência por linha (quando houver dados/comparativos)  
- [ ] Slides (módulos → deck final)  
- [ ] Infográfico final (opcional)  
- [ ] Tags VALIDADO/EM TESTE/DESCARTAR aplicadas aos outputs

---

## Apêndice: Limites do Pro (referência rápida)

> Esta seção é para consulta rápida. Confirme sempre na sua UI do NotebookLM Pro.

- Notebooks: até 500 por usuário (Pro)  
- Fontes: até 300 por notebook (Pro)  
- Chats: 500 por dia (Pro)  
- Deep Research: 20 por dia (Pro)  
- Audio Overviews: 20 por dia (Pro)  
- Video Overviews: 20 por dia (Pro)  
- Reports: 100 por dia (Pro)  
- Flashcards: 100 por dia (Pro)  
- Quizzes: 100 por dia (Pro)  
- Mind Maps: sem limite (Pro)

---

## Como você vai usar este manual comigo (modo “rodadas”)

1) Você faz upload deste Markdown + suas fontes do assunto.  
2) Você me manda o template do BRIEF + FONTES + RESTRIÇÕES.  
3) Eu respondo em BLOCO 1/2/3 (diagnóstico + pipelines).  
4) Você escolhe.  
5) Eu gero o meta prompt do próximo serviço (apenas 1 por rodada).  
6) Você valida e avançamos.

Fim.
