---
name: formacao-brand-visual-ia-static-ads-ecommerce
description: Gera copy de ads estáticos para e-commerce filtrando 10 tipos disponíveis (Direct Offer, Benefit-First, Social Proof, PAS, Story/Narrative, Curiosity, Insider Education, Bundle/Threshold, Scarcity, Lifestyle/Aspirational) automaticamente baseado no Brand Guideline da marca ativa. Skill RECUSA gerar tipos que violam Big Idea ou vocabulário proibido. Inclui modo embutido de UGC/Founder-led (Aula 07 do Extra-Copy) e Hooks short-form (Aula 06). Output são 3 copies (1 de cada tipo recomendado) com Headline ≤12 palavras + Body ≤125 chars + CTA + visual overlay specs + handoff Figma pra montar ad. Use quando o aluno disser - 'ads de e-commerce', 'copy de ad estático', 'ads pra Meta', 'static ads', 'copy de conversão', 'ads de produto', 'criar ads', 'UGC ad', 'founder-led ad'. Bloco 4.5 do workflow Formação Branding Visual com IA — junto com ad-video-creator.
---

# Static Ads E-commerce — Bloco 4.5 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às 14 aulas do Extra-Copy-pra-E-commerce, em especial Aulas 02 (5 níveis de consciência), 03 (5 frameworks), 04 (anatomia do ad de Meta), 05 (10 tipos de copy), 06 (hooks short-form), 07 (UGC + founder-led).

## Propósito

Static ads dominam 60-70% das conversões de e-commerce (segundo casos do Extra-Copy). Esta skill gera copy de ads estáticos filtrando 10 tipos disponíveis baseado no Brand Guideline. **RECUSA tipos que violam Big Idea ou vocabulário proibido** (ex: marca quiet luxury bloqueia automaticamente Direct Offer e PAS agressivo). Inclui modos embutidos de UGC e Hooks short-form.

## Conexão com o curso

- **Extra-Copy Aula 02 (5 níveis de consciência DTC)** — Schwartz adaptado: cold = N2-3, retargeting = N4
- **Extra-Copy Aula 03 (5 frameworks de copy DTC)** — PAS / BAB / FAB / AIDA / 4 Us como filtro final
- **Extra-Copy Aula 04 (Anatomia do ad de Meta)** — Hook + Mecanismo + Prova + Reversão de risco + CTA
- **Extra-Copy Aula 05 (10 tipos de copy de ad estático)** — Direct Offer, Benefit-First, Social Proof, PAS, Story, Curiosity, Insider Education, Bundle/Threshold, Scarcity, Lifestyle/Aspirational
- **Extra-Copy Aula 06 (Hooks pra TikTok e short-form)** — modo embutido pra hooks de vídeo curto
- **Extra-Copy Aula 07 (UGC e founder-led)** — modo embutido pra ads UGC

## Quando acionar

- "Ads de e-commerce / copy de ad estático / static ads"
- "Ads pra Meta / copy de conversão / criar ads"
- "UGC ad / founder-led ad" (modo embutido)
- "Hooks pra TikTok / hooks short-form" (modo embutido)

## Os 10 tipos de ad estático (Extra-Copy Aula 05)

1. **Direct Offer** — "20% off hoje só" — direto na conversão
2. **Benefit-First** — benefício chave em headline
3. **Social Proof** — "1.300+ clientes mudaram" — prova social explícita
4. **PAS** — Problema → Agitação → Solução
5. **Story / Narrative** — micronarrativa em 1-2 frases
6. **Curiosity** — gancho de curiosidade que abre loop
7. **Insider Education** — "5 perguntas que separam X de Y" — autoridade educativa
8. **Bundle / Threshold** — "Compre X, ganhe Y" / "frete grátis acima de R$200"
9. **Scarcity** (REAL — nunca fake) — "47 peças restantes"
10. **Lifestyle / Aspirational** — brand face em cena cotidiana com produto

## O que esta skill entrega

`{vault}/marcas/{slug}/ads/{nome-do-ad}-{data}.md` com:

- **3 copies** (1 de cada tipo recomendado pra essa marca):
  - Headline ≤12 palavras
  - Body ≤125 chars (caption Meta)
  - CTA específico (não "saiba mais")
  - Visual overlay specs (qual texto vai sobreposto na imagem, posicionamento, font, color)
- **Variantes A/B testáveis** (mudando 1 elemento por variante — headline, hook visual ou CTA)
- **Lista de tipos BLOQUEADOS** com razão (transparência editorial)
- **Handoff Figma** — instruções pra `figma` (3.11) montar o ad final com:
  - Imagem aprovada (do `image-generation`)
  - Copy aprovada
  - Logo via Component instance
  - Templates da Página 7 (Ad Estático)

