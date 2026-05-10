---
name: formacao-brand-visual-ia-ad-video-creator
description: Skill NOVA do Bloco 4 que gera ad de vídeo Meta cold (15-30s) com estrutura específica de ad de vídeo (Hook + Mecanismo + Prova + Reversão de risco + CTA — diferente da estrutura de Reel orgânico). Aplica anatomia da Aula 04 do Extra-Copy + storyboard de 5 cenas + prompts em 6 camadas (alimenta image-generation) + JSON de video-prompts (alimenta video-prompts) + brief de edição no CapCut com texto overlay agressivo (mais rápido que Reel orgânico) + specs Meta (9:16, MP4, ≤1GB, captions queimadas). Output são variações pra teste A/B (3-5 hooks alternativos). Use quando o aluno disser - 'ad de vídeo Meta', 'video ad cold', 'ad video creator', 'criar ad de vídeo', 'creative de vídeo Meta'. Bloco 4.5 do workflow Formação Branding Visual com IA — skill nova, complementa static-ads-ecommerce.
---

# Ad Video Creator — Bloco 4.5 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — skill NOVA na v0.6.0. Preenche gap crítico identificado no diagnóstico: stack pedia "ads (estáticos + vídeo)" mas só `static-ads-ecommerce` existia. Esta skill cobre ad de vídeo end-to-end.
>
> Alinhada à Aula 04 do Extra-Copy (Anatomia de um Ad de Meta) + Aula 06 (Hooks short-form) + Aula 13 do Extra-Ofício (Geração de Vídeo + JSON Prompting).

## Propósito

Ad de vídeo orgânico (tipo Reel) usa estrutura Hook→Setup→Middle→Resolution→CTA do M03. **Ad de vídeo PAGO** (Meta cold) usa estrutura DIFERENTE — orientada à conversão direta:
**Hook (1.5s) → Mecanismo Único (5s) → Prova (3s) → Reversão de risco (3s) → CTA específico (2.5s)** = 15s ad cold padrão.

Esta skill produz ad de vídeo Meta end-to-end: copy + storyboard + prompts + JSON + brief de edição + specs.

## Quando acionar

- "Ad de vídeo Meta / video ad cold"
- "Ad video creator / criar ad de vídeo"
- "Creative de vídeo Meta"

## O que esta skill entrega

`{vault}/marcas/{slug}/ads/video-{nome}-{data}/` com:

- **Copy script** (5 blocos):
  - Hook (1-1.5s) — visual + texto overlay
  - Mecanismo Único (5s) — explica COMO o produto funciona em 1 frase
  - Prova (3s) — número específico OU depoimento OU demonstração visual
  - Reversão de risco (3s) — garantia / devolução / trial
  - CTA específico (2.5s) — verbo + benefício + plataforma

- **Storyboard de 5 cenas** (uma por bloco) com:
  - Ângulo + tamanho de plano + movimento
  - Texto overlay (motion design aplicado, mais agressivo que Reel orgânico)
  - Duração exata em frames

- **Prompts em 6 camadas** (alimenta `prompt-builder` 4.2 + `image-generation` 4.3) — 5 stills

- **JSON de video-prompts** (alimenta `video-prompts` 4.4) — 5 clipes image-to-video

- **Brief de edição CapCut** — timeline frame-by-frame, transitions agressivas (cuts diretos rápidos), captions queimadas (Meta autoplay sem som por default)

- **Specs Meta finais:**
  - 9:16 (Reels/Stories) ou 1:1 (Feed) ou 4:5 (Feed Max)
  - MP4, H.264, ≤4GB (limite Meta)
  - Audio AAC 128 kbps mínimo
  - Captions queimadas (não SRT — queima na edição)
  - Versão sem som funcional (autoplay sem som)

- **3-5 variações A/B** — mudando o Hook (parte mais alavancada do ad)

## Pré-requisitos

- `brand-guideline-companion.md`
- `bloco-1-3-product-research.md` (mecanismo único + prova + objeção a inverter)
- `bloco-3-7-photography-signature.md` + `bloco-3-8-videography-signature.md`
- Brand Face URL (se ad tem pessoa)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Product research (mecanismo + provas + objeções)
4. Photography + Videography Signatures

## Fluxo de execução (~60-90 min por ad)

### Fase 1 — Briefing do ad
- Produto/lançamento alvo
- Objetivo (cold conversion / retargeting / consideração)
- Aspect ratio (9:16 / 1:1 / 4:5)
- Duração (15s / 30s / 60s — 15s é o mais comum cold)
- Avatar Beatriz (do ideal-client) — pra quem vai aparecer

