---
name: formacao-brand-visual-ia-edicao
description: Conduz o aluno pela edição final de Reels/vídeos no CapCut (default) ou DaVinci Resolve aplicando Videography Signature + Motion Design + Transitions Signature do Brand Vocabulary. Cobre timeline frame-by-frame, stack de áudio em camadas (música licenciada + diegéticos + voiceover se permitido), motion design dos textos overlay (fade, slide, scale, typewriter, hard cut), color grading consistente, export settings finais. Usa Figma como template-source de overlays, thumbnails e end cards. Aplica Quality Check pré-publicação contra Brand Guideline. Use quando o aluno disser - 'edição', 'CapCut', 'DaVinci', 'editar Reel', 'montar timeline', 'motion design de texto', 'sound design', 'export final'. Bloco 4.7 do workflow Formação Branding Visual com IA — depois de video-prompts e catalog-coherence, antes de platform-adaptation.
---

# Edição — Bloco 4.7 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às Aulas 12 (9 Hacks de Edição), 14 (Processo Completo) e 15 (Pós-produção) do Extra-Ofício + M06 toda (Videografia).

## Propósito

Vídeos image-to-video gerados pelo Higgsfield/Veo são clipes de 3-5 segundos. Esta skill conduz a **montagem final no CapCut** (default) ou DaVinci Resolve, aplicando Videography Signature + Motion Design + transitions da marca, usando Figma como template-source pra overlays/thumbnails/end cards.

## Conexão com o curso

- **Extra-Ofício Aula 12 (9 Hacks de Edição)** — Hack 8 (sound design via masking) + outros aplicáveis
- **Extra-Ofício Aula 14 (Processo Completo de Produção)** — Estação 5 (vídeo) e timeline
- **Extra-Ofício Aula 15 (Pós-produção)** — masking, color grading, ajustes finais
- **M06 Aulas 06 (Transitions), 08 (Videography Style), 09 (Pacing+Grading+Atmosfera), 10 (Aplicação Integrada)** — vocabulário aplicado na edição

## Quando acionar

- "Edição / CapCut / DaVinci"
- "Editar Reel / montar timeline"
- "Motion design de texto / sound design / export final"

## O que esta skill entrega

`{vault}/marcas/{slug}/edicoes/{nome-do-reel}-blueprint.md` (blueprint da edição) + MP4 final salvo em `edicoes/{nome}.mp4`:

- **Setup do projeto:** aspect ratio + resolution + fps + color space
- **Timeline frame-by-frame com timecode:**
  - V4: brand overlays (logo + end card)
  - V3: text overlays (motion design aplicado)
  - V2: B-roll / cutaways
  - V1: A-roll (clipes principais)
  - A1: voiceover (se aplicável)
  - A2: música licenciada
  - A3: diegéticos / SFX
- **Transitions por par de shots** (Cut direto / J Cut / L Cut / Match Cut / Whip Pan — só usa as da Transitions Signature)
- **Motion design de texto** (font + size + weight + easing + duração — vem do Motion Design da marca)
- **Stack de áudio com volumes** (música -22 a -28dB / diegéticos -8dB / voiceover 0dB)
- **Color grading** aplicado consistentemente (vem do Videography Signature)
- **Quality check pré-publicação** (15-20 itens)
- **Export settings finais:** H.264 16-20 Mbps + AAC 320 kbps 48 kHz

## Pré-requisitos

- `bloco-3-7-photography-signature.md`
- `bloco-3-8-videography-signature.md`
- `bloco-3-9-motion-design.md`
- Vídeos image-to-video gerados (URLs/files de Higgsfield/Veo/Kling)
- Storyboard com timeline (`storyboard` 4.1)
- Música licenciada (Artlist / Epidemic Sound / Musicbed / Soundstripe — biblioteca do aluno)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Storyboard do Reel/vídeo
4. Lista dos clipes gerados

## Fluxo de execução (varia — 60-180 min por Reel)

### Fase 1 — Setup do projeto no CapCut (default) ou DaVinci
Aspect ratio (9:16 / 1:1 / 16:9), resolution (1080p mínimo / 4K se pra YouTube), fps (30 ou 24), color space (sRGB pra web; Rec.709 pra YouTube).

