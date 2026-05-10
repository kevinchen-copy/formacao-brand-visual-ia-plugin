---
name: formacao-brand-visual-ia-logo-system
description: Conduz o aluno a construir o sistema de logo da marca como Components vivos no Figma — não apenas 1 logo, mas um SISTEMA com primário + variações (horizontal, vertical, monograma, invertido, monocromático) + clear space + tamanhos mínimos + contextos aprovados + usos proibidos. Cria Components reutilizáveis na Página Brand Guideline do Figma Studio. Use quando o aluno disser - 'logo', 'sistema de logo', 'logotipo', 'monograma', 'variações de logo', 'clear space', 'usos do logo', 'logo novo', 'redesenhar logo'. Bloco 3.2 do workflow Formação Branding Visual com IA — depois do moodboard, antes da tipografia.
---

# Logo System — Bloco 3.2 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às Aulas 04 do M02 (Logo System: Não é Logo, é Sistema) + Aula 06 do M04 (Pilar Formas).

## Propósito

Marca pequena entrega "1 logo" e improvisa em todos os contextos. Marca profissional entrega **sistema** com 5 variações + regras de uso, vivos como Components no Figma — qualquer peça do Bloco 4 puxa o Component certo via instância.

## Conexão com o curso

- **M02 Aula 04 (Logo System)** — 5 versões obrigatórias; clear space; tamanhos mínimos; teste dos 24px; regra polêmica "Reels sem logo estático"; reconhecimento vem dos 14 outros elementos
- **M04 Aula 06 (Pilar Formas)** — geometria do logo (círculo / quadrado / triângulo / linhas) carrega psicologia visual

## Quando acionar

- "Logo / sistema de logo / logotipo / monograma"
- "Variações de logo / clear space / usos do logo"
- "Logo novo / redesenhar logo"

## O que esta skill entrega

**Components no Figma** (Página 2 — Brand Guideline):
- 5 Components Master:
  1. Logo Primário (versão principal)
  2. Logo Horizontal (lockup horizontal)
  3. Logo Vertical (lockup vertical)
  4. Monograma (símbolo isolado, sem nome)
  5. Logo Invertido (pra fundo escuro)
- Cada Component com Auto Layout + clear space marcado em frames de demonstração
- Tabela visual de tamanhos mínimos (16px, 24px, 48px, 96px)
- Grid de "usos proibidos" (5-6 antipatterns mostrando o que NÃO fazer)

**Localmente:**
- `{vault}/marcas/{slug}/bloco-3-2-logo-system.md` com:
  - Princípios de construção do logo (ancorados no moodboard)
  - 5 variações documentadas com referência ao Figma
  - Clear space (em múltiplos da altura X)
  - Tamanhos mínimos por contexto
  - 5-6 usos proibidos com razão
- Pasta `{vault}/marcas/{slug}/logos/` com SVG/PNG/PDF dos 5 logos exportados

## Pré-requisitos

- `bloco-2-1-big-idea.md` + `bloco-2-2-positioning.md`
- `bloco-3-1-moodboard.md` (princípios visuais da marca já travados)
- `figma-file-key.txt`

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. Big Idea + Positioning + Moodboard
3. `figma-file-key.txt`

## Fluxo de execução (~60-90 min)

### Fase 1 — Diagnóstico de logo atual (se existir)
Aluno tem logo? Aplica Teste do Squint (M01 Aula 01 — aperta os olhos): logo passa em legibilidade reduzida? Funciona em 24px? Funciona invertido? Se passa nos 3, refina; se falha, redesenha.

### Fase 2 — Decisão estrutural (4 tipos de logo)
- Logotipo (só tipografia, sem ícone) — ex: Google, Coca-Cola
- Símbolo/Monograma — ex: Apple, Nike (já consagrados)
- Combinado — ex: Adidas, Lacoste (mais comum em marca em construção)
- Lockup — arranjo fixo de elementos

Skill ajuda aluno a escolher tipo baseado em moodboard + Big Idea.

### Fase 3 — Construção das 5 variações
Skill orienta a construção (ou refinamento) das 5 variações no Figma. Se aluno é designer, ele desenha; se não, skill recomenda contratar designer especializado pra essa fase específica + retomar com o sistema pronto.

### Fase 4 — Clear space + tamanhos mínimos
Define clear space em múltiplos da altura X (geralmente 0.5x ou 1x). Tamanhos mínimos: 16px (favicon), 24px (mobile UI), 48px (cards), 96px (post hero), 200px (vitrine).

### Fase 5 — Criar Components no Figma
Via MCP, criar 5 Components Master na Página Brand Guideline com Auto Layout + frames de clear space + grid de tamanhos.

### Fase 6 — Usos proibidos (5-6 antipatterns)
Grid visual mostrando: distorcer / mudar cor sem motivo / encaixar em forma alheia / esticar / sobrepor com texto / aplicar efeito 3D — com X vermelho em cada.

### Fase 7 — Exportar SVG/PNG/PDF
Via MCP, exportar as 5 variações em SVG (escala) + PNG (web) + PDF (impressão) pra `{vault}/marcas/{slug}/logos/`.

## Padrão de comunicação (Contrato B)

PT-BR. Quando o aluno é designer: linguagem técnica (Auto Layout, clear space, monograma). Quando não é: explica termos antes de usar.

## Decisões com o aluno (Contrato C)

- **Tipo estrutural (4 opções):** aluno escolhe baseado em proposta da skill
- **Designer externo:** se aluno não desenha, skill SUGERE buscar designer especializado pra essa fase (não tenta desenhar pelo aluno via IA — logos via IA têm problemas conhecidos)
- **5 usos proibidos:** aluno aprova lista (alguns podem não se aplicar à marca dele)

## Output e integração downstream (Contrato D)

Consumido por:
- `brand-guideline-builder` (3.10) — Seção 6 (Sistema de Logo)
- `static-ads-ecommerce` (4.5) e `carrossel-estatico` (4.5) — usam Component instance do logo
- `platform-adaptation` (4.8) — adapta logo por plataforma
- TODAS as peças do Bloco 4 — instância do Component

## Quality check (Contrato E)

- 5 variações criadas como Components (não cópias de imagens)?
- Auto Layout aplicado em cada Component?
- Clear space marcado em frame de demonstração?
- Tamanhos mínimos validados (24px ainda legível)?
- 5-6 usos proibidos documentados visualmente?
- SVGs exportados (não só PNG)?

## Antipatterns

1. Tentar gerar logo via Midjourney/Higgsfield — IAs têm problemas com tipografia precisa em logo
2. 1 logo só, sem variações (quebra em contextos invertidos / pequenos / mono)
3. Pular clear space (aluno cola tudo encostado em vitrine real)
4. Esquecer monograma (versão pequena / favicon precisa de algo legível)
5. Component sem Auto Layout — fica difícil de redimensionar consistentemente

## Frase-âncora

> **"Logo não é 1 imagem. É um sistema de variações que protege a marca em todos os contextos. Quem define só 1 logo, perde controle em 30 dias."**
