---
name: formacao-brand-visual-ia-voice-tone
description: Define a voz e tom da marca em 2 camadas — voz permanente (3 adjetivos que NÃO mudam) + tom variável por contexto (lançamento / educativo / suporte / crise). Inclui vocabulário favorito (10-15 palavras) + vocabulário proibido (10-15 palavras saturadas a evitar) + regras de copy (frases curtas, pausa, sem ponto de exclamação, sem adjetivos cumulativos, etc). Output é Voice & Tone Matrix completa pronta pra alimentar todas as skills de copy. Use quando o aluno disser - 'voz da marca', 'tom de voz', 'voice and tone', 'vocabulário da marca', 'palavras proibidas', 'regras de copy', 'voice tone'. Bloco 3.6 do workflow Formação Branding Visual com IA — REORDENADA na v0.3.0 pra antes de photography-signature (decisão D).
---

# Voice & Tone — Bloco 3.6 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — REORDENADA na v0.3.0: agora vem ANTES de `photography-signature`. Voz da marca define ESTÉTICA, não o contrário.
>
> Alinhado à Aula 03 do M04 (Pilar Verbo) + Aula 11 do M02 (Brand Guidelines — Voz e Tom) + Aula 15 do M01 (Copy e Microcopy).

## Propósito

Marca confunde **voz** (permanente — quem ela É) com **tom** (variável — como ela MODULA por contexto). Esta skill estrutura as 2 camadas + vocabulário favorito/proibido + regras concretas de copy. Output alimenta TODAS as skills de copy do Bloco 4 (static-ads, ad-video, email-flows, organico-diario, carrossel-estatico).

## Conexão com o curso

- **M04 Aula 03 (Pilar Verbo)** — naming, slogan, manifesto, tom de voz vêm ANTES de tipografia/cor/forma
- **M02 Aula 11 (Brand Guidelines)** — voz e tom como seção do brand book; "se a marca fosse pessoa", "minha marca nunca"
- **M01 Aula 15 (Copy e Microcopy)** — Regra dos 4 U's, hierarquia, edição "até doer"

## Quando acionar

- "Voz da marca / tom de voz / voice and tone"
- "Vocabulário da marca / palavras proibidas"
- "Regras de copy / voice tone"

## O que esta skill entrega

`{vault}/marcas/{slug}/bloco-3-6-voice-tone.md` com:

- **VOZ PERMANENTE** (3 adjetivos que NÃO mudam):
  - Adjetivo 1 — definição operacional + exemplo
  - Adjetivo 2 — idem
  - Adjetivo 3 — idem
  - 3 anti-adjetivos (a marca NÃO é) — protege contra dispersão

- **TOM × 4 CONTEXTOS:**
  - Tom em LANÇAMENTO (ar de novidade, sem estridência)
  - Tom EDUCATIVO (didático sem condescendência)
  - Tom em SUPORTE (acolhedor, resolutivo, sem floreio)
  - Tom em CRISE (transparente, responsável, sem defensiva)

- **VOCABULÁRIO FAVORITO** (10-15 palavras que aparecem repetidas vezes — viram assinatura)

- **VOCABULÁRIO PROIBIDO** (10-15 palavras saturadas no mercado a EVITAR — vêm do market-mapping):
  - Exemplo em joalheria autoral BR 2026: "artesanal", "curadoria", "lote único", "feito à mão", "exclusivo", "premium"
  - Exemplo em skincare BR: "incrível", "imperdível", "fórmula revolucionária"

- **REGRAS DE COPY** (5-8 regras concretas):
  - Sentence length (curtas / médias / longas)
  - Pontuação (! permitido? CAIXA ALTA permitida?)
  - Verbos no presente / passado
  - Pontuação que abre vs fecha
  - Uso de listas vs prosa

- **3-5 EXEMPLOS PAREADOS** (on-brand × off-brand) — mostrando a mesma frase escrita certa e errada

## Pré-requisitos

