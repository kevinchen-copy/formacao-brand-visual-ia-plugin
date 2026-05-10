---
name: formacao-brand-visual-ia-platform-adaptation
description: Adapta pacote-âncora (Reel + hero shot + carrossel) pras plataformas USADAS pela marca (Instagram, Newsletter, Site, Pinterest) e EXPRESSAMENTE recusa publicar nas EVITADAS (TikTok, LinkedIn) salvo override explícito do aluno. Aplica matriz CORE × EXECUTION (5 elementos permanentes da marca × 7 dimensões variáveis - polish/pace/caption/tom/format/audio/logo use). Orquestra 3 trilhas (Figma para post/story/carrossel/reel cover, Claude Design para hero piece de site, edicao para Reel). Output são variantes exportadas + caption específica por plataforma + quality check de exclusão. Use quando o aluno disser - 'adaptação multiplataforma', 'platform adaptation', 'adaptar Reel pra Stories', 'cross-platform', 'newsletter da marca', 'adaptar conteúdo'. Bloco 4.8 do workflow Formação Branding Visual com IA — última skill da produção do bloco 4.
---

# Platform Adaptation — Bloco 4.8 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado à Aula 10 do M02 (Adaptação por Ponto de Contato).

## Propósito

Aluno produziu peça-âncora (Reel + hero shot + carrossel). Esta skill **adapta** pras plataformas que a marca USA (Instagram, Newsletter, Site, Pinterest) e **recusa explicitamente** publicar nas EVITADAS (TikTok, LinkedIn) salvo override consciente do aluno. Aplica matriz CORE × EXECUTION pra manter coerência da marca enquanto otimiza por plataforma.

## Conexão com o curso

- **M02 Aula 10 (Adaptação por Ponto de Contato)** — núcleo fixo (cor/fonte/rosto/motion/voz) é inegociável; camada adaptável (formato/pacing/polimento/tom) muda por plataforma; "melhor excelente em duas que medíocre em cinco"

## Quando acionar

- "Adaptação multiplataforma / platform adaptation"
- "Adaptar Reel pra Stories / cross-platform"
- "Newsletter da marca / adaptar conteúdo"

## O que esta skill entrega

`{vault}/marcas/{slug}/multiplataforma/{nome-da-peca}/` com:
- **Reel principal (9:16)** — vai pra IG Reels
- **Hero shot estático (1:1 ou 4:5)** — IG Feed
- **Carrossel slides (4:5)** — IG Feed (montado no Figma)
- **Stories cards (9:16)** — sequência de 3-5 cards (Figma)
- **Reel cover (9:16)** — thumbnail otimizada (Figma)
- **Pinterest pins (2:3)** — 3 versões (Figma)
- **Hero de site / manifesto / one-pager** — via `rapid-prototyping` (Claude Design)
- **Newsletter HTML** — versão pra base de email
- **captions.md** — caption específica por plataforma (tom + comprimento ajustados)

## Matriz CORE × EXECUTION (M02 Aula 10)

### CORE (5 elementos permanentes — NÃO mudam entre plataformas)
1. Paleta de cores
2. Tipografia
3. Brand face (rosto)
4. Motion identity
5. Voice & Tom (voz permanente)

### EXECUTION (7 dimensões variáveis por plataforma)
1. **Polish** — Instagram polido / Newsletter formal / Site editorial
2. **Pace** — Reel 30s slow contemplativo / Stories 15s mais punchy
3. **Caption length** — IG curta-média / Newsletter longa / Pinterest descritiva
4. **Tom** — voz permanente, tom modula por plataforma (mais íntimo no Newsletter, mais celebrativo no IG)
5. **Format** — 9:16 / 1:1 / 4:5 / 2:3 / HTML
6. **Audio** — som no Reel / silencioso no Newsletter / sons curtos no Stories
7. **Logo use** — sutil no IG (não grita) / explícito no Newsletter / médio no Pinterest

## Pré-requisitos

- `brand-guideline-companion.md`
- Pacote-âncora gerado (Reel + hero shot + carrossel)
- `figma-file-key.txt`

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Pasta com pacote-âncora pronto