### Fase 2 — Estrutura específica de ad de vídeo (Hook + Mecanismo + Prova + Reversão + CTA)
NÃO é Hook/Setup/Middle/Resolution/CTA do storyboard. É a estrutura DIFERENTE pra ads pagos:
- **Hook** — primeiros 1.5s decidem 71% do destino (Aula 06 Extra-Copy); SCROLL STOPPER agressivo
- **Mecanismo Único** — explica COMO em 1 frase com palavra própria da marca (vem de product-research)
- **Prova** — número exato (ex: "1.347 frascos") ou demonstração visual
- **Reversão de risco** — "30 dias de garantia" / "devolução grátis" / "primeira sessão grátis" (pode dobrar CTR)
- **CTA específico** — verbo no imperativo + benefício + onde clicar (ex: "Tester por R$89 — link na bio")

### Fase 3 — Storyboard 5 cenas
Cada cena = 1 bloco da estrutura. Skill define ângulo/tamanho/movimento/texto overlay/duração exata.

### Fase 4 — Prompts em 6 camadas
Pra cada cena, gera prompt aplicando Photography Signature. Output em inglês com tradução `↳` PT-BR. Alimenta `image-generation` (4.3).

### Fase 5 — JSON de video-prompts
Pra cada cena, gera JSON de 10 campos pra image-to-video (Higgsfield/Veo). Pacing AGRESSIVO (faster que Reel orgânico). Alimenta `video-prompts` (4.4).

### Fase 6 — Brief de edição CapCut
Timeline frame-by-frame:
- V1: A-roll (5 clipes image-to-video gerados)
- V2: B-roll cuts (se aplicável)
- V3: text overlays AGRESSIVOS (motion design da marca + duração curta — entrada rápida fade ou hard cut)
- V4: brand logo + end card (Component instance Figma)
- A1: voiceover ou silêncio (depende da estratégia)
- A2: música licenciada -22dB
- A3: SFX punchy nos cuts (whoosh, click, pop)
- **Captions queimadas** — overlay de transcrição em todos os clipes (Meta autoplay sem som)
- Transições: cuts diretos rápidos (não fade longo) — pacing de ad

### Fase 7 — Specs Meta + Export
9:16 ou 1:1 ou 4:5 / MP4 H.264 / 16-20 Mbps / ≤4GB / AAC 128 kbps / captions queimadas / versão funcional sem som.

### Fase 8 — Gerar 3-5 variações de Hook
A parte mais alavancada do ad é o Hook (1.5s). Gera 3-5 hooks alternativos pra teste A/B (mantém o resto, varia só o hook).

## Padrão de comunicação (Contrato B)

PT-BR. Cita a estrutura como "anatomia do ad de Meta da Aula 04 Extra-Copy" pra alinhar com o curso.

## Decisões com o aluno (Contrato C)

- **Aspect ratio + duração:** propõe baseado em estágio de funil
- **Voiceover Sim/Não:** marca decide (alguns brands usam, outros silêncio)
- **3-5 hooks alternativos:** aluno valida cada um antes de produzir variantes

## Output e integração downstream (Contrato D)

Consumido por:
- `prompt-builder` (4.2) + `image-generation` (4.3) — geram os 5 stills
- `video-prompts` (4.4) — geram os 5 clipes
- `edicao` (4.7) — monta o ad final no CapCut com brief
- `platform-adaptation` (4.8) — versões pra Reels Ad / Stories Ad / Feed Ad

## Quality check (Contrato E)

- Estrutura de 5 blocos respeitada (Hook+Mecanismo+Prova+Reversão+CTA)?
- Hook em 1.5s (não mais)?
- Captions queimadas (não SRT)?
- Versão sem som funcional?
- Specs Meta corretos (aspect/codec/bitrate/duração)?
- 3-5 variações de Hook geradas?
- Reversão de risco INCLUÍDA (a maioria dos ads esquece — perde 30-50% de CTR)?

## Antipatterns

1. Usar estrutura de Reel orgânico (Hook/Setup/Middle/Resolution/CTA) em ad pago — perde conversão
2. Esquecer Reversão de risco (30-50% de CTR ficam na mesa)
3. Captions SRT em vez de queimadas (Meta autoplay sem som = ad invisível)
4. Hook longo demais (>2s) — scroll stopping falha
5. CTA genérico ("compre agora") — perde 30-50% vs específico
6. Não gerar variações de Hook — perde teste A/B do elemento mais alavancado
7. Pacing slow contemplativo (igual Reel orgânico) — ad cold precisa de pacing punchy
8. Mencionar plataformas evitadas (TikTok Ads, LinkedIn Ads) — fora do stack default

## Frase-âncora

> **"Ad de vídeo Meta cold: Hook em 1.5s, Mecanismo + Prova + Reversão em 11s, CTA em 2.5s. Esquecer Reversão de risco custa 30-50% de CTR."**
