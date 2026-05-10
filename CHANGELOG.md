# Changelog

Todas as mudanças notáveis neste plugin serão documentadas aqui.

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/), versionamento semântico [SemVer](https://semver.org/lang/pt-BR/).

## [1.0.0] — 2026-05-09 — Onda 4B FINAL: Outputs específicos + 4 NOVAS skills

🎉 **PLUGIN COMPLETO — 38 SKILLS DISTRIBUÍDAS EM 5 BLOCOS**

### Atualizado
- `formacao-brand-visual-ia-platform-adaptation` — alinhada à Aula 10 do M02; matriz CORE × EXECUTION (5 elementos permanentes × 7 dimensões variáveis); recusa publicar TikTok/LinkedIn por default; 3 trilhas (Figma + Claude Design + edicao)
- `formacao-brand-visual-ia-static-ads-ecommerce` — incorpora 10 tipos do Extra-Copy Aula 05; filtra automaticamente contra Brand Guideline (recusa Direct Offer/PAS em marca quiet luxury); inclui modos UGC e Hooks short-form embutidos; handoff Figma pra montagem final do ad

### Adicionado (4 SKILLS NOVAS)
- `formacao-brand-visual-ia-ad-video-creator` — preenche gap crítico de "ads de vídeo Meta cold"; estrutura específica Hook+Mecanismo+Prova+Reversão+CTA da Aula 04 do Extra-Copy; 3-5 variações de Hook pra teste A/B; specs Meta + captions queimadas; pipeline image-generation + video-prompts + edicao
- `formacao-brand-visual-ia-email-flows` — 1 skill com 3 modos (Welcome 5 emails / Abandoned 3 / Post-purchase 5 + Win-back 3); aplicada às Aulas 8-11 do Extra-Copy; output em MD pronto pra colar em Klaviyo/Mailchimp/RD Station
- `formacao-brand-visual-ia-carrossel-estatico` — estrutura específica de carrossel (não vídeo); pipeline Claude→HTML→Figma com 8-9 frames vivos no template carousel-base; 5 tipos (Educativo/Narrativo/Product Showcase/Social Proof/Drop)
- `formacao-brand-visual-ia-organico-diario` — calendário de 16 posts/mês (Seg/Qua/Sex/Sáb) com regra 60-30-10 + 9 tipos canônicos de post; alinhada à Aula 12 do Extra-Copy; orquestra storyboard + carrossel-estatico + image-generation + figma

### Bloco 4 fechado (12 skills)
storyboard → prompt-builder → image-generation → video-prompts → carrossel-estatico (NOVA) → static-ads-ecommerce → ad-video-creator (NOVA) → email-flows (NOVA) → organico-diario (NOVA) → catalog-coherence → edicao → platform-adaptation

### 🎯 PLUGIN v1.0.0 — Status Final
- **38 skills** distribuídas em 5 blocos (Setup / Pesquisas / Tese / Identidade Visual + Figma vivo / Produção)
- Stack-alvo Kevin preservado em todas: **Figma + Higgsfield + Midjourney + Claude Desktop + CapCut**
- Pipeline Claude→HTML→Figma operacional via MCP Figma
- Brand Guideline gerado em 3 ativos sincronizados (Figma + companion MD + PDF A4)
- Sem ChatGPT/Custom GPT/Sora/Seedream/Runway/Pika/Luma
- Aluno capaz de produzir: fotos, vídeos, ads (estáticos + vídeo), carrosséis, emails, orgânico — TODOS os tipos de conteúdo do briefing original do Kevin

### Próximo passo recomendado
- **Onda 5 (validação cruzada)** — spot-check de 5 skills + atualizar `_Mapeamento.md` no Obsidian + criar `CHANGELOG-skills-v2.md` consolidado
- Rodar uma marca-piloto end-to-end pra validar workflow completo

## [0.5.0] — 2026-05-09 — Onda 4A: Pipeline base de produção (6 skills)

### Atualizado
- `formacao-brand-visual-ia-storyboard` — alinhada às 11 aulas do M03; 5 elementos obrigatórios + Triple Hook + 4 frameworks narrativos + Visual Interest 6 elementos; brief técnico downstream pra `prompt-builder`/`image-generation`/`video-prompts`/`edicao`
- `formacao-brand-visual-ia-prompt-builder` — **MUDANÇA CRÍTICA**: skill nativa Claude Desktop que SUBSTITUI o Custom GPT do ChatGPT (Kevin não usa ChatGPT). 6 camadas (Concept → Subject → Colors+Materials → Composition → Lighting → Camera+Lens) com Lighting/Camera Signatures auto-aplicadas + tradução `↳` PT-BR
- `formacao-brand-visual-ia-image-generation` — Brand Production Process em 5 fases; 5 métodos pra hero shot de produto; 9 hacks Nano Banana; Brand Face cref; scale awareness pra joias; **stack reduzido pra Higgsfield (default) + MJ (alternativa)**
- `formacao-brand-visual-ia-video-prompts` — JSON estruturado em 10 campos + tradução `↳` PT-BR; "always image-to-video"; Videography Signature auto-aplicada; **stack reduzido pra Higgsfield/Veo/Kling — sem Sora/Seedream/Pika/Runway/Luma**
- `formacao-brand-visual-ia-catalog-coherence` — usa hero shot aprovado como âncora; 90% do prompt herdado; 5 métodos (Product Swap default); checklist de coerência em 5 pontos; geração 1 por vez
- `formacao-brand-visual-ia-edicao` — CapCut como protagonista (DaVinci como alternativa); Figma como template-source de overlays/logo/end card; stack de áudio em 3 camadas com volumes específicos; 15-20 itens de quality check pré-publicação

### Princípios editoriais aplicados
- Pipeline Claude→HTML→Figma documentado em cada skill quando aplicável
- Stack-alvo Kevin preservado (sem ChatGPT, Sora, Seedream, Runway, Pika, Luma)
- Prompts/JSONs em INGLÊS pra IA + tradução `↳` PT-BR pro aluno
- Atribuição limpa de aulas-fonte do M03/M05/M06 + Extra-Ofício

### Próxima sub-onda
- **Onda 4B:** 6 skills restantes (platform-adaptation + static-ads-ecommerce atualizadas + 4 skills NOVAS — ad-video-creator + email-flows + carrossel-estatico + organico-diario)

## [0.4.0] — 2026-05-09 — Onda 3B: Bloco 3 assinaturas + consolidação (6 skills)

### Atualizado
- `formacao-brand-visual-ia-photography-signature` — 4 dimensões (lighting/mood/subjects/filter); Lighting Signature + Camera Signature em INGLÊS pronto pra prompt; alinhada às 15 aulas do M05
- `formacao-brand-visual-ia-videography-signature` — 5 decisões (lighting/camera/pacing/grading/transitions); frase-prompt em inglês pra alimentar JSON image-to-video; alinhada às 10 aulas do M06
- `formacao-brand-visual-ia-motion-design` — regra 80/20 (1 style dominante, 1 secundário); easing técnico (cubic-bezier); safe zones por aspect ratio em px; 3 antipatterns por marca
- `formacao-brand-visual-ia-brand-guideline-builder` — **MUDANÇA ESTRUTURAL v2.0**: gera 3 ativos sincronizados (Página 2 do Figma como FONTE DE VERDADE + companion MD machine-readable + PDF A4 EXPORTADO automaticamente do Figma via MCP — não mais via weasyprint paralelo)
- `formacao-brand-visual-ia-figma` — RENOMEADA conceitualmente pra Modo OPERAÇÃO; complementar a `figma-setup` (Modo Setup); operações sob demanda (duplicar template, montar peça, exportar, atualizar Production Log)
- `formacao-brand-visual-ia-rapid-prototyping` — escopo CERCEADO em 3 casos onde Claude Design ganha do Figma (deck/one-pager, prototype site, exploração); SEMPRE remete pra figma quando pedido for repetitivo; Canva minimizado (só destino opcional de handoff)

### Princípios editoriais aplicados
- Figma é PROTAGONISTA absoluto — toda skill aponta pro Figma como destino final
- Pipeline Claude→HTML→Figma documentado em cada skill
- Frases-prompt em INGLÊS pra Lighting/Camera/Videography Signatures (vão pra prompt em IA)
- Stack-alvo Kevin preservado (sem ChatGPT, Sora, Seedream, Runway, Pika, Luma)

### Bloco 3 fechado (13 skills)
Após Onda 3B, o Bloco 3 — Identidade Visual está completo: figma-setup → moodboard → logo-system → typography → color-palette → brand-faces → voice-tone (reordenada) → photography-signature → videography-signature → motion-design → brand-guideline-builder → figma (operação) → rapid-prototyping

### Próxima onda
- **Onda 4:** Bloco 4 — 8 skills atualizadas + 4 skills novas (`ad-video-creator`, `email-flows`, `carrossel-estatico`, `organico-diario`) + opcional `prompt-writer-marca` substituindo Custom GPT

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
