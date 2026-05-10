# Changelog

Todas as mudanças notáveis neste plugin serão documentadas aqui.

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/), versionamento semântico [SemVer](https://semver.org/lang/pt-BR/).

## [0.3.0] — 2026-05-09 — Onda 3A: Bloco 3 fundação visual (7 skills)

### Adicionado
- Skill **NOVA** `formacao-brand-visual-ia-figma-setup` — primeira do Bloco 3, cria estúdio Figma com 12 páginas mestras + Variable Collection inicial via MCP Figma. Habilita pipeline Claude→HTML→Figma de todas as skills downstream.

### Atualizado
- `formacao-brand-visual-ia-moodboard` — agora preenche Página Moodboard do Figma (não pasta MD); 3 fontes obrigatórias; técnica anti-Pinterest (extract pra esta marca); âncoras culturais nomeadas
- `formacao-brand-visual-ia-logo-system` — 5 variações como Components vivos no Figma com Auto Layout + clear space marcado + grid de tamanhos mínimos + 5-6 usos proibidos
- `formacao-brand-visual-ia-typography` — Text Styles vivos no Figma; taxonomia das Aulas 04-05 do M04 (6 estilos canônicos) + regra dos 3 Cs explícita; alternativa free obrigatória
- `formacao-brand-visual-ia-color-palette` — Color Variables vivas na Variable Collection "Brand Tokens"; 4 camadas (primárias/secundárias/neutras/alertas); harmonia nomeada; acessibilidade WCAG verificada; regra 60-30-10
- `formacao-brand-visual-ia-brand-faces` — alinhada com Aula 07 do M02 (4 caminhos A/B/C/D); 10 dimensões por brand face; alerta crítico sobre etnia explícita (anti content restriction); armadilha demográfica resolvida
- `formacao-brand-visual-ia-voice-tone` — **REORDENADA** pra antes de photography-signature (era 3.9, agora 3.6); 2 camadas (voz permanente × tom variável por contexto); vocabulário favorito + proibido ancorado em market-mapping; 3-5 exemplos pareados on-brand × off-brand

### Princípios editoriais aplicados
- Toda skill conecta com aula(s) específica(s) do M02 (Identidade Visual) e M04 (Pilares de Design)
- Pipeline Claude→Figma documentado em cada skill (não só MD)
- Fontes externas atribuídas com clareza (Eva Heller, Jung, Gestalt cromática)
- Stack-alvo Kevin preservado (sem ChatGPT, Sora, Seedream, Runway)

### Próximas sub-ondas
- **Onda 3B:** 6 skills restantes do Bloco 3 (photography-signature, videography-signature, motion-design, brand-guideline-builder, figma operação, rapid-prototyping)
- **Onda 4:** Bloco 4 — 8 skills atualizadas + 4 skills novas
- **Onda 5:** Validação cruzada + atualização do `_Mapeamento.md` no Obsidian

## [0.2.0] — 2026-05-09 — Onda 2: Bloco 0/1/2 (8 skills estratégicas)

### Adicionado/Atualizado
- Skill `formacao-brand-visual-ia-briefing-inicial` — alinhada às Aulas 1-7 do M01; capta stack do aluno; padronização editorial (Ferra/Cala como exemplos)
- Skill `formacao-brand-visual-ia-audience-research` — 3 níveis de dor + VoC com 30+ quotes + Mapa de Schwartz com atribuição; conecta com Aulas 08-09 e 13-14 do M01
- Skill `formacao-brand-visual-ia-market-mapping` — **REMOVIDA "Lyrae" cravada no corpo** (vazamento de outro projeto); auditoria dos 7 diferenciais virou-entrada (M01 Aula 04); 4 fases de mercado (M01 Aula 02)
- Skill `formacao-brand-visual-ia-product-research` — Matriz Deep Dive (Marcelo Braggion / Copy Sniper) com atribuição limpa; Mecanismo Único em 5-7 passos auditáveis; 4U's pontuados; Mapa de Provas em 5 tipos (M01 Aulas 13-14)
- Skill `formacao-brand-visual-ia-big-idea` — alinhada com tese "diferenciais viraram entrada" (M01 Aula 01) — não "morreram"; Filtros Ogilvy + SUCCESs + Regra do Um com atribuição
- Skill `formacao-brand-visual-ia-positioning` — frase em 4 peças (PARA QUEM + O QUÊ + COMO + PARA QUE); 3 tipos de Reenquadramento (M01 Aula 10); slogan ≤7 palavras; 12 traits Sim/Não; Lei da Escada Mental (Ries & Trout)
- Skill `formacao-brand-visual-ia-ideal-client` — F1∩F2 + auto-imagem aspiracional/evitada (M01 Aula 09); Disciplina do NÃO com 5 perfis recusados + roteiro de redirecionamento educado
- Skill `formacao-brand-visual-ia-tribe-enemy` — alinhada com Aula 16 do M01 (autoral Kevin); 5 perguntas de descoberta + 4 perigos + 3 fórmulas de contraste + 3 peças manifesto + ritual sustentável

### Removido
- Referência a "Lyrae" como exemplo cravado em market-mapping
- Numeração herdada do MEC ("Skill 1-9", "M0-M08") nas 8 skills
- Menções a ChatGPT/Custom GPT, Sora, Seedream, Runway, Pika, Luma como ferramentas oficiais

### Princípios editoriais aplicados
- Toda skill cita aulas específicas do M01 (referência cruzada explícita)
- Atribuições limpas pra frameworks externos: Schwartz, Ogilvy, Heath Brothers, Pareto, Ries & Trout, Marcelo Braggion (Copy Sniper)
- Sem inflação de exemplos travados — exemplos vêm da marca ATIVA do aluno (não cravados na skill)
- Stack-alvo Kevin (Figma + Higgsfield + MJ + CapCut + Claude) preservado

### Próximas ondas
- **Onda 3:** Bloco 3 — 13 skills de identidade visual + nova `figma-setup` adiantada pra início do bloco
- **Onda 4:** Bloco 4 — 8 skills atualizadas + 4 skills novas (`ad-video-creator`, `email-flows`, `carrossel-estatico`, `organico-diario`)
- **Onda 5:** Validação cruzada + atualização do `_Mapeamento.md` no Obsidian

## [0.1.0] — 2026-05-09 — Onda 1: Esqueleto Crítico

### Adicionado
- Estrutura inicial do plugin (manifest, README, LICENSE)
- Skill `formacao-brand-visual-ia-maestro` — orquestrador atualizado: 38 skills mapeadas em 5 blocos, voice-tone reordenado pra antes de photography-signature
- Skill `formacao-brand-visual-ia-diagnostico` — Brand AI-Readiness Assessment com pergunta 15 atualizada (Higgsfield + Figma), roteamento corrigido pra fluxo atual
- Skill `formacao-brand-visual-ia-troubleshooting` — 6 categorias (não 5), CapCut adicionado nos fixes de vídeo, Claude no troubleshoot de skills
- Skill `formacao-brand-visual-ia-fechamento` — recap por blocos atuais (não M0-M08 do MEC), inventário real das 38 skills

### Mudado
- Skill `formacao-brand-visual-ia-brand-vocabulary` convertida em **stub de redirecionamento** pra `briefing-inicial` ou `brand-guideline-builder`. Mantida pra compatibilidade com invocações antigas; conteúdo monolítico aposentado.

### Removido
- Referências a ChatGPT/Custom GPT (substituídas por skills nativas Claude)
- Referências a Sora, Seedream, Runway, Pika, Luma como ferramentas oficiais
- Numeração herdada do MEC (M0-M08, "Skill 1-9") em todas as skills transversais
