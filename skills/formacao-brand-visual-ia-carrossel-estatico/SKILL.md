---
name: formacao-brand-visual-ia-carrossel-estatico
description: Skill NOVA do Bloco 4 que produz carrossel estático (não vídeo-cêntrico) pra feed de Instagram — educativo, narrativo, social proof ou drop. Estrutura específica de carrossel - Capa (slide 1 com Hook visual + texto manchete) + Setup (slide 2 contexto) + Middle (slides 3-7, 1 conceito por slide) + Resolution (slide 8 payoff) + CTA opcional (slide 9). Aplica Brand Vocabulary + voice-tone + paleta + tipografia. Pipeline Claude→HTML→Figma - skill gera HTML dos 8 slides no canvas Cowork, aluno aprova, skill joga no Figma via MCP usando template carousel-base. Use quando o aluno disser - 'carrossel estático', 'carrossel feed', 'criar carrossel', 'carrossel educativo', 'carrossel narrativo', 'carousel-base', '8 slides', 'carrossel de produto'. Bloco 4.5 do workflow Formação Branding Visual com IA — skill nova.
---

# Carrossel Estático — Bloco 4.5 do Workflow (skill NOVA)

> **Cumpre Contrato Comum das Skills v2.0** — skill NOVA na v0.6.0. Preenche gap: `storyboard` é vídeo-cêntrico (5 elementos temporais); carrossel estático precisa de framework próprio + pipeline Claude→HTML→Figma.

## Propósito

Carrossel estático é um dos formatos de maior engajamento orgânico no Instagram (8-12 slides 4:5 ou 1:1). Esta skill produz carrossel end-to-end com **estrutura específica de slide-a-slide** (não a do storyboard de vídeo) e usa o **pipeline Claude→HTML→Figma**: skill gera HTML dos 8 slides no canvas Cowork, aluno aprova visual, skill joga no Figma via MCP usando template `carousel-base`.

## Conexão com o curso

- **M03 Aulas 02-08 (Storytelling)** — frameworks aplicáveis ao carrossel: Educational, Product Showcase, Story-driven
- **Extra-Copy Aula 12 (Conteúdo orgânico diário)** — carrossel narrativo é 1 dos 9 tipos de post recorrente
- **M02 Aulas 05-06 (Paleta + Tipografia)** — toda decisão visual do slide vem da marca

## Quando acionar

- "Carrossel estático / carrossel feed / criar carrossel"
- "Carrossel educativo / carrossel narrativo"
- "Carousel-base / 8 slides / carrossel de produto"

## Estrutura específica de carrossel (não vídeo)

| Slide | Função | Tempo de leitura | Conteúdo |
|---|---|---|---|
| 1 (Capa) | Hook + headline | 1.5s | Visual forte + texto manchete que faz parar o scroll |
| 2 (Setup) | Contextualizar problema | 2s | "Por que isso importa pra você?" |
| 3-7 (Middle) | 1 conceito/passo por slide | 3s cada | Hierarquia tipográfica consistente |
| 8 (Resolution) | Payoff / síntese | 3s | Frase-âncora + recap visual |
| 9 (CTA opcional) | Ação | 2s | "Salva esse post" / "Conhece a coleção" / "DM com 'Anel' pra link" |

**Tipos de carrossel:**
- **Educativo** — "Por que joia tem nome — a Rota das Mãos em 6 passos"
- **Narrativo** — micro-história de 8 slides
- **Product Showcase** — produto em 8 ângulos / contextos / detalhes
- **Social proof empilhado** — 6-8 depoimentos visuais
- **Drop / lançamento** — apresentação da coleção em 8 slides

## O que esta skill entrega

`{vault}/marcas/{slug}/carrosseis/{nome-do-carrossel}/` com:
- **HTML preview** dos 8-9 slides (renderizado no canvas Cowork pra aprovação visual)
- **8-9 frames vivos no Figma** (Página 4 — Templates Carrossel) com:
  - Color Variables aplicadas (não hardcode)
  - Text Styles aplicados
  - Logo via Component instance (slide 1 e/ou slide 9)
  - Imagem de fundo se aplicável (importada do `image-generation`)
- **Caption específica do post** (75-150 palavras) com hashtags relevantes
- **Production Log** atualizado (Página 11 do Figma)

## Pipeline Claude → HTML → Figma

