---
name: formacao-brand-visual-ia-image-generation
description: Conduz o aluno pela geração de imagens em Higgsfield + Nano Banana 2 (default) ou Midjourney (alternativa) usando o prompt gerado pelo prompt-builder. Cobre workflow completo - Brand Production Process em 5 fases (Brief → Prompt → Generate → Refine → Approve), 5 métodos para fotos de produto (Hero Object Placeholder, Omni Reference, Product Swap, Scene Swap, Background Swap), manter Brand Face consistente com cref, 9 hacks Nano Banana (color/material/product/angle/logo/scene/model/outfit swap + copy-and-seed). Inclui Multi-Reference Workaround V7→V6.1 + scale awareness pra joias. Use quando o aluno disser - 'gerar imagem', 'image generation', 'rodar prompt', 'Higgsfield', 'Nano Banana', 'gerar foto', 'Midjourney profile', 'cref', 'character consistency'. Bloco 4.3 do workflow Formação Branding Visual com IA — depois de prompt-builder, antes de video-prompts.
---

# Image Generation — Bloco 4.3 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às Aulas 08 (Midjourney na Prática), 09 (Imagens de Produto), 10 (Imagens de Modelo), 11 (Biblioteca dos 5 Casos de Uso), 12 (9 Hacks de Edição) do Extra-Ofício.

## Propósito

Prompt está pronto. Esta skill conduz a **geração real** das imagens em Higgsfield (Nano Banana, default) ou Midjourney (alternativa pra quando precisa de Profile + cref consistente). Aplica Brand Production Process em 5 fases + 5 métodos canônicos pra hero shot de produto + 9 hacks Nano Banana.

## Conexão com o curso

- **Extra-Ofício Aula 04 (AI Models vs Plataformas)** — modelo é motor, plataforma é carro
- **Extra-Ofício Aula 05 (Escolhendo a Ferramenta Certa)** — Higgsfield + Midjourney como dupla central
- **Extra-Ofício Aula 08 (Midjourney na Prática)** — Profile training + Moodboards + 3 tipos de referência (Image Prompt / Style Reference / Omni Reference) + Edit tab + parâmetros
- **Extra-Ofício Aula 09 (Imagens de Produto)** — 5 métodos canônicos (Hero Object Placeholder, Omni Reference, Product Swap, Scene Swap, Background Swap)
- **Extra-Ofício Aula 10 (Imagens de Modelo)** — close-up primeiro, character reference, manter brand face
- **Extra-Ofício Aula 11 (Biblioteca de 5 Casos)** — model / product / 3D product / scene / texture
- **Extra-Ofício Aula 12 (9 Hacks Nano Banana)** — color/material/product/angle/logo/scene/model/outfit swap + copy-and-seed

## Quando acionar

- "Gerar imagem / image generation / rodar prompt"
- "Higgsfield / Nano Banana"
- "Gerar foto / Midjourney profile / cref / character consistency"

## O que esta skill entrega

Output salvo em `{vault}/marcas/{slug}/imagens/{nome-do-shot}.md` com:
- URL/seed da imagem aprovada
- Iteration log (quantas variações, quais não funcionaram, qual foi a final)
- Ferramenta usada + método aplicado
- Custo aproximado (créditos consumidos)

## Pré-requisitos

- `brand-guideline-companion.md`
- Prompt do `prompt-builder` (Bloco 4.2)
- Opcional: URL master da Brand Face (pra cref)
- Conta ativa em Higgsfield + opcionalmente Midjourney

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Prompt em mãos
4. Brand face URL (se peça tem pessoa)

## Brand Production Process (5 fases — Extra-Ofício Aulas 09-10)

### Fase 1 — Brief
Aluno define: o que tem que ser preservado vs o que pode variar. Skill ALERTA: "sempre dizer o que preservar".

### Fase 2 — Prompt
Skill puxa do `prompt-builder` ou pede pra rodar.