## Modos embutidos

### Modo UGC / Founder-led (Aula 07 Extra-Copy)
Quando aluno pede "ad UGC" ou "founder-led":
- Estrutura de 5 linhas (contexto pessoal + tentativa anterior fracassada + encontro sem hype + resultado específico + recomendação contida)
- 5 anti-padrões evitados (sem adjetivos cumulativos, sem !, sem simetria, sem CTA explícito, sem linguagem de marca)
- Vulnerabilidade controlada da founder

### Modo Hooks Short-form (Aula 06 Extra-Copy)
Quando aluno pede "hooks pra TikTok" / "hooks short-form" (ainda que TikTok seja evitado por default — pode ser pra Reels orgânicos):
- 5 tipos de hook (padrão visual quebrado, pergunta-incômodo, afirmação polêmica, revelação visual, fala humana)
- Payoff específico (anti-clickbait)
- 5 erros mortais evitados

## Pré-requisitos

- `brand-guideline-companion.md` (CRÍTICO — Big Idea + vocabulário proibido + Do's & Don'ts)
- Imagem/produto-alvo (URL aprovada via `image-generation` ou própria foto do produto)
- Definição da peça (cold / retargeting / retenção / lançamento)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Imagem/produto-alvo

## Fluxo de execução (~20-30 min por set de 3 ads)

### Fase 1 — Identificar estágio de funil
Cold (N2-N3) / Retargeting (N4) / Retenção (N5). Define quais dos 10 tipos fazem sentido.

### Fase 2 — Filtrar 10 tipos contra Brand Guideline
Skill lê voz da marca + vocabulário proibido + Big Idea. Bloqueia tipos que violam:
- Marca quiet luxury bloqueia Direct Offer + PAS agressivo + Scarcity
- Marca founder-led pode preferir Story + UGC sobre Social Proof "X clientes"
- Marca educativa prioriza Insider Education

### Fase 3 — Selecionar 3 tipos recomendados
Dos não-bloqueados, escolhe 3 que cobrem ângulos diferentes (ex: Story + Insider Education + Lifestyle = jornada de funil completa).

### Fase 4 — Gerar 3 copies
Pra cada tipo:
- Headline ≤12 palavras com 4 Us aplicados (Útil + Urgente + Único + Ultra-específico)
- Body ≤125 chars
- CTA específico
- Visual overlay specs

### Fase 5 — Variantes A/B
Pra cada copy, propõe 1-2 variações mudando 1 elemento.

### Fase 6 — Handoff pro Figma
Skill prepara instruções pra `figma` (3.11) montar o ad final:
- Qual template usar (Página 7)
- Onde posicionar copy
- Qual Color Variable aplicar
- Qual Text Style usar

### Fase 7 — Documentar tipos BLOQUEADOS
Lista os tipos não-recomendados com razão (transparência editorial).

## Padrão de comunicação (Contrato B)

PT-BR. Quando bloqueia um tipo, explica POR QUÊ ("Direct Offer foi bloqueado porque sua marca posiciona como contemplativa — descontos agressivos quebrariam Big Idea").

## Decisões com o aluno (Contrato C)

- **3 tipos selecionados:** propõe baseado em filtro, aluno aprova/troca
- **Variantes A/B:** propõe, aluno escolhe quais testar
- **Override de tipo bloqueado:** se aluno insiste em usar Direct Offer numa marca que bloqueia, alerta que quebra brand guideline

## Output e integração downstream (Contrato D)

Consumido por:
- `figma` (3.11) — monta ad final no template Ad Estático
- `platform-adaptation` (4.8) — adapta ads pros canais (Meta vs Pinterest têm diferenças)

## Quality check (Contrato E)

- Tipos selecionados ressoam com estágio de funil?
- Tipos BLOQUEADOS documentados com razão?
- Headlines ≤12 palavras, body ≤125 chars?
- 4 Us aplicados em cada headline?
- Variantes A/B mudam só 1 elemento?
- Vocabulário proibido NÃO aparece em nenhum copy?

## Antipatterns

1. Gerar copy ignorando voz da marca — vira ad genérico
2. Usar todos os 10 tipos — perde foco, marca dispersa
3. Scarcity FAKE ("últimas peças" quando não é) — destrói confiança quando descoberto
4. CTA genérico ("saiba mais") — perde 30-50% de conversão vs CTA específico
5. Caption que ignora limite de char do Meta — vira "..." truncado
6. Pular handoff Figma — copy fica no MD, não vira creative final

## Frase-âncora

> **"Static ads dominam 60-70% das conversões e-commerce. Mas só funcionam quando o tipo bate com a marca. Filtragem de tipo > criatividade pontual."**
