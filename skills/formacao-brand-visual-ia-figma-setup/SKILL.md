---
name: formacao-brand-visual-ia-figma-setup
description: Skill NOVA do Bloco 3 que cria o estúdio Figma da marca com 12 páginas mestras logo no início (antes do moodboard). Usa MCP Figma pra criar arquivo + páginas (Cover, Moodboard, Brand Guideline, Templates Stories/Carrossel/Feed/Reel Cover/Ad Estático/Ad Vídeo/Newsletter/Pinterest, Production Log) + Variable Collection inicial + Text Styles inicial. Salva figma-file-key.txt no vault. Habilita pipeline Claude→HTML→Figma de todas as skills do Bloco 4. Use quando o aluno disser - 'figma-setup', 'criar estúdio Figma', 'montar arquivo Figma da marca', 'inicializar Figma', 'estúdio da marca', 'preparar Figma para o Bloco 3'. Bloco 3.0 do workflow Formação Branding Visual com IA — primeira skill do Bloco 3, vem antes do moodboard.
---

# Figma Setup — Bloco 3.0 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — skill NOVA na v0.3.0 do plugin. Implementa decisão estratégica do Kevin: Figma é o ambiente vivo desde o DIA 1 do Bloco 3.

## Propósito

Antes do aluno escolher uma cor, fonte ou referência visual, esta skill **cria o arquivo Figma da marca** com 12 páginas mestras prontas. Cada skill do Bloco 3 vai preencher a página correspondente. Cada skill do Bloco 4 vai usar os templates pra produzir peças.

**Sem este passo, todas as outras skills visuais ficam órfãs** — não têm Figma onde aterrissar.

## Quando acionar

- "Figma-setup / criar estúdio Figma"
- "Montar arquivo Figma da marca"
- "Inicializar Figma / estúdio da marca"
- "Preparar Figma para o Bloco 3"

## O que esta skill entrega

**Arquivo Figma** com 12 páginas estruturadas:

```
📄 [Marca] — Brand Studio
├── 📑 Página 0  — Cover (logo + tagline + status do brand-build)
├── 📑 Página 1  — Moodboard (frames vazios pra aluno colar refs)
├── 📑 Página 2  — Brand Guideline (vai ser preenchida ao longo do Bloco 3)
├── 📑 Página 3  — Templates Stories (9:16, safe zones IG)
├── 📑 Página 4  — Templates Carrossel (4:5 e 1:1, 8 frames numerados)
├── 📑 Página 5  — Templates Feed (1:1, hero shot, post educativo, social proof)
├── 📑 Página 6  — Templates Reel Cover (9:16, com safe zones)
├── 📑 Página 7  — Templates Ad Estático (Meta cold + retargeting, 4:5 e 9:16)
├── 📑 Página 8  — Templates Ad Vídeo (storyboard pad)
├── 📑 Página 9  — Templates Newsletter (HTML email mockup)
├── 📑 Página 10 — Templates Pinterest Pin (2:3)
└── 📑 Página 11 — Production Log (todas as peças produzidas, organizadas por data/campanha)
```

**Tokens iniciais:**
- Variable Collection "Brand Tokens" criada (vazia, será preenchida por color-palette)
- Estrutura inicial pra Text Styles (será preenchida por typography)

**Arquivos locais salvos:**
- `{vault}/marcas/{slug}/figma-file-key.txt` — file key do arquivo (CRÍTICO — todas as skills downstream leem)
- `{vault}/marcas/{slug}/figma-pages-inventory.md` — lista das 12 páginas com IDs

## Pré-requisitos

- Bloco 0+1+2 fechados (briefing + 3 pesquisas + 4 docs de tese)
- MCP Figma autenticado (skill checa via `whoami`)
- Aluno tem conta Figma com plano que permite criar arquivo (Free serve pra testar)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. Verificar se `figma-file-key.txt` JÁ existe (se sim, pergunta se é pra recriar ou usar o existente)
3. Rodar `whoami` do MCP Figma pra pegar `planKey` do team

## Fluxo de execução (~20-30 min)

### Fase 1 — Verificar autenticação MCP Figma
Rodar `mcp__...__whoami` pra confirmar autenticação. Se falhar, parar e pedir reconexão.

### Fase 2 — Confirmar nome da marca + plano
Pergunta: "Vamos criar arquivo `[Nome da Marca] — Brand Studio` no team `[planKey]`. OK?"

