---
name: formacao-brand-visual-ia-briefing-inicial
description: Conduz entrevista inicial estruturada com o aluno pra organizar a confusão dele sobre a própria marca em hipóteses testáveis. Captura visão, motivação, restrições, aspirações, hipóteses do dono ANTES de qualquer pesquisa externa. Output é dossiê estruturado em .md que vai ser testado nos blocos seguintes do workflow. Use quando o aluno disser - 'quero começar minha marca', 'briefing inicial', 'organizar minhas ideias da marca', 'tenho lojinha mas falta direção', 'primeiros passos da marca', 'já tenho ideia mas bagunçada', 'vou criar marca nova', 'quero estruturar o que penso da minha marca'. Primeira skill do workflow Formação Branding Visual com IA — vem ANTES de qualquer pesquisa, decisão estratégica ou identidade visual.
---

# Briefing Inicial — Bloco 0 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às Aulas 1-7 do Módulo 01 do curso autoral.

## Propósito

Toda jornada de marca começa numa cabeça confusa. Aluno chega com ideias, frustrações, aspirações, referências misturadas. Esta skill organiza essa confusão num **dossiê de hipóteses testáveis** — captura o que o aluno acha sobre a marca dele, ANTES da pesquisa externa validar (ou refutar) cada hipótese.

Esta skill é o primeiro passo do workflow. Sem briefing estruturado, o aluno pula pra pesquisa sem saber o que pesquisar — e pra estratégia sem saber qual hipótese validar.

## Conexão com o curso

Atravessa as fundações do M01:
- **Aula 01 (A Inversão)** — diferenciais clássicos viraram entrada; o que vende é posicionamento
- **Aula 02 (As 4 Fases de Mercado)** — saber em que fase o mercado do aluno está
- **Aula 03 (Custo × Preço × Valor Percebido)** — equação real da venda
- **Aulas 05-06 (Identidade × Imagem + Economia da Percepção)** — separação fundamental
- **Aula 07 (Canvas)** — a plataforma de marca que vai ser preenchida ao longo do workflow

## Quando acionar

- "Quero começar minha marca"
- "Briefing inicial"
- "Organizar minhas ideias da marca"
- "Tenho lojinha mas falta direção"
- "Primeiros passos da marca"
- "Vou criar marca nova"
- "Quero estruturar o que penso da minha marca"

## O que esta skill entrega

- Dossiê em formato `.md` cobrindo 13 dimensões da marca
- Lista explícita de **8-10 hipóteses do dono** (H1, H2...) que serão testadas no Bloco 1
- Lista de pendências (TBD) marcadas pra preencher conforme o workflow avança
- Status do workflow atualizado pra "Bloco 0 concluído"

## Pré-requisitos

Nenhum — esta é a primeira skill do workflow. Se o aluno tem dúvida se devia rodar outra antes, a resposta é: comece aqui.

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand` — se já existe marca ativa, perguntar se é pra essa marca ou nova
2. Se for marca nova: criar `{vault}/marcas/{novo-slug}/` e ativar essa marca

## Fluxo de execução (5 fases, ~30-40 min)

### Fase 1 — Identificação da marca
"Qual o nome da marca? Categoria? Fase do negócio (pré-lançamento, ativa, rebrand)? Há quanto tempo existe?"

### Fase 2 — Visão na cabeça do dono
"O que sua marca É? Pra quem? Por quê? O que ela REJEITA?" Captura sem polir.

### Fase 3 — Hipóteses explícitas (a parte mais valiosa)
A skill ajuda o aluno a transformar afirmações em **hipóteses numeradas** (H1, H2...). Exemplos do tipo de hipótese:
- *H1 (cliente):* "Minha cliente paga R$ 500 por essa peça"
- *H2 (mercado):* "Sou a única loja de produto X na cidade Y"
- *H3 (produto):* "O que diferencia meu produto é fornecedora local artesanal"
- *H4 (canal):* "Instagram vende mais que Newsletter"

Cada hipótese vai ser testada no Bloco 1 (audience-research, market-mapping, product-research).

### Fase 4 — Restrições e aspirações
"Orçamento? Equipe? Plataformas USADAS? Plataformas EVITADAS? O que você NÃO quer fazer?"

Aqui captura também o **stack atual de ferramentas do aluno**: Figma? Higgsfield? Midjourney? CapCut? Já usa alguma IA?

### Fase 5 — Validação e geração do dossiê
Apresenta o dossiê montado pra o aluno aprovar. Anti-autonomia: aluno valida antes de salvar.

## Padrão de comunicação (Contrato B)

PT-BR brevemente. Sem jargão técnico desnecessário. Quando precisa explicar termo (ex: "F1∩F2"), explica em 1 frase + remete pra aula correspondente do M01.

## Decisões com o aluno (Contrato C — anti-autonomia)

- **Categoria proposta:** se hesita, skill propõe 2-3 e pergunta qual ressoa
- **Hipóteses:** skill ajuda a formular, mas é o aluno que confirma cada uma
- **Restrições:** skill pode sugerir restrições comuns do nicho, aluno aprova
- A skill NUNCA preenche TBD com chute — marca como `[TBD — a definir no Bloco X]`

## Output e integração downstream (Contrato D)

Salva: `{vault}/marcas/{slug}/bloco-0-briefing-inicial.md`

Consumido por:
- `audience-research` (1.1) — testa hipóteses sobre cliente
- `market-mapping` (1.2) — testa hipóteses sobre mercado
- `product-research` (1.3) — testa hipóteses sobre produto

## Quality check (Contrato E)

- 13 seções preenchidas (com TBD onde aplicável)?
- Hipóteses NUMERADAS e EXPLÍCITAS (não embutidas em prosa)?
- Stack de ferramentas do aluno capturado?
- Aluno aprovou explicitamente antes de salvar?

## Antipatterns

1. Pular fases pra ser rápido — cada fase ancora o pensamento
2. Preencher TBD com chute pra "fechar" o dossiê
3. Decidir categoria, posicionamento ou cliente pelo aluno
4. Apresentar hipóteses como verdades — sempre marcar como "hipótese a testar"
5. Pular a aprovação final do aluno antes de salvar
6. Mencionar ferramentas fora do stack do Kevin (ChatGPT, Sora, Seedream, Runway)

## Exemplos canônicos pra usar com o aluno (referência)

- **Ferra** (utensílios artesanais brasileiros, ticket R$250, B2C produto físico) — exemplo recorrente nas aulas integradoras do M02/M05/M06
- **Cala** (skincare botânico BR, founder-led, ticket R$180-280) — exemplo do Extra-Copy

## Frase-âncora

> **"Briefing inicial não é planejamento — é organizar a confusão honestamente. Hipóteses claras agora valem mais que respostas erradas com cara de certeza."**
