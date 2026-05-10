---
name: formacao-brand-visual-ia-typography
description: Conduz o aluno a escolher e estruturar o sistema tipográfico da marca como Text Styles vivos no Figma — família primária (heading), secundária (body), opcionalmente terciária + hierarquia completa H1/H2/H3/Body/Caption/Quote com size, weight, line-height, letter-spacing exatos + pairing tipográfico (3 Cs - Concordante, Conflitante, Contrastante). Aplica taxonomia das Aulas 04-05 do M04 (serif clássica/moderna, sans neutra/geométrica, manuscrita, display, mono). Use quando o aluno disser - 'tipografia', 'fontes', 'família tipográfica', 'pairing', 'heading e body', 'serifa', 'sans serif', 'tipografia da marca'. Bloco 3.3 do workflow Formação Branding Visual com IA — depois de logo-system, antes de color-palette.
---

# Typography — Bloco 3.3 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado à Aula 06 do M02 (Sistema Tipográfico de Marca) + Aulas 04-05 do M04 (Pilar Tipografia I — Anatomia + II — 3 Cs).

## Propósito

Tipografia é o pilar mais subestimado por empreendedor e o mais decisivo na percepção de profissionalismo. Esta skill estrutura a escolha + cria Text Styles VIVOS no Figma (não só decisão num MD) que TODAS as peças do Bloco 4 vão consumir.

## Conexão com o curso

- **M02 Aula 06 (Sistema Tipográfico)** — máximo 3 fontes; hierarquia (headline 2-3x, sub 1.5x, corpo 16-18px, caption 60-70%); safe zones por plataforma; estratégia 2 etapas com IA (gera imagem sem texto, adiciona tipografia em pós); licenciamento (Google Fonts, Adobe Fonts)
- **M04 Aula 04 (Pilar Tipografia I)** — anatomia mínima (5 atributos) + 6 estilos tipográficos canônicos
- **M04 Aula 05 (Pilar Tipografia II — 3 Cs)** — Concordante (igual demais — monótono) / Conflitante (parecido demais — confuso) / **Contrastante** (a regra que funciona)

## Quando acionar

- "Tipografia / fontes / família tipográfica"
- "Pairing / heading e body / sistema tipográfico"
- "Serifa / sans serif"

## O que esta skill entrega

**Text Styles vivos no Figma** (Página 2 — Brand Guideline):
- H1 / Display
- H2 / Title
- H3 / Subtitle
- Body / Default
- Body / Small
- Caption
- Quote / Italic (opcional)

Cada Text Style com font-family, weight, size, line-height, letter-spacing definidos.

**Localmente:**
- `{vault}/marcas/{slug}/bloco-3-3-typography.md` com:
  - Família primária (heading) — escolhida + razão (ancorada no moodboard)
  - Família secundária (body) — escolhida + razão
  - Família terciária opcional (mono / display)
  - Análise de pairing (qual dos 3 Cs)
  - Hierarquia completa documentada
  - Alternativa free (Google Fonts) caso primária seja paga

## Pré-requisitos

- `bloco-3-1-moodboard.md` (CRÍTICO — fontes ressoam o moodboard)
- `bloco-3-2-logo-system.md` (a fonte do logo pode informar a fonte primária)
- `bloco-2-1-big-idea.md`
- `figma-file-key.txt`

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. Moodboard + Logo + Big Idea
3. `figma-file-key.txt`

## Fluxo de execução (~45-60 min)

### Fase 1 — Decisão da família primária
Skill propõe 3-5 famílias baseadas em moodboard + Big Idea, dos 6 estilos canônicos do M04 Aula 04:
- Serifada clássica (Garamond, Caslon, Baskerville) — tradição, autoridade
- Serifada moderna/editorial (Didot, Playfair, Cormorant Garamond) — elegância editorial
- Sans-serifa neutra (Helvetica, Inter, Söhne) — neutralidade, modernidade
- Sans-serifa geométrica (Futura, Avenir, Gotham) — modernidade arquitetônica
- Manuscrita / Script — calor, gesto (CUIDADO — só pra display, nunca corpo)
- Display / Decorativa — statement, ousadia (só pra titular)

Aluno escolhe.

### Fase 2 — Decisão da família secundária (regra dos 3 Cs)
Skill aplica: pairing precisa ser **CONTRASTANTE** (não conflitante). Se primária é serifada, secundária deve ser sans (e vice-versa). Apresenta 2-3 pairs contrastantes que funcionam com a primária escolhida.

### Fase 3 — Família terciária opcional
Se faz sentido (marca tech-design-forward = adicionar Mono pra dados; marca premium = adicionar Display pra capas), define a terceira. Senão, pula.

### Fase 4 — Hierarquia operacional
Define cada nível com size + weight + line-height + letter-spacing. Padrão sugerido (mobile-first):
- H1 / Display: 96-64px (varia)
- H2 / Title: 48-40px
- H3 / Subtitle: 32-24px
- Body / Default: 16-18px
- Body / Small: 14px
- Caption: 12px

### Fase 5 — Criar Text Styles no Figma
Via MCP, criar todos os Text Styles na Página Brand Guideline com naming consistente (H1 / Display, Body / Default, etc.).

### Fase 6 — Alternativa free
Se a fonte escolhida é paga (ex: Cormorant Garamond paga), sugere alternativa Google Fonts ou Adobe Fonts (incluso em assinatura) que tenha vibe similar.

## Padrão de comunicação (Contrato B)

PT-BR. Mostra exemplo de cada decisão com texto-amostra ("A vida começa aqui." renderizada em 3 fontes pra aluno sentir).

## Decisões com o aluno (Contrato C)

- **Família primária:** apresenta 3-5, aluno escolhe
- **Família secundária:** apresenta 2-3 pairs contrastantes, aluno escolhe
- **Terciária Sim/Não:** aluno decide se vale a pena
- **Hierarquia:** propõe padrão, aluno valida (pode ajustar pra mobile-first ou desktop-first)

## Output e integração downstream (Contrato D)

Consumido por:
- `brand-guideline-builder` (3.10) — Seção 7 (Tipografia)
- TODAS as peças do Bloco 4 — usam Text Styles ao colocar texto
- `motion-design` (3.9) — animação respeita line-height e letter-spacing
- `carrossel-estatico` (4.5) — hierarquia tipográfica é estrutura do carrossel

## Quality check (Contrato E)

- Pairing é CONTRASTANTE (passa regra dos 3 Cs)?
- Hierarquia tem 5+ níveis (não só H1 + Body)?
- Text Styles criados no Figma com naming consistente?
- Alternativa free documentada (caso primária paga)?
- Licenciamento esclarecido (Google Fonts = livre; comercial = paga)?

## Antipatterns

1. Pairing CONFLITANTE (duas serifadas parecidas — Garamond + Caslon) — erro mais comum
2. Manuscrita usada em corpo de texto (vira ilegível)
3. 4+ famílias na marca (vira feira de fontes)
4. Text Styles no Figma sem naming sistemático (impossível manter)
5. Não documentar alternativa free (cliente sem orçamento fica travado)
6. Hierarquia chutada sem testar legibilidade em mobile real

## Frase-âncora

> **"Tipografia decide em meio segundo se a pessoa lê ou dá scroll. Não é decoração — é a porta de entrada do conteúdo."**