1. Claude gera HTML/SVG dos 8-9 slides no canvas Cowork (renderizado live com cores reais via CSS variables que batem com Figma Color Tokens, tipografia da marca, hierarquia)
2. Aluno avalia visualmente, pede ajustes em chat ("aumenta o título do slide 3", "troca paleta do slide 5")
3. Claude refaz HTML em segundos
4. Quando aluno aprova → Claude chama `figma` (3.11) via MCP pra criar 8-9 frames novos na Página 4 do Figma com nomes `{nome-carrossel}-slide-01` até `slide-09`
5. Aplica Variables + Text Styles + Component instances do logo
6. Atualiza Production Log

## Pré-requisitos

- `brand-guideline-companion.md`
- `bloco-3-9-motion-design.md` (safe zones por aspect ratio — mesmo carrossel sendo estático, slide pode virar Story)
- `figma-file-key.txt`
- Tema do carrossel + objetivo definido pelo aluno

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. `figma-file-key.txt`

## Fluxo de execução (~30-60 min por carrossel)

### Fase 1 — Briefing
- Tipo (Educativo / Narrativo / Product Showcase / Social proof / Drop)
- Tema central (1 frase)
- Aspect ratio (4:5 default pra feed; 1:1 alternativa)
- Quantidade de slides (8 padrão; 9 se inclui CTA explícito)
- Quem narra (founder / marca em 3ª pessoa / cliente em depoimento)

### Fase 2 — Estrutura slide-a-slide
Skill propõe outline de cada slide baseado no tipo. Aluno valida.

### Fase 3 — Copy slide-a-slide
Pra cada slide:
- Headline ≤8 palavras
- Body ≤30 palavras
- Voice-tone aplicado
- Vocabulário proibido evitado

### Fase 4 — Geração HTML no canvas Cowork
Skill renderiza 8-9 slides em HTML com:
- CSS variables que batem com Color Variables do Figma
- Tipografia carregada via Google Fonts ou system fallback
- Hierarquia tipográfica consistente
- Background (cor sólida, gradiente sutil ou imagem importada do `image-generation`)

### Fase 5 — Iteração com aluno
Aluno pede ajustes em chat. Skill refaz HTML.

### Fase 6 — Handoff Figma via MCP
Quando aprovado, skill chama `figma` (3.11) pra criar os frames no estúdio.

### Fase 7 — Caption do post
75-150 palavras com voice-tone + hashtags (5-15) + CTA na última frase.

### Fase 8 — Salvar tudo
HTML preview + Figma frames + caption + log.

## Padrão de comunicação (Contrato B)

PT-BR pra orientação. Quando renderiza HTML no canvas, mostra ao vivo + pergunta se quer ajustar.

## Decisões com o aluno (Contrato C)

- **Tipo de carrossel:** propõe baseado em objetivo, aluno escolhe
- **8 vs 9 slides:** aluno decide se quer CTA explícito no último
- **Aprovação visual antes do handoff Figma:** crítico — skill NÃO joga no Figma sem aluno ver o HTML primeiro

## Output e integração downstream (Contrato D)

Consumido por:
- `figma` (3.11) — recebe handoff dos 8-9 frames
- `platform-adaptation` (4.8) — adapta carrossel pros canais (Stories cards, Pinterest pins se aplicável)

## Quality check (Contrato E)

- Estrutura específica de carrossel respeitada (não estrutura de Reel)?
- 8-9 slides (não 5, não 15)?
- Headlines ≤8 palavras + Body ≤30 palavras por slide?
- Hierarquia tipográfica consistente entre slides 3-7?
- Color Variables + Text Styles + Logo Component aplicados (não hardcode)?
- Caption tem 75-150 palavras + hashtags + CTA?

## Antipatterns

1. Usar estrutura Hook/Setup/Middle/Resolution/CTA do storyboard (vídeo) em carrossel — slides são paralelos, não sequenciais temporais
2. Texto longo demais por slide — gente dá scroll
3. Hardcode de cor — quebra Brand Tokens
4. Pular handoff Figma — fica em HTML, não vira post final
5. Sem CTA na caption — engajamento cai
6. 15+ slides — Instagram corta em 10 e ninguém vai até o fim mesmo

## Frase-âncora

> **"Carrossel não é vídeo. É 8-9 slides paralelos com hierarquia constante. Slide 1 para o scroll, slides 3-7 entregam valor, slide 8 fecha."**
