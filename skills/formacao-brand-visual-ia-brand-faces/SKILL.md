---
name: formacao-brand-visual-ia-brand-faces
description: Conduz o aluno a definir as Brand Faces da marca (rostos humanos visíveis no conteúdo) escolhendo entre 4 caminhos - A) fundadora ou pessoa real é o rosto, B) 1-3 brand faces criadas via IA, C) múltiplas brand faces por contexto, D) sem rosto humano (só produto e cenários). Para caminhos com IA, conduz descrição detalhada em 10 dimensões (idade, traços físicos sem etnia explícita pra evitar content restriction, cabelo, olhos, pele, expressão default, estilo de roupa, postura, gestual, contexto) + URL imagem master pra usar como cref. Estrutura 3 brand faces (core/adjacente/diversidade) baseada em ideal-client. Inclui regras de uso (quando aparece, quando não, como olha pra câmera). Use quando o aluno disser - 'brand faces', 'rosto da marca', 'modelo da marca', 'avatar IA', 'character consistency', 'fundadora aparece', 'sem rosto humano'. Bloco 3.5 do workflow Formação Branding Visual com IA — depois de paleta, antes de voice-tone.
---

# Brand Faces — Bloco 3.5 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado à Aula 07 do M02 (Brand Faces: Os Rostos da Marca) + Aula 12 (Aplicação Integrada com Marina/Ricardo/Dona Cleusa) + Aula 10 do Extra-Ofício (Gerando Imagens de Modelo).

## Propósito

Logo dá reconhecimento. **Rosto humano dá conexão.** Esta skill define quem aparece como rosto da marca e como manter consistência absoluta entre múltiplas peças (caso B/C/D — via IA — exige `--cref` no Midjourney + cref equivalente em Higgsfield).

## Conexão com o curso

- **M02 Aula 07 (Brand Faces)** — "people buy from people"; Caminho A (founder-led) × Caminho B (modelos/IA); regra "decida por estratégia, não por medo de câmera"; armadilha demográfica (rosto principal bate com core, entorno mostra diversidade); 3 brand faces (core/adjacente/diversidade); 10 dimensões de documentação por rosto
- **M02 Aula 12 (Aplicação Integrada — Ferra)** — exemplo canônico: Marina (core 42a) + Ricardo (adjacente 38a) + Dona Cleusa (artesã 65a)
- **Extra-Ofício Aula 10 (Gerando Imagens de Modelo)** — close-up primeiro, reutilizar via Nano Banana mantendo cref

## Quando acionar

- "Brand faces / rosto da marca / modelo da marca"
- "Avatar IA / character consistency"
- "Fundadora aparece / sem rosto humano"

## O que esta skill entrega

**Localmente:**
- `{vault}/marcas/{slug}/bloco-3-5-brand-faces.md` com:
  - Caminho escolhido (A / B / C / D) + razão
  - Pra cada brand face (1-3): 10 dimensões documentadas
  - URL da imagem master de cada (pra usar como cref)
  - Regras de uso (quando aparece, em que contexto, como olha pra câmera, quando NÃO aparece)
  - Armadilha demográfica resolvida (core + adjacente + diversidade)

**No Figma** (Página Brand Guideline):
- Board com 3 imagens master + descrição em 10 dimensões + regras de uso

## Os 4 caminhos (M02 Aula 07)

- **Caminho A — Fundadora ou pessoa real é o rosto** (founder-led)
  - Vantagem: autenticidade máxima, conexão humana imediata
  - Custo: limita escala (uma pessoa só), exige que a fundadora apareça
  
- **Caminho B — 1 brand face criada via IA**
  - Vantagem: consistência total, controle estético
  - Custo: requer descrição rigorosa + cref disciplinado

- **Caminho C — 3 brand faces (core + adjacente + diversidade) via IA**
  - Vantagem: cobre armadilha demográfica + 3 contextos
  - Recomendado pra marcas B2C que precisam mostrar variedade
  - Exemplo: Ferra do M02 — Marina/Ricardo/Dona Cleusa

- **Caminho D — Sem rosto humano (só produto + cenários)**
  - Vantagem: foco absoluto no produto
  - Custo: perde camada de conexão emocional humana
  - Funciona em: marcas tech B2B, marcas premium minimalistas (Aesop), produtos abstratos

## As 10 dimensões por brand face (M02 Aula 07)

Pra cada brand face em caminhos B/C, documentar:

