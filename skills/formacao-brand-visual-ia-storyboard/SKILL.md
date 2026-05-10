---
name: formacao-brand-visual-ia-storyboard
description: Conduz o aluno a planejar peças de conteúdo (Reel/TikTok, carrossel, long form) com framework de 5 elementos obrigatórios (Hook, Setup, Middle, Resolution, CTA) + Triple Hook Strategy + 4 frameworks narrativos (Educational, Product Showcase, BTS, Transformation) + Visual Interest meta-framework em 6 elementos. Output é storyboard frame-by-frame pronto pra alimentar prompt-builder, image-generation, video-prompts e edicao. Use quando o aluno disser - 'storyboard', 'planejar Reel', 'planejar carrossel', 'estruturar conteúdo', 'roteiro visual', 'blueprint de peça', 'storyboard builder'. Bloco 4.1 do workflow Formação Branding Visual com IA — primeira skill da produção, vem depois do Brand Guideline fechado.
---

# Storyboard — Bloco 4.1 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às 11 aulas do M03 (Storytelling) — em especial Aula 02 (4 frameworks narrativos), Aula 03 (5 elementos panorâmica), Aulas 04-08 (cada elemento), Aula 09 (Visual Interest), Aula 10 (Storyboard — a costura prática), Aula 11 (Aplicação Integrada — Cabra Café).

## Propósito

20 minutos de storyboard economizam 4 horas de geração desperdiçada. Esta skill estrutura QUALQUER peça de conteúdo (Reel/TikTok/carrossel/long form) ANTES de qualquer geração de imagem/vídeo. Output frame-by-frame alimenta `prompt-builder`, `image-generation`, `video-prompts`, `edicao`.

## Conexão com o curso

- **M03 Aula 02 (4 Frameworks Narrativos)** — Educational / Product Showcase / Behind-the-Scenes / Transformation
- **M03 Aula 03 (5 Elementos Panorâmica)** — Hook → Setup → Middle → Resolution → CTA
- **M03 Aula 04 (Hook — Triple Hook Strategy)** — Visual + Texto/Sonoro + Subliminal sobrepostos
- **M03 Aula 09 (Visual Interest)** — 6 elementos (Ângulo, Textura, Profundidade, Movimento, Contraste, Inesperado); regra 60-70% movimento / 30-40% estático
- **M03 Aula 10 (Storyboard — Costura Prática)** — regra dos dois estágios (descrições textuais antes de imagens); processo em 6 passos; Framework Matrix (4x3); padrão de 10 quadros
- **M03 Aula 11 (Aplicação Integrada — Cabra Café)** — exemplo canônico: 4 storyboards completos pra mesma marca

## Quando acionar

- "Storyboard / planejar Reel / planejar carrossel"
- "Estruturar conteúdo / roteiro visual / blueprint de peça"

## O que esta skill entrega

`{vault}/marcas/{slug}/storyboards/storyboard-{nome-da-peca}.md` com:

- **Cabeçalho:** Objetivo + Takeaway + Público (avatar) + Plataforma + Duração + Aspect Ratio + Framework escolhido (1 dos 4)
- **5 elementos preenchidos:**
  - Hook (com Triple Hook Strategy: visual + verbal + subliminal)
  - Setup
  - Middle
  - Resolution
  - CTA
- **Storyboard frame-by-frame** (8-12 frames pra Reel curto / 6-10 pra carrossel / 15+ pra long form):
  - Pra cada frame: ângulo + tamanho de plano + movimento + texto overlay + duração (vídeo) ou texto principal (carrossel)
- **Visual Interest checklist** (M03 Aula 09 — 6 elementos verificados em cada frame)
- **Brief técnico downstream:**
  - Prompts de imagem necessários (alimenta `prompt-builder`)
  - Prompts de vídeo necessários (alimenta `video-prompts`)
  - Texto pra overlay (alimenta `edicao`)

## Pré-requisitos