### Fase 2 — Importar clipes + montar A-roll
A-roll (V1) = backbone do vídeo. Clipes na ordem do storyboard. Aplica pacing definido pela Videography Signature.

### Fase 3 — Adicionar B-roll (V2)
Cutaways pra cobrir cortes + adicionar contexto. Ratio 70/30 ou 80/20 (A-roll/B-roll) baseado em tipo de conteúdo (M06 Aula 07).

### Fase 4 — Transitions
Aplica APENAS as 2-3 transições da Transitions Signature da marca (M06 Aula 06 — não usa as 9 todas). Default: cut direto + 1 expressiva.

### Fase 5 — Text overlays + Motion Design
V3 = textos. Aplica:
- Font + size + weight da Tipografia da marca
- Animation style dominante (fade / slide / scale / typewriter / hard cut — vem do Motion Design)
- Easing técnico (cubic-bezier)
- Safe zones por aspect ratio (220px topo / 420px base pra 9:16)
- Posicionamento padrão (lower third, etc.)

### Fase 6 — Brand overlays (V4)
- Logo via Component instance do Figma (export PNG transparente da Página 2)
- End card final (template do Figma)
- Captions queimadas se for ad pago

### Fase 7 — Stack de áudio em camadas
- A1 voiceover (se permitido pela marca — alguns brands evitam IA voiceover)
- A2 música licenciada (-22 a -28dB)
- A3 diegéticos / SFX (-8dB)
- Sound design pode usar masking (Hack 8 do Extra-Ofício Aula 12)

### Fase 8 — Color grading
Aplica grading da Videography Signature (Warm Muted / Cool Clean / Vibrant Saturated / Naturalist / High Contrast Editorial). Highlights + shadows do brand book.

### Fase 9 — Quality check pré-publicação (15-20 itens)
- Aspect ratio correto?
- Resolution mínima?
- Safe zones respeitadas?
- Transitions só do brand book?
- Text styles aplicados?
- Logo legível?
- Audio sem clipping?
- Color grading consistente entre clipes?
- Loop perfeito (se Reel)?
- Captions sincronizadas?
- Etc.

### Fase 10 — Export
H.264 16-20 Mbps (qualidade vs tamanho — Reel curto pode 16, ad pago vai 20).
AAC 320 kbps 48 kHz.
MP4 ≤1GB (limite Meta Ads).

Salva como `edicoes/{nome}.mp4` no vault.

## Padrão de comunicação (Contrato B)

PT-BR. Quando aluno é editor experiente: linguagem técnica (V1-V4, A1-A3, color space, dB). Quando não é: explica termos.

## Decisões com o aluno (Contrato C)

- **CapCut vs DaVinci:** propõe baseado em complexidade da edição
- **Voiceover IA Sim/Não:** marca decide (alguns brands evitam por ética/autenticidade)
- **Music track:** aluno escolhe da biblioteca licenciada que ele tem
- **Quality check:** aluno aprova antes do export final

## Output e integração downstream (Contrato D)

Consumido por:
- `platform-adaptation` (4.8) — adapta MP4 pros canais (corta pra Stories, gera versão Feed, etc.)
- `figma` (3.11) — thumbnail/cover frame importado como referência

## Quality check (Contrato E)

- Setup do projeto correto (aspect/resolution/fps/color space)?
- Transitions APENAS do brand book?
- Motion design dos textos aplicado?
- Audio em 3 camadas com volumes corretos?
- Color grading consistente?
- 15-20 itens do checklist passados?
- Export settings corretos pro destino (Meta Ads / IG orgânico / YouTube)?

## Antipatterns

1. Usar todas as 9 transições — vira improviso, sem assinatura
2. Music sem licença (Suno / YouTube Audio Library OK; tracks aleatórias do TikTok = strike de copyright)
3. Voiceover IA sem permissão da marca — alguns brands proíbem por ética
4. Color grading inconsistente entre clipes — quebra coerência
5. Pular safe zones — texto cortado pela UI
6. Export em qualidade baixa pra "ser leve" — fica granulado
7. Não usar Figma como template-source pra logo/end card — perde Component instance, fica difícil atualizar

## Frase-âncora

> **"Edição não é montagem de cortes — é orquestração de respirações. Cada transição, cada respiro, cada overlay deve ressoar a marca."**
