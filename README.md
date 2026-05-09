# Formação Branding Visual com IA — Plugin Oficial

Plugin Cowork/Claude Code com **38 skills** que conduzem o aluno da Formação Branding Visual com IA do briefing inicial até a produção de qualquer tipo de conteúdo de marca com IA.

## O que o aluno consegue produzir ao final

- **Brand Guideline completo** (Figma vivo + PDF A4 + companion MD)
- **Fotos** (hero shots de produto, lifestyle, beauty, brand faces)
- **Vídeos** (Reels, Stories, vídeos longos)
- **Ads** estáticos e em vídeo (Meta, Pinterest)
- **Carrosséis** educativos e de produto
- **Email flows** (Welcome, Abandoned Cart, Post-purchase)
- **Conteúdo orgânico diário** (calendário 60-30-10)
- **Adaptação multiplataforma** (Instagram, Newsletter, Site, Pinterest)

## Stack-alvo

- **Figma** — protagonista, estúdio permanente da marca, destino final de toda peça
- **Higgsfield** — geração de imagem (Nano Banana) e vídeo (Veo, Kling)
- **Midjourney** — stills de marca + brand faces consistentes via Profile + cref
- **Claude Desktop** — orquestração das skills + escrita de copy + handoff pro Figma
- **CapCut** — edição final de vídeo

## Arquitetura — 5 blocos sequenciais

| Bloco | Função | # Skills |
|---|---|---|
| **0 — Setup** | Captura inicial de hipóteses do dono | 1 |
| **1 — Pesquisas** | Validar hipóteses externamente | 3 |
| **2 — Tese da Marca** | Construir estratégia | 4 |
| **3 — Identidade Visual** | Construir os ativos de marca + Figma vivo | 13 |
| **4 — Produção** | Criar peças com IA | 11 |
| **Aux — Orquestração** | Maestro, diagnóstico, troubleshooting, fechamento | 6 |

## Instalação

### Cowork

```
1. Abre Cowork → Customize → Habilidades
2. Plugins → Add Marketplace → cola URL deste repo
3. Plugin: "Formação Branding Visual com IA" → Install
```

### Claude Code

```bash
claude plugin marketplace add kevinchen-copy/formacao-brand-visual-ia-plugin
claude plugin install formacao-brand-visual-ia
```

## Como usar

Depois de instalado, fala com Claude:

> *"Quero começar minha marca."*

Skill `formacao-brand-visual-ia-maestro` ativa, mostra o mapa do workflow e indica a próxima skill (geralmente `briefing-inicial` ou `diagnostico`).

## Versão

**0.1.0** — Onda 1 (5 skills transversais atualizadas: maestro, diagnostico, troubleshooting, fechamento, brand-vocabulary)

Ver `CHANGELOG.md` pra histórico completo.

## Licença

Apache 2.0 — ver `LICENSE`.

## Suporte

Alunos da Formação: canal exclusivo de suporte na plataforma do curso.