- `bloco-2-1-big-idea.md` (CRÍTICO — voz deriva da Big Idea)
- `bloco-2-2-positioning.md`
- `bloco-2-3-ideal-client.md` (vocabulário do F1 vira voz)
- `bloco-2-4-tribe-enemy.md` (vocabulário do inimigo = vocabulário proibido)
- `bloco-1-2-market-mapping.md` (palavras saturadas = vocabulário proibido)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. Big Idea + Positioning + Ideal Client + Tribe-Enemy + Market Mapping

## Fluxo de execução (~45-60 min)

### Fase 1 — Voz permanente (3 adjetivos)
Skill propõe 5-7 adjetivos baseados em Big Idea + posicionamento. Aluno escolhe 3. Pra cada um, definição operacional ("contemplativa significa: pausa antes de afirmar; sem urgência artificial").

### Fase 2 — 3 anti-adjetivos
Aluno define 3 adjetivos que a marca NÃO é. Cada um é uma REGRA de não-fazer.

### Fase 3 — Tom × 4 contextos
Pra cada um dos 4 contextos (lançamento / educativo / suporte / crise), define como o tom MODULA mantendo a voz permanente. Skill mostra exemplo.

### Fase 4 — Vocabulário favorito (10-15 palavras)
Lista palavras que vão se repetir consistentemente — viram assinatura linguística.

### Fase 5 — Vocabulário proibido (10-15 palavras)
Skill puxa palavras saturadas do market-mapping + vocabulário do inimigo do tribe-enemy. Aluno aprova.

### Fase 6 — Regras de copy (5-8)
Decisões concretas: frases curtas? Exclamação permitida? Etc.

### Fase 7 — 3-5 exemplos pareados
Pra cada regra crítica, exemplo de frase ON-brand × OFF-brand. Treina o aluno (e a IA) no diferencial.

## Padrão de comunicação (Contrato B)

PT-BR. Aplica o próprio voice-tone ao escrever a documentação (skill demonstra com a própria voz). Sem exemplos genéricos — usa Big Idea da marca ativa.

## Decisões com o aluno (Contrato C)

- **3 adjetivos da voz:** propõe 5-7, aluno escolhe 3
- **Anti-adjetivos:** propõe baseado em tribe-enemy + ideal-client (auto-imagem evitada)
- **Vocabulário favorito vs proibido:** aluno aprova listas

## Output e integração downstream (Contrato D)

CRÍTICO. Consumido por:
- `brand-guideline-builder` (3.10) — Seção 13 (Voice & Tom)
- `static-ads-ecommerce` (4.5) — recusa tipos de ad que violam voz
- `ad-video-creator` (4.5) — voiceover respeita voz
- `email-flows` (4.5) — copy de cada email
- `carrossel-estatico` (4.5) — texto dos slides
- `organico-diario` (4.5) — caption de cada post
- `tribe-enemy` (atualização) — peças manifesto usam voz
- TODA peça com texto do Bloco 4

## Quality check (Contrato E)

- 3 adjetivos com definição operacional (não só palavra)?
- 3 anti-adjetivos explícitos?
- 4 contextos × tom documentados?
- Vocabulário favorito (10+) e proibido (10+) listados?
- 5-8 regras concretas (não vagas)?
- 3-5 exemplos pareados (on-brand × off-brand)?

## Antipatterns

1. Voz com 7 adjetivos (vira lista de virtudes — não filtra nada)
2. Tom igual em todos os contextos (perde modulação)
3. Vocabulário favorito genérico ("autenticidade", "qualidade") — saturado em qualquer mercado
4. Vocabulário proibido sem ancorar no market-mapping (chute)
5. Regras vagas ("seja humano") — não operacionalizam
6. Não criar exemplos pareados (regra fica abstrata)

## Frase-âncora

> **"Voz é permanente. Tom varia. Vocabulário protege. Quem documenta os 3 evita que a marca soe diferente em cada peça de copy."**