### Fase 3 — Criar arquivo Figma
`create_new_file` com nome `[Marca] — Brand Studio`, editorType `design`, planKey do team.

### Fase 4 — Criar 12 páginas + estrutura mínima
Rodar `use_figma` com código que:
- Renomeia página inicial pra "Cover"
- Cria as outras 11 páginas com nomes corretos
- Em Cover, cria placeholder de logo + tagline
- Em Templates Stories, cria 1 frame 1080x1920 com safe zones marcadas (220px topo + 420px base)
- Em Templates Carrossel, cria 8 frames 1080x1350 (4:5) numerados
- Em Templates Feed, cria 1 frame 1080x1080
- Em Templates Reel Cover, cria 1 frame 1080x1920 com safe zones
- Em Templates Ad Estático, cria 2 frames (4:5 e 9:16)
- Em Templates Ad Vídeo, cria storyboard pad (5 sub-frames)
- Em Templates Newsletter, cria 1 frame 600px largura
- Em Templates Pinterest Pin, cria 1 frame 1000x1500 (2:3)
- Cria Variable Collection "Brand Tokens" vazia
- Salva file_key + IDs das páginas

### Fase 5 — Salvar referências locais
- `{vault}/marcas/{slug}/figma-file-key.txt` com o file_key
- `{vault}/marcas/{slug}/figma-pages-inventory.md` com lista nome:id de cada página

### Fase 6 — Mostrar pro aluno
Compartilhar URL do Figma + breve passeio pelas páginas. Aluno abre, confirma que está tudo certo.

## Padrão de comunicação (Contrato B)

PT-BR. Quando rodar operações Figma, mostrar o que está fazendo em alto nível ("criando 12 páginas... criando templates Stories com safe zones..."). Não dump JSON cru no chat.

## Decisões com o aluno (Contrato C)

- **Recriar vs reusar:** se figma-file-key.txt JÁ existe, pergunta antes de sobrescrever
- **planKey:** se aluno tem múltiplos teams, pergunta qual usar
- **Customização inicial:** aluno pode pedir páginas adicionais (ex: "adiciona página de Apresentações Comerciais") — skill aceita expansão modesta

## Output e integração downstream (Contrato D)

CRÍTICO: salva `figma-file-key.txt` que TODAS as skills downstream leem:
- `moodboard` (3.1) — preenche Página Moodboard
- `logo-system` (3.2) — cria Components na Página Brand Guideline
- `typography` (3.3) — cria Text Styles vivos
- `color-palette` (3.4) — preenche Variable Collection "Brand Tokens"
- `brand-faces` (3.5) — board de refs na Página Brand Guideline
- `voice-tone` (3.6 — reordenada) — adiciona seção na Página Brand Guideline
- `photography-signature` (3.7) — frase-âncora na Página Brand Guideline
- `videography-signature` (3.8)
- `motion-design` (3.9)
- `brand-guideline-builder` (3.10) — consolida tudo na Página 2 + exporta PDF A4
- `figma` (3.11) — operação do dia a dia
- TODAS as skills do Bloco 4 — usam templates das Páginas 3-10

## Quality check (Contrato E)

- 12 páginas criadas com nomes corretos?
- Templates com tamanhos exatos por plataforma (1080x1920, 1080x1350, etc)?
- Safe zones marcadas em Stories e Reel Cover (retângulos translúcidos vermelhos)?
- Variable Collection criada (mesmo vazia)?
- `figma-file-key.txt` salvo?
- URL do arquivo compartilhada com aluno?

## Antipatterns

1. Pular Fase 1 (autenticação) — vai dar erro silencioso depois
2. Criar arquivo sem `figma-file-key.txt` salvo — quebra todas as skills downstream
3. Usar tamanhos errados nos templates (Stories ≠ 9:16 = problema crítico)
4. Não marcar safe zones em Stories/Reel Cover — aluno coloca texto em zona cortada pelo IG
5. Customização excessiva — skill cria estrutura mínima padrão; expansão vem com pedido explícito do aluno

## Frase-âncora

> **"Figma é o estúdio permanente da marca. Esta skill cria o estúdio. As próximas 12 skills do Bloco 3 mobiliam ele. Sem estúdio criado, marca não tem casa."**
