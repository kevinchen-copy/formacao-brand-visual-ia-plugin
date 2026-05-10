---
name: formacao-brand-visual-ia-videography-signature
description: Define o cinema da marca em 5 decisões — lighting (mesma da photography ou ajustada pra movimento) + camera signature pra vídeo + pacing (slow contemplativo / médio narrativo / fast dinâmico) + color grading (warm muted / cool clean / vibrant saturated / naturalist documental) + transitions signature (cut direto, fade, dissolve, match cut, whip pan, J/L cut). Output é frase pronta pra alimentar JSON de image-to-video em Higgsfield/Veo/Kling. Use quando o aluno disser - 'videography signature', 'cinema da marca', 'estilo de vídeo', 'pacing', 'color grading', 'transitions', 'video style'. Bloco 3.8 do workflow Formação Branding Visual com IA — depois de photography signature, antes de motion design.
---

# Videography Signature — Bloco 3.8 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às 10 aulas do M06 (Videografia), em especial Aula 04 (9 movimentos), Aula 06 (9 transições), Aula 08 (Videography Style — 5 decisões), Aula 09 (Pacing + Color Grading + Atmosfera), Aula 10 (Aplicação Integrada — Reel da Ferra).

## Propósito

Vídeo é fotografia + tempo. Esta skill estende a Photography Signature pras 5 decisões adicionais que viram a assinatura cinematográfica da marca. Disciplina de consistência transforma qualquer vídeo em reconhecível em 2 segundos sem ver logo nem rosto.

## Conexão com o curso

- **M06 Aula 04 (Movimento de Câmera — 9 Movimentos)** — Static, Tracking, Crane, Pan, Tilt, Zoom, Push-In/Pull-Out, Handheld, Arc
- **M06 Aula 06 (Transitions — 9 Transições)** — Fade, Dissolve, Match Cut, Iris, Wipe, Mask, Whip Pan, Smash Cut, J Cut/L Cut
- **M06 Aula 08 (Videography Style)** — 5 decisões repetidas viram assinatura: Movimento + Pacing + Color Grading + Direct cuts vs creative transitions + B-roll style
- **M06 Aula 09 (Pacing + Color Grading + Atmosfera)** — paradoxo do pacing lento; 4 looks canônicos de color grading; 4 elementos de atmosfera

## Quando acionar

- "Videography signature / cinema da marca / estilo de vídeo"
- "Pacing / color grading / transitions / video style"

## O que esta skill entrega

`{vault}/marcas/{slug}/bloco-3-8-videography-signature.md` com:

- **As 5 decisões cinematográficas:**
  1. **Lighting** — mesma da Photography Signature ou ajustada pra movimento (geralmente herda 80%)
  2. **Camera Signature pra vídeo** — modelo, sensor, lens setup, framing dominante
  3. **Pacing** — slow contemplativo (5+ seg/shot) / médio narrativo (2-4 seg/shot) / fast dinâmico (<2 seg/shot)
  4. **Color Grading** — warm muted / cool clean / vibrant saturated / naturalist documental / high contrast editorial (mesmo da foto pra coerência)
  5. **Transitions Signature** — 2-3 transições assinatura escolhidas dos 9 canônicos (ex: cut direto + match cut + dissolve sutil)

- **Movement repertoire** (3-4 movimentos do repertório oficial — não usar os outros sem motivo): ex: "static dominante + push-in lento + arc 360° em produto premium"

- **B-roll style** — Cinematic / Documentary / Product-focused / Lifestyle (M06 Aula 08)

- **Frase-prompt em inglês** pronta pra alimentar JSON de image-to-video:
  > Ex: *"slow contemplative pacing 5s per shot, warm muted color grading, golden hour lighting carried from photography, smooth cinematic camera movement (push-in slow + static dominante), match cut transitions between hands and product, documentary B-roll style"*

**No Figma** (Página Brand Guideline):
- Seção Videography Signature com 5 decisões + frase-prompt + 1-2 reference Reels (URLs)

## Pré-requisitos

