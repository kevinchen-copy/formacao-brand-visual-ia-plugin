---
name: formacao-brand-visual-ia-color-palette
description: Conduz o aluno a construir a paleta cromática da marca como Color Variables vivas no Figma — primárias (2-3 cores), secundárias (1-2 acentos), neutras (background, texto), alertas opcionais (success/warning/error pra interfaces). Cada cor com HEX + RGB + CMYK + Pantone aproximado + caso de uso + emoção. Aplica harmonia cromática (complementar, análoga, monocromática, tríade) + verifica acessibilidade AA/AAA contra branco e preto. Cria Color Variables na Variable Collection 'Brand Tokens' criada pelo figma-setup. Use quando o aluno disser - 'paleta', 'paleta cromática', 'cores da marca', 'color palette', 'HEX da marca', 'cor primária', 'acento', 'harmonia cromática', 'cores'. Bloco 3.4 do workflow Formação Branding Visual com IA — depois de tipografia, antes de brand faces.
---

# Color Palette — Bloco 3.4 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado à Aula 05 do M02 (Paleta de Cores da Marca) + Aulas 07-08 do M04 (Pilar Cor I — Fundamentos + II — Harmonias e Psicologia).

## Propósito

Paleta da marca não é "minhas cores favoritas" — é sistema de Color Variables vivas no Figma com camadas (primárias / secundárias / neutras / alertas), harmonia cromática nomeada, regra 60-30-10 documentada e acessibilidade verificada. Skills do Bloco 4 leem essas Variables e aplicam automaticamente.

## Conexão com o curso

- **M02 Aula 05 (Paleta de Cores)** — primeiro elemento que o público reconhece no scroll; regra das 2-3 primárias; documentação com HEX + coluna "sentimento"; estrutura primárias/secundárias/neutras; regra 60-30-10; fim da era "sad beige"
- **M04 Aula 07 (Pilar Cor I — Fundamentos)** — círculo cromático, 3 dimensões (matiz/saturação/brilho), temperatura, sistemas técnicos (HEX/RGB/CMYK/Pantone)
- **M04 Aula 08 (Pilar Cor II — Harmonias e Psicologia)** — 4 famílias de harmonia + psicologia das cores principais

## Quando acionar

- "Paleta / paleta cromática / cores da marca"
- "Color palette / HEX da marca"
- "Cor primária / acento / harmonia cromática"

## O que esta skill entrega

**Color Variables no Figma** (Variable Collection "Brand Tokens" da Página Brand Guideline):
- 2-3 Primárias (`Primary/Color-Name`)
- 1-2 Secundárias / Acento (`Accent/Color-Name`)
- 2-3 Neutras (`Neutral/Background`, `Neutral/Text-Primary`, `Neutral/Text-Secondary`)
- 3-4 Alertas opcionais (`Alert/Success`, `Alert/Warning`, `Alert/Error`, `Alert/Info`)
- Cada Variable com HEX exato

**Localmente:**
- `{vault}/marcas/{slug}/bloco-3-4-color-palette.md` com:
  - Paleta documentada com HEX + RGB + CMYK + Pantone aproximado + emoção + caso de uso por cor
  - Harmonia nomeada (Complementar / Análoga / Monocromática / Tríade)
  - Regra 60-30-10 aplicada (qual cor é 60% / 30% / 10%)
  - Tabela de acessibilidade WCAG (cada cor primária × branco e preto = AA ou AAA?)
  - 3 paletas alternativas que foram consideradas e descartadas (com razão)

## Pré-requisitos

- `bloco-3-1-moodboard.md` (CRÍTICO — paleta destila moodboard)
- `bloco-2-1-big-idea.md`
- `bloco-3-2-logo-system.md` (cor do logo é parte da primária geralmente)
- `figma-file-key.txt`

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. Moodboard + Big Idea + Logo
3. `figma-file-key.txt`

## Fluxo de execução (~45-60 min)