1. **Idade** (faixa: 28-32 / 38-44 / 60-68)
2. **Traços físicos** (sem etnia explícita pra evitar content restriction — usar "luminous skin", "warm undertone", "natural features")
3. **Cabelo** (comprimento, cor, textura, estilo dominante)
4. **Olhos** (cor, formato)
5. **Pele** (textura, vellus hair, subsurface scattering pra evitar plastificação)
6. **Expressão default** (contemplativa / amigável / focada / serena)
7. **Estilo de roupa** (paleta + materiais + 3 peças canônicas)
8. **Postura** (relaxada / ereta / em movimento)
9. **Gestual** (mãos visíveis, gesto característico)
10. **Contexto** (onde geralmente aparece — interior / exterior / atelier / casa)

## Pré-requisitos

- `bloco-2-3-ideal-client.md` (CRÍTICO — brand face responde ao F1)
- `bloco-3-1-moodboard.md` (estética visual da marca)
- `bloco-3-4-color-palette.md` (paleta filtra escolha de roupa/contexto)
- `figma-file-key.txt`

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. Ideal Client + Moodboard + Color Palette
3. `figma-file-key.txt`

## Fluxo de execução (~60-90 min)

### Fase 1 — Decisão do caminho (A / B / C / D)
Skill apresenta os 4 caminhos com prós/contras + recomendação baseada em ideal-client. Aluno decide.

### Fase 2 — Documentação em 10 dimensões (caminhos B/C)
Pra cada brand face (1-3), aluno preenche as 10 dimensões com auxílio da skill. Skill ALERTA sobre etnia explícita (gera content restriction em MJ/Higgsfield).

### Fase 3 — Geração da imagem master (caminhos B/C)
Skill gera prompt em 6 camadas (estrutura usada por `prompt-builder` no Bloco 4) pra criar close-up de cada brand face. Aluno gera no MJ ou Higgsfield, escolhe a melhor, salva URL.

### Fase 4 — Validação de consistência
Aluno gera 2-3 variações da mesma brand face (ângulos diferentes, contextos diferentes) usando `--cref` (MJ) ou cref equivalente (Higgsfield). Skill valida que rosto se mantém reconhecível.

### Fase 5 — Regras de uso
Define: quando cada brand face aparece (Marina em peças core, Dona Cleusa em peças de origem, Ricardo em peças de público adjacente)? Como olha pra câmera (direto / lateral / nunca)? Em que estado emocional?

### Fase 6 — Salvar localmente + no Figma
MD com tudo documentado + board no Figma com 3 imagens master + 10 dimensões + regras.

## Padrão de comunicação (Contrato B)

PT-BR. CRÍTICO: ao escrever descrições pra MJ/Higgsfield, usar inglês + evitar etnia explícita (gera content restriction). Substituir por descrição neutra: "luminous skin with warm undertone", "natural facial features", etc.

## Decisões com o aluno (Contrato C)

- **Caminho A vs B vs C vs D:** decisão estratégica do aluno (skill ajuda a pesar)
- **Quem é a brand face core (caminho A):** fundadora? Equipe? Modelo profissional?
- **Quantas brand faces (caminho C):** 1, 2 ou 3?
- **Imagem master final:** aluno aprova após gerar 5-10 variações

## Output e integração downstream (Contrato D)

Consumido por:
- `brand-guideline-builder` (3.10) — Seção 9 (Brand Faces)
- `prompt-builder` (4.2) — auto-aplica brand face cref em prompts de pessoa
- `image-generation` (4.3) — usa cref pra manter consistência
- `video-prompts` (4.4) — JSON inclui character reference
- `static-ads-ecommerce` (4.5) e `ad-video-creator` (4.5) — peças com pessoa usam brand face certa por contexto

## Quality check (Contrato E)

- Caminho documentado (A/B/C/D) com razão?
- Pra B/C: 10 dimensões preenchidas por brand face?
- URL master salva pra cada brand face?
- Etnia EVITADA em descrições (anti content restriction)?
- Regras de uso documentadas (quando aparece, como olha)?
- Armadilha demográfica resolvida (caminho C)?

## Antipatterns

1. Etnia explícita na descrição ("African woman" / "Asian man") — gera content restriction recorrente
2. 1 brand face única em marca B2C grande — cliente não se reconhece
3. Brand face genérica (sem 10 dimensões) — fica diferente em cada geração
4. Não salvar URL master — impossível manter consistência depois
5. Pular regras de uso — peças misturam brand faces em contextos errados
6. Skill tentar GERAR a imagem por conta própria — aluno gera no MJ/Higgsfield e aprova

## Frase-âncora

> **"Logo constrói reconhecimento. Rosto humano constrói conexão. As duas coisas são diferentes, e marca forte tem as duas."**