- `bloco-3-7-photography-signature.md` (CRÍTICO — herda lighting + camera + grading)
- `bloco-3-1-moodboard.md`
- `bloco-2-1-big-idea.md` (pacing reflete velocidade emocional da marca)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. Photography Signature + Moodboard + Big Idea

## Fluxo de execução (~45 min)

### Fase 1 — Lighting (herda da Photography)
Confirma se mantém igual à fotografia ou ajusta. Geralmente herda 90%.

### Fase 2 — Camera Signature pra vídeo
Modelo (RED Komodo / Sony FX3 / Canon C70 / iPhone 15 Pro Max), lens setup (anamorphic / spherical / wide / standard), framing dominante (medium close-up / wide cinematic).

### Fase 3 — Pacing (a decisão mais estratégica)
Slow contemplativo (luxo, quiet luxury, marca premium) / Médio narrativo (lifestyle, BTS) / Fast dinâmico (esporte, ad agressivo). Skill avisa do paradoxo do pacing lento (M06 Aula 09): "ritmo lento exige cena bonita".

### Fase 4 — Color Grading
Mesmo da foto pra coerência. Especifica highlights (clipped / rolled off) e sombras (crushed / lifted).

### Fase 5 — Transitions Signature
Escolhe 2-3 transições assinatura dos 9 canônicos (M06 Aula 06). Default recomendado: cut direto + 1 expressiva (match cut OU whip pan OU dissolve).

### Fase 6 — Movement repertoire (3-4 dos 9)
Quais movimentos a marca USA frequentemente? Quais EVITA? Disciplina protege contra "câmera mexendo sem motivo" (M06 Aula 04).

### Fase 7 — B-roll style
Cinematic / Documentary / Product-focused / Lifestyle. Cada um tem gramática diferente.

### Fase 8 — Frase-prompt em inglês
Skill destila as 5 decisões em 1 parágrafo de 50-80 palavras pronto pra colar em JSON de image-to-video da skill `video-prompts` (4.4).

### Fase 9 — Reference Reels (1-2)
Aluno aponta 1-2 Reels de marcas-referência (Aesop, Apple, Liquid Death, Rolex etc.) que materializam a assinatura. Salva URLs.

## Padrão de comunicação (Contrato B)

PT-BR pra explicar; INGLÊS pra frase-prompt. Vocabulário cinematográfico técnico (push-in, dolly, anamorphic, J cut/L cut) atribuído.

## Decisões com o aluno (Contrato C)

- **Pacing:** decisão mais estratégica — aluno define
- **Camera Signature:** propõe 2-3 setups, aluno escolhe
- **Transitions:** propõe 2-3 dos 9, aluno escolhe a assinatura

## Output e integração downstream (Contrato D)

Consumido por:
- `brand-guideline-builder` (3.10) — Seção 14 (Videography Signature)
- `motion-design` (3.9) — pacing do motion respeita pacing do vídeo
- `video-prompts` (4.4) — frase-prompt vai pra JSON
- `edicao` (4.7) — CapCut respeita pacing + transitions + grading

## Quality check (Contrato E)

- 5 decisões definidas (não 2-3)?
- Pacing escolhido com lucidez (não "médio" como default por preguiça)?
- Transitions Signature limita a 2-3 (não usa as 9)?
- Frase-prompt em inglês pronta pra colar em JSON?
- 1-2 reference Reels documentadas?

## Antipatterns

1. Pacing "médio" sem decisão consciente — perde personalidade
2. Usar todos os 9 movimentos — vira improviso, sem assinatura
3. Color grading diferente da foto — quebra coerência marca
4. Frase-prompt em PT-BR — vai gerar bug em Higgsfield/Veo/Kling
5. B-roll style ambíguo — Reel fica em terra-de-ninguém
6. Mencionar Sora/Pika/Runway/Luma como ferramentas oficiais (fora do stack do Kevin — ele usa Higgsfield + Veo + Kling)

## Frase-âncora

> **"Videografia de marca é fotografia + tempo + ritmo + som. A diferença está em disciplina de decisão repetida. Alguém viu 2 segundos do seu Reel sem ver logo, sem ver rosto, e já sabe que é seu."**
