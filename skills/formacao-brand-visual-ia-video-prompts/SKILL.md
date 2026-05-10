---
name: formacao-brand-visual-ia-video-prompts
description: Converte cada still aprovado em JSON estruturado pra image-to-video em Higgsfield (principal), Veo 3 ou Kling. Aplica vocabulário cinematográfico (8 angles + 8 shot sizes + 9 movements) e preenche 10 campos estruturados (shot, camera, subject, environment, lighting, color_grade, pacing, audio, mood_keywords, negatives). Usa Videography Signature + Motion Design da marca como input automático. Princípio always image-to-video preservado. Output é JSON pronto pra colar em Higgsfield + nota de qual modelo é mais otimizado pra cada shot. Use quando o aluno disser - 'video prompts', 'JSON pra Higgsfield', 'image-to-video', 'animar imagem', 'JSON video', 'prompt de vídeo'. Bloco 4.4 do workflow Formação Branding Visual com IA — depois de image-generation, antes de catalog-coherence.
---

# Video Prompts — Bloco 4.4 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado à Aula 13 do Extra-Ofício (Geração de Vídeo com IA + JSON Prompting) + M06 (10 aulas).

## Propósito

JSON estruturado é a diferença entre vídeo IA genérico e vídeo cinematográfico. Esta skill converte cada still aprovado em JSON de 10 campos pra alimentar Higgsfield (principal), Veo 3 ou Kling. **Princípio absoluto: always image-to-video** — nunca text-to-video puro.

## Conexão com o curso

- **Extra-Ofício Aula 13 (Geração de Vídeo + JSON Prompting)** — sempre image-to-video; JSON estruturado; 9 movement keywords; ética anti-avatar UGC
- **M06 Aula 04 (9 Movimentos de Câmera)** — Static, Tracking, Crane, Pan, Tilt, Zoom, Push-In, Handheld, Arc
- **M06 Aula 06 (9 Transições)** — vocabulário pra transições entre shots
- **M06 Aula 08 (Videography Style — 5 decisões)** — pacing + grading + transitions + B-roll style já definidos pela marca

## Quando acionar

- "Video prompts / JSON pra Higgsfield"
- "Image-to-video / animar imagem"
- "JSON video / prompt de vídeo"

## O que esta skill entrega

`{vault}/marcas/{slug}/video-prompts/{nome-do-shot}.json` com 10 campos estruturados:

```json
{
  "shot": "...",
  "camera": "...",
  "subject": "...",
  "environment": "...",
  "lighting": "...",
  "color_grade": "...",
  "pacing": "...",
  "audio": "...",
  "mood_keywords": [...],
  "negatives": [...]
}
```

+ Tradução `↳` em PT-BR de cada campo + recomendação de qual modelo usar pra esse shot específico.

## Pré-requisitos

- `bloco-3-8-videography-signature.md` (Videography Signature — pacing/grading/transitions)
- `bloco-3-9-motion-design.md` (motion da marca)
- Still aprovado pelo `image-generation` (URL + seed)
- Storyboard com motion description (`storyboard` 4.1)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Still aprovado + storyboard

## Os 10 campos do JSON

1. **`shot`** — descrição da ação (5-15 palavras): "Woman turns head slowly toward camera, slight smile emerges"
2. **`camera`** — movimento + ângulo + tamanho de plano (puxa de Videography Signature): "Slow push-in from medium close-up to close-up, three-quarter angle, 85mm equivalent"
3. **`subject`** — quem/o quê + estado: "Woman 40s, contemplative expression, natural makeup, looking directly at lens"
4. **`environment`** — onde: "warm interior, soft window light from left, blurred bookshelf in background"
5. **`lighting`** — Lighting Signature da marca: "window light north-facing, soft directional, golden hour warmth, raking light revealing skin texture"
6. **`color_grade`** — Color Grading da marca: "warm muted, highlights rolled off, shadows lifted slightly, naturalist documentary"
7. **`pacing`** — em segundos: "5 seconds total, slow contemplative pacing"
8. **`audio`** — diegético + música/silêncio: "Diegetic: subtle breath, fabric rustle. Music: ambient piano low (-22dB). No voiceover."
9. **`mood_keywords`** — 3-5 palavras-mood: ["contemplative", "intimate", "warm", "cinematic"]
10. **`negatives`** — o que EVITAR: ["fast cuts", "dramatic zoom", "vibrant saturation", "harsh shadows", "background motion"]

## Fluxo de execução (~10-15 min por shot)

### Fase 1 — Identificar o shot
A partir do storyboard, qual shot específico vamos converter em vídeo? Confirmar still aprovado.

### Fase 2 — Aplicar Videography Signature
Pacing + Color Grading + Movement vêm AUTO da marca. Aluno só ajusta se for shot específico que precisa exceção.

### Fase 3 — Preencher os 10 campos
Skill conduz preenchimento de cada campo. Vocabulário cinematográfico técnico em inglês.

### Fase 4 — Recomendação de modelo
Pra esse shot específico, recomenda:
- **Higgsfield** — default, smooth movement, pacing controlado
- **Veo 3** — melhor pra qualidade premium + lip sync
- **Kling** — melhor pra movimento detalhado / transformação

⚠️ Sora, Seedream, Pika, Runway, Luma NÃO estão no stack do Kevin — não recomendar.

### Fase 5 — Output JSON + tradução
Apresenta JSON formatado + tradução `↳` PT-BR de cada campo. Salva em `video-prompts/`.

## Padrão de comunicação (Contrato B)

PT-BR pra explicar; INGLÊS no JSON (vai pra ferramenta IA). Tradução `↳` por campo pra aluno entender.

## Decisões com o aluno (Contrato C)

- **Pacing:** propõe default da Videography Signature, aluno valida ou pede exceção
- **Modelo:** propõe baseado no shot, aluno escolhe
- **Negatives:** propõe lista, aluno acrescenta exceções

## Output e integração downstream (Contrato D)

Consumido por:
- `edicao` (4.7) — vídeos gerados são montados no CapCut
- `ad-video-creator` (4.5) — JSON específico pra ad de vídeo curto

## Quality check (Contrato E)

- 10 campos preenchidos (não pulou nenhum)?
- Pacing bate com Videography Signature da marca?
- Color grade bate com paleta + photography signature?
- Negatives explícitos (anti-bug)?
- Tradução `↳` PT-BR presente?
- Modelo recomendado é Higgsfield/Veo/Kling (não Sora/Pika/Runway)?

## Antipatterns

1. Text-to-video puro (sem still âncora) — quebra "always image-to-video"
2. Pacing genérico ("medium") sem aplicar o da marca
3. Mencionar Sora/Pika/Runway/Luma como opções (fora do stack do Kevin)
4. JSON sem `negatives` — aumenta taxa de bug
5. Audio sempre "music" — vídeo de marca usa silêncio + diegéticos com mais frequência que se imagina
6. Pular tradução `↳` (aluno não-fluente fica perdido)

## Frase-âncora

> **"Always image-to-video. JSON estruturado. 10 campos. A diferença entre vídeo genérico e vídeo cinematográfico."**
