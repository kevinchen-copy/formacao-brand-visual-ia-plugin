---
name: formacao-brand-visual-ia-prompt-builder
description: Wizard que conduz o aluno a montar prompts profissionais de imagem em 6 camadas (Concept → Subject → Colors+Materials → Composition → Lighting → Camera+Lens) usando o Brand Guideline da marca ativa pra preencher Lighting Signature, Camera Signature e paleta automaticamente. Substitui o Custom GPT do ChatGPT (Kevin não usa ChatGPT) — wizard nativo no Claude Desktop. Inclui pre-prompt planning (3 perguntas antes de começar) + 8-year-old test no fim. Output é prompt em inglês pronto pra colar em Higgsfield, Nano Banana 2, Midjourney — com tradução pontual em PT-BR. Use quando o aluno disser - 'prompt builder', 'criar prompt', 'montar prompt', 'prompt em 6 camadas', 'prompt de imagem', 'preciso de prompt'. Bloco 4.2 do workflow Formação Branding Visual com IA — depois de storyboard, antes de image-generation.
---

# Prompt Builder — Bloco 4.2 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado à Aula 06 do Extra-Ofício (A Estrutura de 6 Camadas do Prompt) + Aula 07 (Custom GPT como Prompt Writer — agora SEM ChatGPT, é skill nativa no Claude).

## Propósito

Custom GPT do ChatGPT é o caminho ensinado no Mobile Editing Club original. Mas o Kevin **não usa ChatGPT** no stack-alvo. Esta skill **substitui o Custom GPT por wizard nativo no Claude Desktop** — mesmo método de 6 camadas, mas dentro do plugin que o aluno já tem.

## Conexão com o curso

- **Extra-Ofício Aula 03 (Como a IA Lê Prompts)** — keywords como gatilhos; ordem importa; vocabulário técnico
- **Extra-Ofício Aula 06 (Estrutura de 6 Camadas)** — Concept → Subject → Colors+Materials → Composition → Lighting → Camera+Lens
- **Extra-Ofício Aula 07 (Custom GPT como Prompt Writer)** — adaptada: Claude faz o papel do Custom GPT; sem migração pra ChatGPT
- **M05 (toda)** — vocabulário fotográfico técnico que cada camada usa
- **M02 Aula 03 (Framework dos 3 Eixos)** — vocabulário escrito alimenta direto o prompt

## Quando acionar

- "Prompt builder / criar prompt / montar prompt"
- "Prompt em 6 camadas / prompt de imagem"
- "Preciso de prompt"

## O que esta skill entrega

Prompt em inglês pronto pra colar em Higgsfield (Nano Banana) ou Midjourney, com:
- 6 camadas estruturadas
- Lighting Signature aplicada automaticamente (puxada de `bloco-3-7-photography-signature.md`)
- Camera Signature aplicada automaticamente
- Paleta da marca aplicada
- Brand Face cref (se peça tem pessoa)
- Tradução pontual `↳` em PT-BR de termos técnicos

Opcionalmente salva em `{vault}/marcas/{slug}/prompts/prompt-{nome-do-shot}.md`.

## Pré-requisitos

- `brand-guideline-companion.md` (CRÍTICO — Lighting/Camera Signatures + paleta + Brand Faces)
- Opcional: storyboard (se peça vem de storyboard, prompt herda contexto)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Opcional: storyboard atual

## Fluxo de execução (~10-15 min por prompt)

### Fase 1 — Pre-prompt planning (3 perguntas)
1. Qual o **conceito** dessa imagem? (hero shot de produto / brand face em ação / cenário sem pessoa / detalhe)
2. Em qual **gênero visual** dos 60 do M02 ela cai?
3. Pra qual **plataforma + formato** vai (1:1 IG / 9:16 Story / 16:9 YouTube)?

### Fase 2 — Camada 1: Concept
Define o gênero visual em 5-7 palavras (ex: "minimalist beauty hero shot, editorial composition").

### Fase 3 — Camada 2: Subject
Pra pessoa: aplica Brand Face cref + 6 dimensões do M05 Aula 03 (postura/pose/roupa/cabelo/expressão/joias/maquiagem) — SEM etnia explícita.
Pra produto: aplica 5 sub-dimensões físicas (tamanho/forma/textura/cor/condição) + posicionamento (M05 Aula 04).

### Fase 4 — Camada 3: Colors + Materials
Aplica paleta da marca (HEX em nome de cor — "Pedra Bruta deep brown #2C1F1A") + materiais (M05 Aulas 05-06 — comportamento da luz nas superfícies).

### Fase 5 — Camada 4: Composition
Posicionamento (regra dos terços / centralizado / off-center), 3 camadas de profundidade, espaço negativo, equilíbrio (M05 Aulas 07-09).

### Fase 6 — Camada 5: Lighting
Aplica AUTOMATICAMENTE a Lighting Signature da marca (`bloco-3-7-photography-signature.md`). Aluno só ajusta se quer variação pontual.

### Fase 7 — Camada 6: Camera + Lens
Aplica AUTOMATICAMENTE a Camera Signature da marca + film stock + abertura. Ajuste pontual se necessário.

### Fase 8 — Teste do "8 anos de idade" (M03 Aula 06 / Extra-Ofício)
Skill faz autoteste: se uma criança de 8 anos lê esse prompt em inglês, ela visualiza o que a marca quer? Se não, refina.

### Fase 9 — Tradução PT-BR pontual
Pra cada termo técnico fotográfico em inglês, adiciona `↳` com tradução breve. Aluno entende o que está escrito.

### Fase 10 — Output
Apresenta prompt final + marcação de qual ferramenta é melhor (Higgsfield / MJ / Nano Banana via Higgsfield).

## Padrão de comunicação (Contrato B)

PT-BR pra explicar; INGLÊS pra prompt final + tradução pontual `↳` PT-BR de termos técnicos.

## Decisões com o aluno (Contrato C)

- **Variação da Lighting/Camera Signatures:** aplica default, pergunta se quer ajustar pontualmente
- **Pessoa Sim/Não:** se sim, qual brand face usar (core / adjacente / diversidade)
- **Plataforma alvo:** define aspect ratio do prompt

## Output e integração downstream (Contrato D)

Consumido por:
- `image-generation` (4.3) — aluno cola prompt em Higgsfield ou MJ
- `catalog-coherence` (4.6) — herda 6 camadas pra gerar variações da coleção
- Opcionalmente salva em `{vault}/marcas/{slug}/prompts/`

## Quality check (Contrato E)

- 6 camadas preenchidas (não pulou nenhuma)?
- Lighting + Camera Signatures aplicadas (não esquecidas)?
- Subject sem etnia explícita (anti content restriction)?
- Passa teste do "8 anos"?
- Tradução `↳` PT-BR presente em termos técnicos?
- Sem menção a ChatGPT / Custom GPT (skill é nativa Claude)?

## Antipatterns

1. Mencionar Custom GPT ou ChatGPT — esta skill SUBSTITUI eles
2. Pular Lighting/Camera Signatures (perde coerência da marca)
3. Etnia explícita em Subject (gera content restriction recorrente)
4. Camadas em PT-BR (IA lê melhor em inglês — manter inglês)
5. Sem tradução pontual `↳` (aluno não-fluente em inglês fica perdido)
6. Prompt longo demais (>200 palavras vira ruído pra IA)

## Frase-âncora

> **"Prompt vago = imagem genérica. Prompt em 6 camadas = imagem on-brand replicável. Claude faz o papel do Custom GPT, sem precisar abrir ChatGPT."**
