---
name: formacao-brand-visual-ia-motion-design
description: Define o sistema de motion design da marca — animation style dominante (smooth, bouncy, quick, slow), easing default (ease-in-out, ease-out, linear), duração padrão de transições de texto, safe zones por aspect ratio (9:16, 1:1, 4:5, 16:9), 3 antipatterns visuais a EVITAR. Aplica a regra 80/20 (80% das peças usam UM estilo dominante, 20% variações). Output é Motion Style Block + safe zones documentadas + lista de antipatterns. Use quando o aluno disser - 'motion design', 'animação de texto', 'animação de elementos', 'easing', 'safe zones', 'estilo de animação'. Bloco 3.9 do workflow Formação Branding Visual com IA — depois de videography signature, antes de brand guideline builder.
---

# Motion Design — Bloco 3.9 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado à Aula 09 do M02 (Motion Identity — Como a Marca se Move).

## Propósito

Como a marca se mexe é tão assinatura quanto a cor. Esta skill define os 2 pilares (animação de texto + elementos gráficos) com regra 80/20 (UM estilo dominante em 80% das peças, variações em 20%). Sem isso, cada Reel vira motion improvisado e o feed perde coerência cinética.

## Conexão com o curso

- **M02 Aula 09 (Motion Identity)** — 2 pilares (animação texto + elementos gráficos); 5 estilos canônicos de animação de texto (Fade, Slide, Scale/Pop, Typewriter, Hard cut); regra 80/20; "motion match brand" (velocidade da animação = velocidade emocional da marca); coerência com tipografia + paleta + brand faces
- **M06 Aula 09 (Pacing)** — pacing do motion respeita pacing do vídeo (definido em videography-signature)

## Quando acionar

- "Motion design / animação de texto / animação de elementos"
- "Easing / safe zones / estilo de animação"

## O que esta skill entrega

`{vault}/marcas/{slug}/bloco-3-9-motion-design.md` com:

- **Animation style dominante** (1 dos 5 canônicos): Fade / Slide / Scale-Pop / Typewriter / Hard cut
- **Animation style secundário** (regra 80/20): qual usar em 20% das peças quando precisa de variação
- **Easing default** — cubic-bezier values (ex: `ease-out` cubic-bezier(0.0, 0.0, 0.58, 1.0))
- **Duração padrão** das transições de texto (em ms — ex: 600ms fade-in, 300ms hard cut)
- **Safe zones por aspect ratio** documentadas em px:
  - **9:16 (Stories/Reels):** 220px topo (UI Instagram) + 420px base (UI Instagram); área segura 1080×1280
  - **1:1 (Feed):** sem safe zones de UI, mas margem interna 80px
  - **4:5 (Feed Max):** 80px margem interna; UI do feed cobre só 60px na base
  - **16:9 (YouTube):** 80px topo e base pra captions
- **3 antipatterns visuais a EVITAR** (animações que destroem a marca)
- **Motion Style Block** em texto pronto pra alimentar prompts/skills do Bloco 4

**No Figma** (Página Brand Guideline):
- Seção Motion Design com style dominante + easing + safe zones marcadas em frames de demonstração

## Pré-requisitos

- `bloco-3-3-typography.md` (motion respeita line-height e letter-spacing)
- `bloco-3-4-color-palette.md` (overlays usam paleta)
- `bloco-3-8-videography-signature.md` (pacing do motion bate com pacing do vídeo)
- `bloco-2-1-big-idea.md` (velocidade emocional)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. Typography + Color Palette + Videography Signature + Big Idea

## Fluxo de execução (~30-45 min)

### Fase 1 — Animation style dominante (regra 80/20)
Skill apresenta os 5 estilos canônicos com associações emocionais (M02 Aula 09):
- **Fade** — luxo, contemplação, premium (Apple, Aesop)
- **Slide** — dinamismo controlado, lifestyle (Old Céline, Tiffany)
- **Scale/Pop** — chamativo, juvenil, energia (Duolingo)
- **Typewriter** — autoral, editorial, manifesto (MrBeast)
- **Hard cut** — agressivo, news, urgência (news editorial)

Aluno escolhe 1 dominante + 1 secundário (variação). 80% do conteúdo usa o dominante.

### Fase 2 — Easing
Aluno escolhe ou skill propõe baseado no style. Defaults sugeridos:
- Fade premium: `ease-out` longo (cubic-bezier(0.0, 0.0, 0.2, 1.0))
- Slide: `ease-in-out` médio
- Scale/Pop: `ease-out` curto + bounce (cubic-bezier(0.34, 1.56, 0.64, 1.0))
- Typewriter: `linear`
- Hard cut: sem easing (instantâneo)

### Fase 3 — Duração padrão
Em ms. Exemplo pra fade premium: 600ms entrada + 400ms saída. Pra scale/pop: 250ms.

### Fase 4 — Safe zones por aspect ratio
Documenta em px exatos as zonas seguras de cada formato. Crítico — texto fora da safe zone é cortado pela UI da plataforma.

### Fase 5 — 3 antipatterns
Pra ESTA marca específica, define 3 animações a evitar (ex: pra marca premium contemplativa: "rotação 360° viral", "zoom punch agressivo", "letras pulando como bouncing balls").

### Fase 6 — Motion Style Block
Skill destila em texto pronto pra alimentar prompts/skills do Bloco 4:
> Ex: *"Motion style: fade dominant, ease-out cubic-bezier(0,0,0.2,1), 600ms in / 400ms out, text overlay using Cormorant Garamond H1 for headline / Inter Caption for legend, safe zones 220px top / 420px bottom for 9:16."*

## Padrão de comunicação (Contrato B)

PT-BR pra explicar; valores técnicos em formato CSS-like (cubic-bezier, ms, px). Se aluno não sabe easing, skill explica em 1 frase + exemplo visual.

## Decisões com o aluno (Contrato C)

- **Style dominante:** apresenta 5 com associações, aluno escolhe baseado em Big Idea + videography
- **3 antipatterns:** propõe baseado em style escolhido, aluno aprova/ajusta

## Output e integração downstream (Contrato D)

Consumido por:
- `brand-guideline-builder` (3.10) — Seção 12 (Motion Design)
- `edicao` (4.7) — CapCut aplica style + easing + duração nas transições de texto
- `carrossel-estatico` (4.5) — slides respeitam safe zones quando exportados pra Stories
- `static-ads-ecommerce` (4.5) e `ad-video-creator` (4.5) — overlays seguem motion style

## Quality check (Contrato E)

- Style dominante escolhido com clareza?
- Easing em formato técnico (cubic-bezier ou nome)?
- Duração em ms (não vaga)?
- Safe zones documentadas pra todos os 4 aspect ratios usados?
- 3 antipatterns específicos pra esta marca?
- Motion Style Block escrito como texto pronto pra colar?

## Antipatterns

1. "Motion bonito" sem definir style dominante (improviso por peça)
2. Easing como nome simbólico ("suave") sem cubic-bezier — designer/IA não tem o que aplicar
3. Pular safe zones — texto cortado pela UI Instagram em 30%+ das peças
4. 5 antipatterns vagos ("não exagerar") em vez de 3 específicos
5. Style oposto ao pacing do vídeo (Hard cut em pacing slow contemplativo) — incoerência crítica

## Frase-âncora

> **"Como a marca se mexe é tão assinatura quanto a cor que ela usa. Movimento transmite personalidade antes do cérebro processar o conteúdo."**
