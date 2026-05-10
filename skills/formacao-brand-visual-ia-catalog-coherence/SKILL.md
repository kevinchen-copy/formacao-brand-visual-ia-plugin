---
name: formacao-brand-visual-ia-catalog-coherence
description: Garante consistência visual entre múltiplos produtos de uma mesma coleção/marca — quando o aluno tem 12 hero shots de produtos diferentes, garante que pareçam UMA família de marca em vez de 12 marcas diferentes. Usa 1 hero shot já aprovado como âncora e deriva prompts pros produtos restantes herdando lighting setup, ângulo, paleta de fundo, brand face, direção de sombras, color grading. Apenas o produto muda — todo o resto é replicado. Output são prompts derivados pra cada produto + checklist de coerência. Use quando o aluno disser - 'catálogo congruente', 'consistência multi-produto', 'gerar coleção inteira', 'fotos da família de produtos', 'catalog coherence', 'hero shots da coleção'. Bloco 4.6 do workflow Formação Branding Visual com IA — depois de video-prompts, antes de edicao.
---

# Catalog Coherence — Bloco 4.6 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado à Aula 09 do Extra-Ofício (Imagens de Produto — 5 métodos canônicos) + Aula 12 (9 Hacks Nano Banana) + M02 Aula 02 (Sistema dos 15 Elementos — consistência redundante).

## Propósito

Marca de e-commerce com 12 produtos numa coleção precisa que os 12 hero shots **pareçam UMA família de marca**, não 12 marcas diferentes. Esta skill usa 1 hero shot já aprovado como **âncora** e deriva prompts pros produtos restantes herdando TUDO menos o produto (lighting, ângulo, paleta de fundo, brand face presente, color grading, direção de sombras).

## Conexão com o curso

- **Extra-Ofício Aula 09 (Imagens de Produto)** — Hero Object Placeholder + Product Swap como métodos pra coerência
- **Extra-Ofício Aula 12 (9 Hacks Nano Banana)** — Hack 3 (Product Swap) + Hack 7 (Scene Swap) — base técnica
- **M02 Aula 02 (Sistema dos 15 Elementos)** — "consistência redundante > excelência isolada"

## Quando acionar

- "Catálogo congruente / consistência multi-produto"
- "Gerar coleção inteira / fotos da família de produtos"
- "Catalog coherence / hero shots da coleção"

## O que esta skill entrega

`{vault}/marcas/{slug}/imagens/colecao-{nome}/prompts.md` com:
- **Prompt-âncora** documentado (qual hero shot original, URL/seed, prompt em 6 camadas)
- **Lista de produtos restantes** (10-50 itens) com:
  - Nome do produto
  - Descrição física (5-7 linhas — só o que muda)
  - Prompt derivado (herdando 90% do âncora, mudando só o produto)
  - Método recomendado (Product Swap via Nano Banana / Omni Reference no MJ / Hero Object Placeholder)
- **Checklist de coerência** em 5 pontos pra validar cada imagem gerada

## Pré-requisitos

- `brand-guideline-companion.md`
- 1 hero shot já gerado e APROVADO via `image-generation` (URL + seed + prompt original em 6 camadas)
- Lista dos N produtos restantes da coleção

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Hero shot âncora (URL + seed + prompt)
4. Lista de produtos da coleção

## Fluxo de execução (~30-60 min pra coleção de 12 produtos)

### Fase 1 — Confirmar prompt-âncora
Aluno aponta qual hero shot já aprovado vai virar âncora. Skill puxa o prompt em 6 camadas + URL + seed.

### Fase 2 — Identificar elementos a HERDAR (90% do prompt)
Tudo herda do âncora EXCETO o produto:
- Lighting Signature (mantém)
- Camera Signature (mantém)
- Composition (mantém)
- Color/grading (mantém)
- Background/cenário (mantém)
- Brand face (se houver — mantém com cref)
- Direção de sombras (mantém)
- Atmosfera (mantém)

### Fase 3 — Identificar o que MUDA (10% do prompt)
Apenas:
- Subject = novo produto
- Posicionamento físico do produto (se diferente)
- Talvez ajuste micro de luz pra revelar característica do novo produto

### Fase 4 — Escolha do método de geração
Pra cada produto, recomenda:
- **Product Swap (Nano Banana via Higgsfield)** — DEFAULT pra produtos similares ao âncora
- **Omni Reference (MJ)** — quando produto novo é radicalmente diferente em forma
- **Hero Object Placeholder + Product Swap** — pra produtos com geometria complexa

### Fase 5 — Gerar 1 produto por vez (não em batch)
Geração 1 por vez detecta drift cedo. Se 3º produto começa a divergir do âncora, aluno corrige antes de gerar os 9 restantes.

### Fase 6 — Cross-reference
Adicionar ao prompt: "consistent with reference image [URL do âncora]" pra reforçar coerência.

### Fase 7 — Checklist de coerência (5 pontos)
Pra cada imagem gerada, valida:
1. Lighting bate com âncora (mesma direção, intensidade, cor)?
2. Background bate (mesmo cenário, mesma profundidade)?
3. Color grading idêntico?
4. Direção de sombras consistente?
5. Brand face (se aplica) é o mesmo rosto?

Se 1 ou mais falham → regenera com instrução específica de correção.

### Fase 8 — Salvar coleção completa
URLs + seeds em `prompts.md`; imagens vão pra `imagens/colecao-{nome}/`.

## Padrão de comunicação (Contrato B)

PT-BR. Sempre mostra checklist de coerência antes de aprovar cada imagem. Se algo divergir, aponta especificamente o que (não "tá estranho" — "iluminação no produto 3 vem da direita, no âncora vem da esquerda").

## Decisões com o aluno (Contrato C)

- **Hero shot âncora:** aluno escolhe qual dos hero shots aprovados serve de referência
- **Método por produto:** propõe baseado em complexidade, aluno aprova
- **Aprovação por produto:** valida cada imagem com checklist antes de seguir

## Output e integração downstream (Contrato D)

Consumido por:
- `figma` (3.11) — handoff pra montar grid do catálogo
- `static-ads-ecommerce` (4.5) — usa imagens da coleção em ads
- `platform-adaptation` (4.8) — adapta coleção pros canais

## Quality check (Contrato E)

- 90% do prompt herdado do âncora?
- Geração 1 por vez (não em batch)?
- Cross-reference incluído nos prompts derivados?
- Checklist de coerência aplicado em CADA imagem?
- 5/5 pontos passam ou imagem é regenerada?

## Antipatterns

1. Gerar coleção inteira em batch sem ver — drift acumula sem detectar
2. Pular cross-reference (sem URL do âncora no prompt) — coerência se perde
3. Variar lighting/grading "pra ficar mais variado" — destrói família visual
4. Aprovar imagem com 3/5 do checklist — coleção fica desconjunta
5. Não salvar seed do âncora — impossível reproduzir/iterar

## Frase-âncora

> **"12 hero shots de uma marca precisam parecer UMA família. Apenas o produto muda — todo o resto é replicado."**
