# Changelog

Todas as mudanças notáveis neste plugin serão documentadas aqui.

Formato baseado em [Keep a Changelog](https://keepachangelog.com/pt-BR/1.0.0/), versionamento semântico [SemVer](https://semver.org/lang/pt-BR/).

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
- Referências a Sora, Seedream, Runway, Pika, Luma como ferramentas oficiais (mantidas só como menção contextual onde aplicável)
- Numeração herdada do MEC (M0-M08, "Skill 1-9") em todas as skills transversais

### Próximas ondas
- **Onda 2:** Bloco 0/1/2 — 8 skills estratégicas alinhadas com M01 do curso autoral
- **Onda 3:** Bloco 3 — 13 skills de identidade visual + nova `figma-setup` adiantada pra início do bloco
- **Onda 4:** Bloco 4 — 8 skills atualizadas + 4 skills novas (`ad-video-creator`, `email-flows`, `carrossel-estatico`, `organico-diario`)
- **Onda 5:** Validação cruzada + atualização do `_Mapeamento.md` no Obsidian