## Plataformas USADAS por default

- **Instagram** — Reels, Feed, Stories
- **Newsletter** — email da base
- **Site** — hero piece, manifesto, one-pager
- **Pinterest** — 2:3 pins

## Plataformas EVITADAS por default

- **TikTok** — recusa publicar (regra do brand guideline padrão)
- **LinkedIn** — recusa publicar (regra do brand guideline padrão)

⚠️ Skill PERGUNTA antes de adaptar pra plataformas evitadas. Se aluno tem motivo legítimo (campanha pontual, parceria), permite override + alerta sobre quebra de regra do brand guideline.

## Fluxo de execução (~30-45 min por pacote)

### Fase 1 — Confirmar plataformas-alvo
Skill lista USADAS + EVITADAS do brand guideline. Aluno confirma.

### Fase 2 — Aplicar matriz CORE × EXECUTION
Pra cada plataforma escolhida, decide:
- O que do CORE se mantém (sempre tudo)
- O que da EXECUTION ajusta

### Fase 3 — 3 trilhas paralelas
- **Trilha Figma:** orquestra `figma` (3.11) pra montar post-feed, story, reel-cover, carousel-base, pinterest-pin nos templates
- **Trilha Claude Design:** orquestra `rapid-prototyping` (3.12) pra hero piece de site / manifesto / one-pager
- **Trilha edicao:** orquestra `edicao` (4.7) pra adaptar MP4 do Reel pra versão Story (cortes diferentes) + Reel cover

### Fase 4 — Captions específicas
Pra cada plataforma, caption ajustada:
- IG Feed: 80-150 palavras, hashtags relevantes ao final
- Stories: 5-10 palavras por card, sequencial
- Newsletter: 200-400 palavras, tom mais íntimo
- Pinterest: descritiva 100-200 palavras, focada em searchability

### Fase 5 — Quality check de EXCLUSÃO
Verifica que NÃO publicou em plataformas evitadas. Se publicou (override consciente), documenta razão em `multiplataforma/{nome}/override-log.md`.

### Fase 6 — Salvar exports + log
Estrutura final em `multiplataforma/{nome-da-peca}/` com TODAS as variantes + captions.md + override-log.md (se aplicável).

## Padrão de comunicação (Contrato B)

PT-BR. Ao recusar plataforma evitada, é firme mas educado: "Brand guideline marca TikTok como evitada. Quer override pontual ou pulamos?"

## Decisões com o aluno (Contrato C)

- **Override de plataforma evitada:** sempre pergunta antes
- **Caption por plataforma:** propõe rascunho, aluno aprova
- **Trilha por plataforma:** Figma vs Claude Design vs edicao — recomenda baseado no que está produzindo

## Output e integração downstream (Contrato D)

Produto final do Bloco 4. Não tem skill downstream — o pacote multiplataforma vai pras plataformas reais (publicação fora do plugin).

## Quality check (Contrato E)

- Plataformas USADAS atendidas com variantes específicas?
- Plataformas EVITADAS recusadas (ou override documentado)?
- 5 elementos CORE preservados em TODAS as variantes?
- 7 dimensões EXECUTION ajustadas por plataforma?
- Captions específicas por plataforma (não copy-paste)?
- Aspect ratios + safe zones corretos?

## Antipatterns

1. Publicar em TikTok/LinkedIn sem perguntar (override silencioso quebra brand guideline)
2. Mesma caption em todas as plataformas — perde otimização
3. Copy-paste do Reel pro Stories sem cortar (Stories é vertical mas duração diferente)
4. Esquecer Pinterest — 2:3 vertical não é trivial de adaptar do feed quadrado
5. Ignorar Newsletter (alguns alunos esquecem que email é canal de marca, não só promoção)
6. Aplicar Polish "máximo" em TikTok orgânico (vira ad, perde nativo) — mas como TikTok é evitado por default, esse antipattern só aparece em override

## Frase-âncora

> **"Adaptação multiplataforma não é multiplicar conteúdo — é decidir onde NÃO publicar. Núcleo fixo, execução ajustada, exclusão documentada."**