### Fase 3 — Generate
Skill orienta qual ferramenta usar:
- **Higgsfield (Nano Banana 2) — DEFAULT** pra refinos, hacks, swaps
- **Midjourney V7 com Profile** pra hero shots iniciais e brand face close-up
- **Midjourney V6.1** quando precisa Multi-Reference (workaround V7→V6.1)

### Fase 4 — Refine
Aplica 1+ dos 9 hacks Nano Banana se precisar:
1. Color swap
2. Material swap
3. Product swap
4. Angle change
5. Same image (variação sutil)
6. Add logo
7. Scene swap
8. Model swap
9. Outfit swap

Padrão único pra 8 dos 9: "upload original + instrução natural + dizer o que preservar".

Hack 5 (Copy and Seed) é o único do MJ — usa o seed pra reproduzir a imagem-base e variar.

### Fase 5 — Approve
Aluno aprova URL final. Skill salva em `{vault}/marcas/{slug}/imagens/`.

## 5 métodos pra hero shot de produto (Extra-Ofício Aula 09)

1. **Hero Object Placeholder** — gera cena com objeto-placeholder no MJ, depois substitui pelo produto real via Nano Banana
2. **Omni Reference** — usa imagem do produto como Omni Reference no MJ (`--oref --ow 100-1000`)
3. **Product Swap** — gera cena com produto similar, troca pelo real via Nano Banana
4. **Scene Swap** — produto fixo, troca cenário via Nano Banana
5. **Background Swap** — fundo isolado, mantém produto + iluminação

Skill recomenda método baseado em complexidade do produto + nível de fidelidade necessário.

## Brand Face consistency (Extra-Ofício Aula 10)

- Close-up primeiro (gerar 1 imagem perfeita do rosto)
- Reusa via Nano Banana (mantém mesmo rosto em variações)
- Em MJ: usa `--cref [URL] --cw 100`
- 5 workflows: roupa / joias / produto segurado / interior / set completo
- ⚠️ Scale awareness pra joias — sempre especificar dimensões reais ("8mm ring on adult female ring finger")

## Padrão de comunicação (Contrato B)

PT-BR pra orientação. Quando mostra prompt em inglês, traz tradução `↳` PT-BR de termos técnicos. Cita aulas do Extra-Ofício como fonte.

## Decisões com o aluno (Contrato C)

- **Ferramenta:** propõe Higgsfield ou MJ baseado no caso, aluno escolhe
- **Método pra produto:** propõe 1 dos 5 baseado em fidelidade necessária
- **Aprovação da imagem final:** aluno valida antes de salvar como aprovada

## Output e integração downstream (Contrato D)

Consumido por:
- `video-prompts` (4.4) — usa imagem aprovada como still pra image-to-video
- `static-ads-ecommerce` (4.5) e `ad-video-creator` (4.5) — imagem vai pro creative final no Figma
- `catalog-coherence` (4.6) — primeira imagem aprovada vira "âncora" da coleção
- `figma` (3.11) — handoff pro Figma como conteúdo de frame

## Quality check (Contrato E)

- Lighting + Camera Signatures da marca preservadas?
- Brand Face consistente (se peça tem pessoa)?
- Logo correto (se aparece)?
- Scale correto (especialmente em joias)?
- Salvou URL/seed pra reprodução futura?

## Antipatterns

1. Não dizer "o que preservar" no refinamento (Nano Banana muda elementos não-pedidos)
2. Pular cref em peças com brand face (rosto muda entre imagens — quebra reconhecimento)
3. Esquecer scale em joias (anel vira tamanho de prato)
4. Mencionar Sora / DALL-E / Stable Diffusion como ferramentas oficiais (fora do stack do Kevin)
5. Aprovar imagem com logo errado / produto distorcido (vai pro Figma e descobre o erro depois)
6. Não salvar seed/URL pra reprodução

## Frase-âncora

> **"Brand Production Process: Brief → Prompt → Generate → Refine → Approve. Em cada refinamento: dizer EXPLICITAMENTE o que preservar."**
