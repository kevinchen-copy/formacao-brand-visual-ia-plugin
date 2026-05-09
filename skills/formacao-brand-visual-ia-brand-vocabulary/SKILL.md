---
name: formacao-brand-visual-ia-brand-vocabulary
description: Skill aposentada na v2.0 do plugin. Mantida como stub de redirecionamento pra preservar compatibilidade com invocações antigas. Conteúdo monolítico foi quebrado em 13 skills granulares do Bloco 3 (figma-setup, moodboard, logo-system, typography, color-palette, brand-faces, voice-tone, photography-signature, videography-signature, motion-design, brand-guideline-builder, figma, rapid-prototyping). Use briefing-inicial se a marca é nova ou brand-guideline-builder se você já tem documentos do Bloco 0-3 e quer consolidar.
---

# Brand Vocabulary — APOSENTADA (Stub de Redirecionamento)

> **Esta skill foi aposentada na v0.1.0 do plugin (Onda 1).**
>
> **Mantida apenas pra preservar compatibilidade** com invocações antigas. Se você caiu aqui por engano, leia abaixo pra qual skill usar.

## Por que foi aposentada

Esta skill era um monolito do Mobile Editing Club original (cobria personalidade + cor + tipografia + brand faces + videography + voice & tone numa única entrevista de 5 fases).

A v2.0 do plugin **quebrou esse monolito em 13 skills granulares** do Bloco 3, cada uma profunda o suficiente pra fazer justiça à dimensão correspondente do curso autoral do Kevin Chen:

| Dimensão antiga | Skill nova autoral correspondente |
|---|---|
| Personality | `briefing-inicial` (Bloco 0) + `voice-tone` (Bloco 3) |
| Color & Mood | `color-palette` (Bloco 3) |
| Visual Style Checklist | `moodboard` + `photography-signature` (Bloco 3) |
| Brand Faces | `brand-faces` (Bloco 3) |
| Videography Signature | `videography-signature` (Bloco 3) |
| Voice & Tone | `voice-tone` (Bloco 3) |
| Quick Reference Card | `brand-guideline-builder` consolidado em PDF + Figma + companion MD (Bloco 3) |

## Pra onde te redirecionar

**Se sua marca é NOVA** (ainda não tem briefing nem nada documentado):
→ Use **`formacao-brand-visual-ia-briefing-inicial`** (Bloco 0). Ela conduz a entrevista inicial estruturada e gera o primeiro dossiê.

**Se você já fez Blocos 0-3 e quer CONSOLIDAR tudo num documento único**:
→ Use **`formacao-brand-visual-ia-brand-guideline-builder`** (Bloco 3.10). Ela gera o brand-guideline.md companion + PDF A4 exportado do Figma + DESIGN.md.

**Se você não sabe em que ponto está**:
→ Use **`formacao-brand-visual-ia-maestro`**. Ele faz diagnóstico do estado atual da marca e indica a próxima skill.

**Se você é aluno NOVO da formação e quer fazer assessment antes de começar**:
→ Use **`formacao-brand-visual-ia-diagnostico`**. Brand AI-Readiness Assessment de 20 perguntas.

## Comportamento esperado quando esta skill é invocada

A skill **não conduz a entrevista de 5 fases antiga**. Ela:

1. Reconhece que foi invocada
2. Pergunta ao aluno qual o objetivo dele em 1 frase
3. Roteia pra skill correta acima baseado na resposta
4. Encerra

Não há fluxo de produção próprio. Não gera arquivo `.md`.

## Frase-âncora

> **"Brand Vocabulary monolítico virou 13 skills granulares na v2.0. Granularidade dá controle; monolito dá ilusão de simplicidade. Usa as skills certas — o resultado é mais profundo."**
