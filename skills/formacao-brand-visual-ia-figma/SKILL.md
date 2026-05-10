---
name: formacao-brand-visual-ia-figma
description: Modo OPERAÇÃO do estúdio Figma da marca — opera o dia a dia de produção visual no arquivo já criado pelo figma-setup. Atende pedidos recorrentes - duplicar template, montar peça com imagem gerada e copy, criar template novo sob demanda, exportar finais, atualizar Production Log. Usa o Figma MCP conectado pra executar direto, sem o aluno abrir o Figma manualmente. Use quando o aluno disser - 'figma', 'editar no figma', 'montar peça no figma', 'exportar do figma', 'aplicar no figma', 'duplicar template', 'criar template novo'. Bloco 3.11 do workflow Formação Branding Visual com IA — depois de brand-guideline-builder. Skill chamada repetidamente ao longo do Bloco 4.
---

# Figma — Bloco 3.11 do Workflow (Modo OPERAÇÃO)

> **Cumpre Contrato Comum das Skills v2.0** — Esta é a skill de **Modo Operação** do Figma Studio. Skill complementar a `figma-setup` (Modo Setup). Distingue claramente: setup cria 1 vez; operação roda toda vez que aluno quer mexer no Figma.

## Propósito

Estúdio Figma já existe (criado pelo `figma-setup` no Bloco 3.0). Brand Guideline já está consolidado nele (pelo `brand-guideline-builder` 3.10). Esta skill **opera** o estúdio no dia a dia: duplicar template, montar peça nova, exportar, atualizar log. Roda VIA MCP — aluno não precisa abrir o Figma manualmente pra ações repetitivas.

## Conexão com o curso

- **M02 Aulas 04-11 (Sistema completo de identidade visual)** — Figma é o ambiente onde a identidade vive
- **Extra-Ofício Aula 16 (Aplicação Integrada — Ferra)** — Figma como destino final das peças produzidas com IA

## Quando acionar

- "Figma / editar no figma / montar peça no figma"
- "Exportar do figma / aplicar no figma"
- "Duplicar template / criar template novo"

## O que esta skill entrega

Operações sob demanda no estúdio Figma:

- **Duplicar template** (ex: "duplica template Story pra fazer um Story de lançamento Anel Lourdes 03")
- **Montar peça** com imagem gerada + copy + tipografia + cor (puxa Color Variables + Text Styles do estúdio)
- **Criar template novo** sob demanda (ex: aluno percebe que precisa de "template de e-book de 12 páginas" — skill cria + adiciona à Página correspondente)
- **Atualizar Component** (ex: "atualiza Logo Primário com refinamento que fiz no Illustrator")
- **Exportar peças finais** em PNG/JPG/PDF/MP4 pra `{vault}/marcas/{slug}/exports/{data}/`
- **Atualizar Production Log** (Página 11) com lista do que foi produzido

## Pré-requisitos

- `figma-file-key.txt` (skill `figma-setup` já rodou)
- `brand-guideline-companion.md` (skill `brand-guideline-builder` já rodou)
- MCP Figma autenticado

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `figma-file-key.txt` (file key do Brand Studio da marca)
3. `brand-guideline-companion.md` (pra saber Variables, Text Styles, Components disponíveis)

## Fluxo de execução (varia por pedido — 5-30 min cada)

### Pedidos comuns

**A) Duplicar template + customizar:**
1. Identifica template solicitado (Story / Carrossel / Feed / Reel Cover / Ad Estático / etc.)
2. Duplica via `use_figma` (figma.createCopy ou clone)
3. Customiza com copy + imagem fornecida
4. Aplica Color Variables + Text Styles (não hardcode)
5. Posiciona na página correta
6. Atualiza Production Log

**B) Montar peça nova com imagem gerada (handoff de outras skills):**
1. Recebe imagem (URL gerada via image-generation) + copy aprovada
2. Cria frame no template apropriado
3. Insere imagem como fill do frame ou como elemento posicionado
4. Adiciona copy usando Text Styles
5. Aplica logo via Component instance
6. Exporta versão final em PNG/JPG
7. Atualiza Log

**C) Criar template novo sob demanda:**
1. Pergunta dimensões + propósito + onde adicionar
2. Cria frame com tamanho exato
3. Aplica grid + safe zones se aplicável
4. Adiciona placeholders (texto + imagem)
5. Salva em página correspondente OU cria nova página
6. Atualiza `figma-pages-inventory.md`

**D) Exportar peças finais:**
1. Recebe lista de frames/IDs a exportar
2. Define formato (PNG / JPG / PDF / MP4 — vídeo precisa de export externo)
3. Exporta via MCP em batch
4. Salva em `{vault}/marcas/{slug}/exports/{data}/`
5. Retorna paths

**E) Atualizar Production Log (Página 11):**
- Adiciona linha com data + nome da peça + tipo + ID do frame + URL de export

## Padrão de comunicação (Contrato B)

PT-BR. Quando rodar operação Figma, mostra alto nível ("duplicando template Story... aplicando Color Variable Pedra Bruta no fundo... posicionando Logo via Component instance..."). Não dump JSON.

## Decisões com o aluno (Contrato C)

- **Confirmação antes de operações irreversíveis** (deletar / sobrescrever Component)
- **Tamanho de template novo:** propõe baseado em plataforma, aluno aprova
- **Aprovação visual antes de export final:** mostra screenshot, aluno aprova

## Output e integração downstream (Contrato D)

Skill ROTACIONAL — chamada repetidamente. Outputs ficam no Figma + na pasta `exports/`.

Consumida por:
- `static-ads-ecommerce` (4.5) — handoff de copy + imagem pra montar ad no template
- `carrossel-estatico` (4.5) — handoff de 8 slides
- `ad-video-creator` (4.5) — handoff de storyboard pad
- `platform-adaptation` (4.8) — adapta peça-âncora pros 4 templates de plataforma

## Quality check (Contrato E)

- Variables + Text Styles aplicados (não hardcode de cor/fonte)?
- Logo aplicado como Component instance (não imagem cortada)?
- Safe zones respeitadas em peças 9:16 e 16:9?
- Production Log atualizado?
- Export salvo em pasta correta com nome consistente?

## Antipatterns

1. Hardcode de cor (#2C1F1A) em vez de aplicar Variable — aluno muda paleta depois e quebra tudo
2. Logo colado como imagem — perde Component instance, fica difícil atualizar
3. Texto sem Text Style aplicado — hierarquia tipográfica perde
4. Esquecer safe zones — texto cortado pela UI Instagram em Stories/Reels
5. Não atualizar Production Log — perde rastreabilidade
6. Tentar fazer operação que precisa do aluno abrir Figma sem perguntar (algumas operações exigem interação humana — skill admite e pede)

## Frase-âncora

> **"Figma é o estúdio permanente da marca. Brand-guideline define o quê. Esta skill operacionaliza no diário."**
