---
name: formacao-brand-visual-ia-fechamento
description: Skill de fechamento e graduação da Formação Branding Visual com IA. Conduz reflexão estruturada sobre a jornada (Blocos 0-4), entrega documento de plano de implementação 30/90/365 dias, ajuda definir métricas baseline (tempo/peça atual, custo, frequência) pra comparar em 30 dias, formaliza compromisso público, e orienta protocolo de pay-it-forward pra ajudar outras marcas pequenas. Acione SEMPRE que o aluno mencionar terminei a formação, acabei o curso, fechamento, graduação, plano daqui pra frente, próximos 30 dias, próximos 90 dias, plano de implementação, missão da formação, ética de IA em marca.
---

# Fechamento — Graduação da Formação Branding Visual com IA

> **Skill auxiliar de encerramento.** Última skill da jornada. Cobre missão da formação, ética de uso de IA em branding, recap consolidado dos 5 blocos / 38 skills, e plano de implementação personalizado de 30/90/365 dias.

## Propósito

O aluno terminou (ou está terminando) os 5 blocos da formação. Esta skill faz o **fechamento ritualizado** — não é mais uma aula, é uma transição da fase de aprendizado pra fase de execução autônoma.

Entrega um documento `.md` com plano de implementação concreto que ele vai usar nos próximos 30/90/365 dias.

## Quando acionar

- "Terminei a formação"
- "Acabei o curso"
- "Fechamento / graduação"
- "Plano daqui pra frente"
- "Próximos 30 dias / 90 dias"
- "Plano de implementação"

## O que esta skill entrega

`/mnt/user-data/outputs/plano-formacao-brand-visual-ia-{nome-aluno}.md` com 8 seções:

1. **Reflexão consolidada** sobre a jornada (5 blocos atravessados)
2. **Sistema de produção** (skills + ferramentas que ele agora domina)
3. **Princípios éticos** de uso de IA em branding
4. **Métricas baseline** atuais (pra comparar em 30 dias)
5. **Plano 30 dias** — estabilização do pipeline
6. **Plano 90 dias** — escala e refinamento
7. **Plano 365 dias** — visão de 1 ano
8. **Compromisso público + pay-it-forward**

## Pré-requisitos

Aluno terminou (ou está em estágio avançado de) os 5 blocos da formação. Idealmente:
- ✅ Bloco 0 — briefing-inicial fechado
- ✅ Bloco 1 — 3 docs de pesquisa fechados
- ✅ Bloco 2 — 4 docs de tese fechados
- ✅ Bloco 3 — Brand Guideline (PDF + Figma + companion MD) fechado
- ✅ Bloco 4 — pelo menos 3 peças produzidas com pipeline Claude→Figma

## Fluxo de execução (~45-60 min de conversa)

### Fase 1 — Reflexão estruturada

Conduz o aluno por 5 perguntas (1 por bloco):

1. **Bloco 0:** *"Que hipótese sua sobre a marca foi MAIS refutada pelas pesquisas?"*
2. **Bloco 1:** *"Qual descoberta de cliente, mercado ou produto te surpreendeu mais?"*
3. **Bloco 2:** *"Qual frase do seu posicionamento atual você nunca teria escrito sem a formação?"*
4. **Bloco 3:** *"Que decisão de identidade visual você teria tomado errado se tivesse improvisado?"*
5. **Bloco 4:** *"Qual peça produzida você compartilharia como exemplo do seu nível atual?"*

Captura as respostas em prosa contemplativa (não bullet) — vai pra Seção 1 do documento.

### Fase 2 — Recap do sistema

Skill lista:

**Documentos da fundação** (em `{vault}/marcas/{slug}/`):
- briefing-inicial.md
- audience-research.md, market-mapping.md, product-research.md
- big-idea.md, positioning.md, ideal-client.md, tribe-enemy.md
- brand-guideline.md (companion MD)
- brand-guideline.pdf (visual diagramado A4)
- design-system.md (formato Google open-source)

**Estúdio Figma vivo:**
- Brand Studio com 12 páginas
- Variables (Brand Tokens)
- Text Styles
- Templates: Stories, Carrossel, Feed, Reel Cover, Ad Estático, Ad Vídeo, Newsletter, Pinterest

**Pipeline de produção dominado:**
- Claude orquestra skills
- Higgsfield + Midjourney geram imagem/vídeo
- CapCut edita vídeo
- Figma é destino final de toda peça

### Fase 3 — Princípios éticos (não-negociáveis)

Apresenta ao aluno as **3 regras éticas absolutas** da formação:

1. **IA é tradutora, não criadora.** Marca forte + IA = amplificação. Marca vaga + IA = ruído genérico. Não use IA pra esconder ausência de fundação.
2. **Real com detalhe supera ficção com lustre.** Use IA pra amplificar o que é real (Dona Lourdes existe, a peça existe, a fornecedora existe). Não invente provas, depoimentos, números, casos.
3. **Logos, rostos e marcas de terceiros respeitados.** Não usa IA pra clonar visual de concorrente, não usa rosto de pessoa real sem consentimento, não copia campanha alheia trocando produto.

E **3 práticas encorajadas:**

1. **Compartilhar processo, não só resultado.** Mostra Reels de bastidor, prompts usados, decisões tomadas — isso é educacional pra o mercado.
2. **Documentar erros e correções.** Cada bug que vira aprendizado vira ativo da marca.
3. **Pay-it-forward.** Após dominar a formação, ajudar 3 outras marcas pequenas (gratuitamente ou trocando) acelera o ofício do mercado inteiro.

### Fase 4 — Métricas baseline

Captura as 4 métricas atuais do aluno (vai virar referência pra 30 dias):

1. **Tempo médio por peça** (ad estático, Reel, carrossel) — em horas
2. **Custo médio por peça** (incluindo MJ + Higgsfield + Figma + tempo) — em R$
3. **Frequência de publicação atual** (peças/semana)
4. **Taxa de conformidade com brand guideline** (% peças que passariam quality check)

Exemplo: *"Hoje: 4h por Reel, R$80 custo, 2 Reels/semana, 60% conformidade."*

### Fase 5 — Plano 30 dias (estabilização)

Skill propõe 4 metas SMART pros 30 dias:

1. **Tempo:** reduzir de Xh pra Yh por peça (sugere -40%)
2. **Custo:** manter ou reduzir
3. **Frequência:** aumentar de X pra Y peças/semana (sugere +50%)
4. **Conformidade:** subir pra 90%+ (Brand Guideline aplicado em quality check)

Aluno aprova ou ajusta.

### Fase 6 — Plano 90 dias (escala)

Foco em:
- Construir biblioteca de **20+ prompts canônicos** da marca (reutilizáveis)
- Estabelecer **calendário orgânico mensal** rodando com `organico-diario`
- Lançar primeira **campanha Multi-format completa** (Reel + 3 ads + carrossel + email + stories)
- Revalidar `diagnostico` (esperando subir 1 nível)

### Fase 7 — Plano 365 dias (visão)

Foco em:
- **20+ peças de portfolio** documentadas
- **Marca reconhecível** no nicho (cliente identifica em 2s sem ver logo)
- **Pipeline 100% autônomo** (aluno não depende mais da formação ativa)
- Decidir se vira **referência educacional** (ensina outros) ou foca em escalar próprio negócio

### Fase 8 — Compromisso público + pay-it-forward

- **Compromisso público:** aluno escreve 1 frase pública (post Instagram, story, newsletter) afirmando o que vai fazer nos próximos 30 dias. Ato de "travar" a decisão.
- **Pay-it-forward:** aluno escolhe 3 marcas pequenas que vai ajudar (mentoria curta, feedback de identidade, ou indicação da formação). Anota nomes.

## Padrão de comunicação (Contrato B)

PT-BR contemplativo no início (Fase 1), executável no meio (Fases 4-7), inspirador no fim (Fase 8). Sem exclamação. Sem "parabéns!" genérico — específico ao que o aluno construiu.

## Decisões com o aluno (Contrato C)

- **Cada meta SMART** — aluno aprova ou ajusta antes de salvar
- **Pay-it-forward** — aluno escolhe livremente as 3 marcas (sem sugestão imposta)
- **Compromisso público** — aluno escreve a frase com sua voz, não a skill

## Output e integração downstream (Contrato D)

Salva: `/mnt/user-data/outputs/plano-formacao-brand-visual-ia-{slug-marca}-{data}.md` com as 8 seções.

Sugere ao aluno revalidar o `diagnostico` em 60 dias.

## Quality check (Contrato E)

- 8 seções estão preenchidas?
- Métricas baseline têm número específico (não "vou melhorar")?
- Compromisso público é específico (não "vou tentar")?
- Pay-it-forward tem 3 nomes (não "vou ajudar pessoas")?

## Antipatterns

1. Recap usar numeração antiga MEC (M0-M08, "Skill 1-9") — sempre Blocos 0-4 + Aux
2. Listar ferramentas fora do stack (ChatGPT, Sora, Seedream) no recap
3. Dar parabéns genérico em vez de reconhecer o que foi construído
4. Pular Fase 4 (métricas baseline) — sem baseline, plano 30/90/365 fica abstrato
5. Forçar o aluno a fazer pay-it-forward (oferecer, mas respeitar se não quiser agora)

## Frase-âncora

> **"Não é fim. É começo. Cada erro é uma chance de dominar o ofício. A formação te entregou o sistema; daqui pra frente o ofício é teu."**
