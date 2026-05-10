---
name: formacao-brand-visual-ia-rapid-prototyping
description: Opera o Claude Design (claude.ai/design) com a marca do aluno em 3 casos onde ele ganha do Figma — pitch deck/one-pager, prototype de site/landing, exploração rápida de direção visual nova. Onboarding único alimenta o Claude Design com brand-guideline-companion.md + arquivo Figma da marca pra ele criar design system automático. Em uso recorrente, gera prompt-pronto customizado pra marca ativa, orienta o aluno no refinamento dentro do Claude Design, e conduz o handoff (Canva minimizado, PPTX, PDF, ou Figma via Anima/html.to.design). Skill SEMPRE remete pra figma quando pedido for produção repetitiva. Use quando o aluno disser - 'claude design', 'pitch deck', 'one-pager', 'prototype de site', 'landing page', 'apresentação pra cliente', 'explorar direção visual nova'. Bloco 3.12 do workflow Formação Branding Visual com IA — depois de figma operação, último do Bloco 3.
---

# Rapid Prototyping — Bloco 3.12 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — skill complementar ao Figma. **Escopo CERCEADO em 3 casos** onde Claude Design ganha do Figma. Pra produção repetitiva, sempre remete pra `figma`.

## Propósito

Figma é protagonista absoluto do estúdio da marca. Mas em **3 casos específicos**, Claude Design (`claude.ai/design`) é mais rápido:
1. **Pitch deck / one-pager** com texto rico + diagramação rápida
2. **Prototype de site / landing page** funcional
3. **Exploração rápida** de direção visual nova (variações experimentais)

Esta skill opera o Claude Design com a marca do aluno. **Pra TODO outro caso (post, story, carrossel, Reel cover, ad estático Meta, catálogo), remete pra `figma`** com firmeza.

## Conexão com o curso

Não há aula direta no curso autoral — esta skill é **operacional**, complementa o sistema sem sobrepor o Figma.

## Quando acionar

- "Claude Design"
- "Pitch deck / one-pager"
- "Prototype de site / landing page"
- "Apresentação pra cliente"
- "Explorar direção visual nova"

⚠️ **NÃO acionar pra:** post de feed, story, carrossel, Reel cover, ad estático Meta, catálogo de produto, peças repetitivas. Pra isso usa `figma`.

## O que esta skill entrega

### Modo ONBOARDING (1 vez por marca)
- `claude-design-onboarding.md` em `{vault}/marcas/{slug}/` com instruções pra alimentar Claude Design:
  - Upload do `brand-guideline-companion.md`
  - Upload do `brand-guideline.pdf`
  - Link/screenshots da Página 2 do Figma
  - Custom instructions colando o Brand Style Block

### Modo PRODUÇÃO (recorrente)
Pra cada um dos 3 casos:
- **Pitch deck / one-pager:** prompt-pronto customizado pra marca ativa + handoff (PPTX / PDF / Canva minimizado / Figma via Anima)
- **Prototype site / landing:** prompt-pronto + handoff (HTML / URL / Figma via html.to.design)
- **Exploração visual:** prompt-pronto + análise dos resultados + recomendação se vale levar pro Figma

## Pré-requisitos

- `brand-guideline-companion.md` + `brand-guideline.pdf` + `figma-file-key.txt`
- Conta Claude Pro / Max / Team / Enterprise (Claude Design exige)
- `claude.ai/design` ativado na conta

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Verificar se `claude-design-onboarding.md` existe (se não, é primeira vez — roda Modo Onboarding antes)

## Fluxo de execução

### Modo ONBOARDING (~30 min, 1 vez por marca)

#### Fase 1 — Verificar acesso ao Claude Design
Pergunta se aluno tem plano Claude Pro+. Se não, recomenda upgrade ou sugere alternativa (Figma + plugins como FigJam ou Slides).

#### Fase 2 — Preparar inputs
- Localizar `brand-guideline-companion.md` + `brand-guideline.pdf` + 5-10 screenshots da Página 2 do Figma

#### Fase 3 — Custom Instructions
Skill gera Custom Instructions pronto pra colar no Claude Design configurando: voz da marca + paleta + tipografia + Brand Faces + Brand Style Block.

#### Fase 4 — Salvar onboarding
`claude-design-onboarding.md` documenta tudo pra reusos futuros.

### Modo PRODUÇÃO (varia — 15-60 min por caso)

#### Caso A — Pitch deck / one-pager
1. Aluno descreve objetivo (apresentar marca pra investidor / aluno / cliente)
2. Skill gera prompt-pronto pra Claude Design com tom + estrutura sugerida
3. Aluno cola prompt no Claude Design, gera, refina
4. Handoff: PPTX (download direto) / PDF (download) / Figma (via Anima) / Canva (minimizado, só se aluno insistir)

#### Caso B — Prototype site / landing
1. Aluno descreve objetivo da página + 3-5 seções principais + CTA
2. Skill gera prompt customizado pra Claude Design
3. Aluno gera HTML, refina iterativamente
4. Handoff: HTML standalone (export) / URL pública / Figma (via html.to.design)

#### Caso C — Exploração visual nova
1. Aluno descreve direção a explorar ("quero ver minha marca em estética vibrant saturated em vez do warm muted atual")
2. Skill gera 3-5 prompts experimentais
3. Aluno gera no Claude Design
4. Skill analisa resultados + recomenda se vale levar pro Figma como nova direção OU descartar

## Padrão de comunicação (Contrato B)

PT-BR. Sempre alerta sobre consumo de tokens (Claude Design gasta tokens rapidamente em iterações). Recomenda iteração focada (não "gera 20 variações").

## Decisões com o aluno (Contrato C)

- **Caso A/B/C:** se pedido cabe em mais de um, pergunta qual prefere
- **Handoff format:** apresenta opções, aluno escolhe baseado em onde vai usar
- **Override pro Figma:** SEMPRE pergunta antes de seguir com Claude Design pra cada caso ("essa peça é repetitiva — não seria melhor no Figma?")

## Output e integração downstream (Contrato D)

Outputs ficam em pastas dedicadas:
- `{vault}/marcas/{slug}/decks/`
- `{vault}/marcas/{slug}/prototypes/`
- `{vault}/marcas/{slug}/exploracoes/`

Consumido por:
- `figma` (3.11) — handoff de prototype/exploração que vale levar pro estúdio principal

## Quality check (Contrato E)

- Pedido cabe num dos 3 casos (NÃO é peça repetitiva)?
- Custom Instructions do Claude Design alinhado com brand guideline atual?
- Output salvo em pasta dedicada (não polui pasta principal)?
- Aluno foi alertado sobre consumo de tokens?

## Antipatterns

1. **Usar Claude Design pra produção repetitiva** (post diário, story, carrossel, Reel cover, ad Meta) — `figma` é melhor pra isso
2. Pular Modo Onboarding — Claude Design sem brand guideline carregado gera marca-genérica
3. Iteração descontrolada (50 variações) — queima tokens sem foco
4. Não fazer handoff pro Figma quando exploração resulta em direção que vale levar adiante
5. Ignorar Canva minimizado — Canva aparece só como destino opcional de handoff de deck, NÃO como ferramenta de produção

## Frase-âncora

> **"Claude Design não substitui Figma. Complementa em 3 casos: deck, prototype de site, exploração. Pra todo o resto, Figma é casa."**
