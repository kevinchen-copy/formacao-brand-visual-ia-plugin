---
name: formacao-brand-visual-ia-moodboard
description: Conduz o aluno a montar a coleção de referências visuais (moodboard) DENTRO da Página Moodboard do Figma já criado pelo figma-setup. Não é pasta MD nem Pinterest — é frames vivos no estúdio Figma da marca. Cobre 3 fontes (referências culturais, Pinterest curado, fotos da própria loja/cliente) e ensina a extrair de cada referência O QUE especificamente serve a marca - uma palavra, uma cor, um gestual, uma luz. Output são 12-16 imagens com legenda 'extract pra esta marca' em cada, organizadas como frames vivos no Figma. Use quando o aluno disser - 'moodboard', 'coleção de referências', 'inspirações visuais', 'referências culturais', 'pinterest da marca', 'fotos da minha loja', 'referências'. Bloco 3.1 do workflow Formação Branding Visual com IA — depois de figma-setup, antes de logo-system.
---

# Moodboard — Bloco 3.1 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às Aulas 1-3 do M02 (Identidade Visual + Sistema dos 15 Elementos + Framework dos 3 Eixos) + Aula 13 do M01 (Provas — narrativa visual).

## Propósito

ANTES de qualquer decisão de paleta, tipografia, lighting ou camera, o aluno precisa **coletar referências visuais e extrair delas**. Esta skill conduz a montagem do moodboard DENTRO da Página Moodboard do Figma (criada pelo figma-setup) — não como pasta de MDs.

Cada referência vem com legenda explicitando O QUE servir pra esta marca específica (uma palavra, uma cor, um gestual, uma luz, uma textura).

## Conexão com o curso

- **M02 Aula 01 (O Que é Identidade Visual)** — referência cultural educa o olho
- **M02 Aula 03 (Framework dos 3 Eixos)** — moodboard alimenta posicionamento nos 3 eixos
- **M02 Aula 11 (Brand Guidelines)** — moodboard é parte do brand book final

## Quando acionar

- "Moodboard / coleção de referências"
- "Inspirações visuais / referências culturais"
- "Pinterest da marca / fotos da minha loja"

## O que esta skill entrega

**Na Página Moodboard do Figma:**
- 12-16 frames com imagens de referência organizadas em grade
- Legenda em cada frame: o que extrair PRA ESTA MARCA (não só "isso é bonito")
- 3-5 âncoras culturais nomeadas (ex: "estética sul-italiana 1960", "fotografia de Sebastião Salgado", "interior de ateliê")

**Localmente:**
- `{vault}/marcas/{slug}/bloco-3-1-moodboard.md` com:
  - Lista das 12-16 referências (autor + URL/origem + extract pra marca)
  - 3-5 âncoras culturais nomeadas
  - Tese visual em 1 parágrafo (qual o "DNA visual" emergente)

## Pré-requisitos

- `bloco-2-1-big-idea.md` + `bloco-2-2-positioning.md` + `bloco-2-3-ideal-client.md` + `bloco-2-4-tribe-enemy.md` (CRÍTICO — moodboard responde à tese)
- `figma-file-key.txt` (skill `figma-setup` já rodou)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. 4 docs do Bloco 2
3. `figma-file-key.txt`

## Fluxo de execução (~60-90 min — exige curadoria do aluno)

### Fase 1 — As 3 fontes obrigatórias
Skill explica e o aluno coleta de 3 fontes (cada uma 4-6 referências):

1. **Referências culturais** (cinema, fashion editorial, arquitetura, música, pintura, fotografia documental)
2. **Pinterest curado** — busca específica baseada na Big Idea, NÃO o "salvar tudo"
3. **Fotos da própria loja / cliente / processo** (refs reais, não aspiração)

### Fase 2 — Extract pra esta marca (técnica anti-Pinterest)
Pra cada referência, aluno responde a pergunta-filtro: *"O que ESPECIFICAMENTE desta imagem serve à minha marca?"* — 1 palavra, 1 cor, 1 textura, 1 gestual, 1 luz. Sem isso, vira biblioteca de Pinterest sem direção.

### Fase 3 — Upload pro Figma
Skill orienta como fazer upload das imagens pra Página Moodboard via interface Figma OU via MCP `upload_assets`. 12-16 frames organizados em grade 4×4 ou similar.

### Fase 4 — Legenda em cada frame
Cada frame ganha texto com a legenda "Extract: [palavra/cor/textura específica]" usando Text Style já criado.

### Fase 5 — Âncoras culturais (3-5 nomeadas)
Skill ajuda a destilar o moodboard em 3-5 âncoras culturais nomeadas — referências macro que organizam o todo. Exemplo: "Pôster de cinema italiano dos 60", "Editorial Vogue Paris recente", "Fotografia de Steve McCurry".

### Fase 6 — Tese visual em 1 parágrafo
Aluno escreve 1 parágrafo respondendo: "Olhando esse moodboard inteiro, qual a tese visual que emerge pra minha marca?" — 4-6 linhas máx.

### Fase 7 — Salvar localmente
`bloco-3-1-moodboard.md` com lista das 12-16 refs + extracts + âncoras + tese.

## Padrão de comunicação (Contrato B)

PT-BR. Insistir na pergunta-filtro "Extract pra esta marca" — moodboard sem extract vira decoração inutilizável.

## Decisões com o aluno (Contrato C)

- **Quais 12-16 referências:** aluno escolhe (skill não decide gosto)
- **Âncoras culturais:** aluno nomeia (skill propõe categorização se ele se perder)
- **Tese visual:** aluno escreve, skill revisa por coerência

## Output e integração downstream (Contrato D)

Consumido por TODAS as skills visuais do Bloco 3:
- `logo-system` (3.2)
- `typography` (3.3)
- `color-palette` (3.4)
- `brand-faces` (3.5)
- `photography-signature` (3.7)
- `videography-signature` (3.8)
- `motion-design` (3.9)
- `brand-guideline-builder` (3.10) — Seção 11 (Moodboard)

## Quality check (Contrato E)

- 12-16 referências (não 5, não 50)?
- Cada uma tem extract específico (não "é legal")?
- 3 fontes diferentes representadas (não só Pinterest)?
- 3-5 âncoras culturais nomeadas?
- Tese visual em 1 parágrafo, não 5?

## Antipatterns

1. Aluno colar 50 imagens — vira poluição, não direção
2. Extract genérico ("é bonito", "tem mood") — não filtra nada
3. Referência só de Pinterest — perde camada cultural mais profunda
4. Pular fotos da própria realidade do aluno — moodboard 100% aspiracional descola da entrega real
5. Não criar âncoras culturais nomeadas — moodboard fica solto sem coluna vertebral

## Frase-âncora

> **"Buscar referência não é vergonha. Pular etapa é. Um bom moodboard mostra que você sabe o que NÃO copiar — porque sabe o que extrair."**
