---
name: formacao-brand-visual-ia-photography-signature
description: Define a assinatura fotográfica da marca em 4 dimensões - lighting (natural/studio/dramatic/soft), mood (minimal/clean/busy/artistic), subject (people/products/lifestyle/abstract), filter (color treatment/saturation/brightness). Gera Lighting Signature em frase pronta pra prompt em inglês + Camera Signature (modelo, lente, aperture). Output alimenta diretamente os prompts da skill image-generation. Use quando o aluno disser - 'photography signature', 'estilo fotográfico', 'assinatura fotográfica', 'lighting signature', 'camera signature', 'estilo das fotos', 'photography style'. Bloco 3.7 do workflow Formação Branding Visual com IA — depois de voice-tone (reordenada pra 3.6), antes de videography signature.
---

# Photography Signature — Bloco 3.7 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às 15 aulas do M05 (Fotografia), em especial 01 (princípios), 03-04 (descrevendo pessoas e objetos), 05-06 (cor e material), 07-09 (composição), 10-11 (ângulos e shots), 12-13 (luz estúdio e natural), 14 (câmera e lente), 15 (aplicação integrada).

## Propósito

Marca pequena improvisa fotografia: cada peça tem luz diferente, ângulo diferente, mood diferente. Esta skill **trava 4 dimensões** que viram assinatura visual — toda foto da marca daqui pra frente respeita essas 4 decisões. Output é frase-pronta pra colar em prompt em inglês + Camera Signature pra usar consistentemente em Midjourney + Higgsfield.

## Conexão com o curso

- **M05 Aula 01 (O Que é Fotografia de Marca)** — foto serve à marca antes de servir ao olho; consistência > excelência isolada
- **M05 Aulas 03-04 (Descrevendo Pessoas + Objetos)** — vocabulário rico em 6 dimensões (pessoa) + 2 dimensões (objeto)
- **M05 Aulas 12-13 (Iluminação Estúdio + Natural)** — 4 decisões de luz estúdio + 5 cenários canônicos de luz natural (golden hour, blue hour, overcast, direct sunlight, window light)
- **M05 Aula 14 (Câmera, Lente, DoF)** — look digital × filme; 6 famílias de lente; abertura por gênero
- **M05 Aula 15 (Aplicação Integrada — Ferra)** — exemplo canônico: Lighting (window light norte + golden hour híbrido) + Camera (Hasselblad H6D / 80mm / f/2.8 / Kodak Portra)

## Quando acionar

- "Photography signature / estilo fotográfico / assinatura fotográfica"
- "Lighting signature / camera signature / estilo das fotos"

## O que esta skill entrega

`{vault}/marcas/{slug}/bloco-3-7-photography-signature.md` com:

- **As 4 dimensões fotográficas:**
  1. **Lighting** — natural / studio / dramatic / soft (com cenário específico — ex: window light norte, golden hour, overcast)
  2. **Mood** — minimal / clean / busy / artistic / cinematic
  3. **Subjects predominantes** — people / products / lifestyle / abstract / details
  4. **Filter / Color treatment** — warm muted / cool clean / vibrant saturated / naturalist documental / high contrast editorial
- **Lighting Signature em frase pronta** (em inglês, pra colar em prompt):
  > Ex: *"window light from north-facing window, soft directional, slight golden hour warmth, raking light revealing texture, soft shadows under cheekbones, subsurface scattering on skin"*
- **Camera Signature em frase pronta** (em inglês):
  > Ex: *"Hasselblad H6D-50c, 80mm f/2.8, Kodak Portra 400, slight grain, medium format depth, three-quarter framing"*
- **Composition rules** — 3-5 regras compositivas próprias (ex: "sempre regra dos terços, nunca centralizado", "lead room sempre à esquerda quando rosto olha pra direita")
- **3-5 reference shots** documentadas (do moodboard ou de geração-piloto)

**No Figma** (Página Brand Guideline):
- Seção Photography Signature com Lighting + Camera + 3 reference shots renderizadas

## Pré-requisitos