### Fase 1 — Destilação do moodboard
Skill extrai do moodboard as 5-7 cores recorrentes. Mostra histograma visual ao aluno.

### Fase 2 — Decisão de temperatura dominante
Quente / Fria / Neutra dominante (M04 Aula 07). Marca raramente é equilibrada — escolha estratégica.

### Fase 3 — Escolha da harmonia
Apresenta 4 opções (Monocromática / Análoga / Complementar / Tríade) com prós/contras pra esta marca específica.

### Fase 4 — Decisão das primárias (2-3)
Aluno escolhe 2-3 HEX primários. Skill verifica que cada um:
- Bate com Big Idea + posicionamento + auto-imagem do F1
- Foge da saturação do mercado (lista do market-mapping)
- Funciona em escala (favicon 16px → outdoor)

### Fase 5 — Secundárias / Acento (1-2)
Cores de destaque pra CTAs, momentos pontuais. Geralmente complementar à primária.

### Fase 6 — Neutras (2-3)
Background (raramente branco puro — geralmente off-white quente ou frio); texto primário (raramente preto puro — geralmente carvão muito escuro); texto secundário (cinza médio).

### Fase 7 — Alertas opcionais
Pra marcas com interface digital (site, app), define cores de Success / Warning / Error / Info.

### Fase 8 — Acessibilidade WCAG
Pra cada cor primária + secundária, verifica contraste contra branco e preto (AA mínimo 4.5:1 / AAA 7:1). Documenta resultado.

### Fase 9 — Regra 60-30-10
Define qual cor ocupa 60% (geralmente neutra dominante), 30% (primária), 10% (acento). Cria swatches HTML pra preview.

### Fase 10 — Criar Color Variables no Figma
Via MCP, criar todas as Variables na Collection "Brand Tokens" com naming consistente.

## Padrão de comunicação (Contrato B)

PT-BR. Sempre nomear cor com nome próprio + HEX (ex: "Pedra Bruta #2C1F1A" — não só "marrom escuro"). Cita psicologia das cores com referência (Jung / Eva Heller / Gestalt cromática) quando relevante.

## Decisões com o aluno (Contrato C)

- **Harmonia:** apresenta 4 opções, aluno escolhe
- **Cor primária dominante:** propõe 2-3 candidatas baseadas em moodboard, aluno escolhe
- **Pantone (CMYK):** se aluno é digital-first, opcional; se imprime, obrigatório

## Output e integração downstream (Contrato D)

Consumido por:
- `brand-guideline-builder` (3.10) — Seção 8 (Paleta de Cores)
- TODAS as peças do Bloco 4 — usam Color Variables (não hardcode)
- `photography-signature` (3.7) — paleta da marca filtra color grading da fotografia
- `motion-design` (3.9) — overlays usam cores da marca

## Quality check (Contrato E)

- 2-3 primárias (não 1, não 5)?
- Cada cor com HEX + emoção + caso de uso?
- Harmonia nomeada explícita (1 das 4)?
- Acessibilidade WCAG verificada (AA mínimo)?
- Color Variables criadas no Figma com naming consistente?
- Regra 60-30-10 documentada?
- Foge da saturação do mercado (não bege/marrom em joalheria autoral, etc.)?

## Antipatterns

1. Mais de 3 cores primárias (vira "marca arco-íris", nenhuma cor é a marca)
2. Cor escolhida só por gosto, sem ancorar em moodboard / Big Idea
3. Pular acessibilidade — cliente com baixa visão não consegue ler
4. Hardcode de cor nas peças (não usar Variables) — aluno muda paleta depois e tem que refazer tudo
5. Ignorar saturação do mercado — paleta acabar virando "mais um da pilha"
6. Branco puro #FFFFFF como background — quase nunca é a melhor escolha (off-white tem mais alma)

## Frase-âncora

> **"Cor é o primeiro elemento que o público reconhece quando rola o feed — antes do logo, antes do texto, antes da imagem entrar em foco."**