- `brand-guideline-companion.md` (Voice & Tom + Photography/Videography Signatures + Motion Design)
- Definição da peça-âncora desejada (ou skill ajuda aluno a definir)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`

## Fluxo de execução (~30-60 min por peça)

### Fase 1 — Briefing da peça
- Objetivo: o que essa peça precisa CAUSAR (engajamento / conversão / construção de autoridade / lançamento)?
- Takeaway: o que a pessoa precisa LEMBRAR depois de assistir?
- Plataforma: Instagram Reel / Story / Feed / Carrossel / YouTube longo / Newsletter (cada um com gramática diferente)
- Duração / Aspect Ratio

### Fase 2 — Escolha do framework (M03 Aula 02)
Skill apresenta os 4 frameworks com matriz "qual usar quando":
- **Educational** — autoridade + valor; para tráfego N1-N2 ou educar mercado
- **Product Showcase** — quando produto é o protagonista; conversão direta
- **Behind-the-Scenes** — construção de marca; engajamento; transparência
- **Transformation** — mostra antes/depois; emocional; converte por identificação

Aluno escolhe.

### Fase 3 — Triple Hook Strategy (M03 Aula 04)
Pra cada peça, define 3 hooks sobrepostos nos primeiros 3 segundos:
- Hook visual (o que aparece em quadro)
- Hook verbal (frase falada ou texto overlay)
- Hook subliminal (quebra de padrão / informação visual incompleta / direção do olhar / tensão)

### Fase 4 — Preenchimento dos 5 elementos (M03 Aulas 04-08)
Skill conduz preenchimento de cada um aplicando a estrutura específica do framework escolhido (Educational tem estrutura diferente de Transformation).

### Fase 5 — Storyboard frame-by-frame (M03 Aula 10)
Frames numerados com:
- Ângulo (M05 Aula 10 — 8 ângulos)
- Tamanho de plano (M05 Aula 11 — 7 tamanhos)
- Movimento (M06 Aula 04 — 9 movimentos)
- Texto overlay (se houver, aplicando Voice & Tom + Tipografia + Motion da marca)
- Duração (vídeo) ou propósito do slide (carrossel)

### Fase 6 — Visual Interest checklist (M03 Aula 09)
Pra cada frame, verifica os 6 elementos: tem ângulo variado? Tem textura? Tem profundidade (3 camadas)? Tem movimento (se vídeo)? Tem contraste? Tem inesperado?

Regra: não repetir o mesmo ângulo por mais de 2-3 planos.

### Fase 7 — Brief técnico downstream
Skill destila:
- Lista de prompts de imagem necessários (cada um com Lighting + Camera Signatures aplicadas) → vai pra `prompt-builder`
- Lista de prompts de vídeo (image-to-video) → vai pra `video-prompts`
- Texto de cada overlay pra edição → vai pra `edicao`

## Padrão de comunicação (Contrato B)

PT-BR. Storyboard em formato tabela frame-by-frame. Cita aulas do M03 quando explica framework escolhido.

## Decisões com o aluno (Contrato C)

- **Framework:** apresenta 4 com prós/contras pra esse objetivo, aluno escolhe
- **Triple Hook:** propõe 3 candidatos, aluno escolhe combinação
- **Frames:** propõe estrutura, aluno aprova/refina

## Output e integração downstream (Contrato D)

CRÍTICO. Consumido por:
- `prompt-builder` (4.2) — escreve prompts de imagem pra cada frame
- `image-generation` (4.3) — gera as imagens
- `video-prompts` (4.4) — escreve JSON pra image-to-video se peça é vídeo
- `edicao` (4.7) — monta no CapCut com overlays + transições + pacing

## Quality check (Contrato E)

- Framework escolhido (1 dos 4)?
- Triple Hook em 3 camadas (visual + verbal + subliminal)?
- 5 elementos preenchidos (não pulou Middle por preguiça)?
- Storyboard tem 8-12 frames (não 3)?
- Visual Interest checklist passada em cada frame?
- Brief técnico downstream pronto pra alimentar próximas skills?

## Antipatterns

1. Pular storyboard e ir direto pra geração — gera 30 imagens erradas
2. Hook só visual (sem subliminal) — taxa de scroll cai
3. Middle "improvisado" — drop-off massivo
4. Frames com mesmo ângulo repetido — chato
5. Não passar Visual Interest checklist — peça fica medíocre
6. Storyboard sem brief técnico — `prompt-builder` recebe input vago

## Frase-âncora

> **"20 minutos de storyboard economizam 4 horas de geração desperdiçada."**