- `bloco-3-1-moodboard.md` (CRÍTICO)
- `bloco-3-4-color-palette.md` (paleta filtra color treatment)
- `bloco-3-5-brand-faces.md` (subjects = brand faces se humanos)
- `figma-file-key.txt`

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. Moodboard + Color Palette + Brand Faces

## Fluxo de execução (~45-60 min)

### Fase 1 — Lighting (M05 Aulas 12-13)
Skill apresenta 5 cenários canônicos de luz natural + 4 decisões de estúdio. Aluno escolhe baseado em moodboard. Define cenário primário + cenário secundário.

### Fase 2 — Mood
Aluno marca 1 mood dominante das opções (minimal / clean / busy / artistic / cinematic). Skill puxa do moodboard pra validar.

### Fase 3 — Subjects predominantes
Quem aparece mais? People (brand faces)? Products? Lifestyle (cenas)? Abstract (texturas, detalhes)? Define 1 dominante + 2 secundários.

### Fase 4 — Filter / Color treatment
Define color grading (M05 Aula 09 — naturalist / warm muted / cool clean / vibrant saturated / high contrast editorial). Bate com paleta.

### Fase 5 — Lighting Signature em frase
Skill destila Fases 1-4 em 1 parágrafo de 30-50 palavras EM INGLÊS pronto pra colar em qualquer prompt. Vocabulário técnico (subsurface scattering, raking light, three-quarter, golden hour) das Aulas 12-13.

### Fase 6 — Camera Signature em frase
Modelo (Hasselblad / Sony / Leica / Canon EOS / Nikon Z9), lente (24mm / 50mm / 85mm / 100mm macro), abertura (f/1.4 / f/2.8 / f/8), film stock se aplicável (Kodak Portra / Cinestill). 1 frase em inglês.

### Fase 7 — Composition rules (3-5)
Decisões compositivas próprias (regra dos terços / lead room / triangulação / aspect ratio dominante).

### Fase 8 — 3-5 reference shots
Skill conduz geração-piloto (no MJ ou Higgsfield) usando Lighting + Camera signatures pra produzir 3-5 fotos de referência. Salva URLs no MD + adiciona no Figma.

## Padrão de comunicação (Contrato B)

PT-BR pra explicar; INGLÊS pra Lighting + Camera Signatures (vão pra prompt). Vocabulário técnico fotográfico atribuído (golden hour, raking light, etc. — referência clássica de fotografia).

## Decisões com o aluno (Contrato C)

- **5 cenários de luz natural:** aluno escolhe primário + secundário
- **Camera (modelo + lente + abertura):** propõe 2-3 combinações, aluno escolhe
- **Reference shots aprovados:** aluno valida cada um

## Output e integração downstream (Contrato D)

CRÍTICO. Consumido por:
- `brand-guideline-builder` (3.10) — Seção 13 (Photography Signature)
- `prompt-builder` (4.2) — auto-injeta Lighting + Camera Signatures em todo prompt
- `image-generation` (4.3) — gera com signatures aplicadas
- `videography-signature` (3.8) — herda lighting (vídeo + foto compartilham luz)

## Quality check (Contrato E)

- 4 dimensões definidas (não só 1-2)?
- Lighting Signature em inglês pronta pra colar em prompt?
- Camera Signature com modelo + lente + abertura concretos?
- 3-5 reference shots gerados e salvos?
- Vocabulário técnico correto (não "luz bonita" — "raking light revealing texture")?

## Antipatterns

1. Lighting Signature em PT-BR — vai gerar bug em MJ/Higgsfield
2. Camera Signature genérica ("DSLR moderna") — IA não tem o que processar
3. Filter contradiz paleta da marca (vibrant em marca de paleta dessaturada)
4. Pular composition rules — peça por peça vai virar improviso
5. Não gerar reference shots — signature fica abstrata, sem prova de funcionamento

## Frase-âncora

> **"Lighting Signature + Camera Signature são as 2 frases mais valiosas da identidade visual. Toda foto da marca daqui pra frente parte delas."**
