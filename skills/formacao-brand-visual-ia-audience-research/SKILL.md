---
name: formacao-brand-visual-ia-audience-research
description: Pesquisa profunda de audiência aplicando 3 níveis de dor (externo, interno, filosófico) + Voice of Customer (linguagem real do público) + Mapa de Consciência de Eugene Schwartz. Valida ou refuta hipóteses sobre a cliente que vieram do briefing-inicial. Usa pesquisa real na web (Reddit, comentários YouTube, grupos Facebook, Reclame Aqui) sempre que possível. Output é dossiê de audiência com avatar detalhado, dores em 3 níveis, vilões nomeados, linguagem real, gatilhos de compra, mapa antes/depois. Use quando o aluno disser - 'pesquisa de audiência', 'quero entender meu cliente', 'mapeamento de público', 'persona', 'cliente ideal', 'voz do cliente', 'mapeamento de dores', 'nível de consciência', 'audience research'. Bloco 1.1 do workflow Formação Branding Visual com IA — depois de briefing-inicial, antes de market-mapping.
---

# Audience Research — Bloco 1.1 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado às Aulas 8-9 e 13-14 do Módulo 01 do curso autoral (Cliente Ideal + Provas).

## Propósito

Briefing capturou o que o aluno ACHA da cliente. Esta skill **valida ou refuta** essas hipóteses fazendo pesquisa real externa: o que a cliente DIZ, o que SENTE, em que NÍVEL DE CONSCIÊNCIA está, qual é o vilão simbólico contra o qual ela se posiciona.

Output alimenta diretamente: `ideal-client` (F1∩F2), `big-idea` (vazio não-tratado a ocupar), `tribe-enemy` (inimigo simbólico), `static-ads-ecommerce` (10 ângulos de copy).

## Conexão com o curso

- **M01 Aula 08 (Cliente Ideal I — Pareto)** — não tratar base como homogênea
- **M01 Aula 09 (Cliente Ideal II — Ficha + Cliente Negativo)** — densidade psicográfica > demografia; **auto-imagem** como conceito-chave
- **M01 Aula 13 (Provas I)** — entender o ceticismo da cliente vem de dores reais

## Quando acionar

- "Pesquisa de audiência / persona / avatar"
- "Quero entender meu cliente"
- "Voice of customer / VoC"
- "Mapeamento de dores"
- "Nível de consciência / Schwartz"

## O que esta skill entrega

`{vault}/marcas/{slug}/bloco-1-1-audience-research.md` com:

- **Avatar nomeado** (com idade, profissão, contexto, vocabulário próprio)
- **Dores em 3 níveis:**
  - Externa (o que ela RECLAMA em comentário público)
  - Interna (o que ela SENTE mas não fala em público)
  - Filosófica (o que ela QUESTIONA sobre si mesma e o mundo)
- **Vilões nomeados** (não pessoas — comportamentos/ideias contra os quais ela se posiciona)
- **VoC com 30-50 quotes reais** copiadas de fontes externas (Reddit, YouTube, etc.)
- **Mapa de Consciência de Schwartz** — em qual dos 5 níveis a maioria da audiência está (Inconsciente / Consciente do problema / Consciente da solução / Consciente do produto / Mais consciente)
- **Mapa antes/depois** em 5 dimensões (funcional / emocional / status / identidade / relação)
- **10 ganchos de copy testáveis** baseados na pesquisa
- **Quais hipóteses do briefing foram validadas vs refutadas**

## Pré-requisitos

`{vault}/marcas/{slug}/bloco-0-briefing-inicial.md` com hipóteses sobre cliente (geralmente H1, H3, H7).

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `{vault}/marcas/{slug}/bloco-0-briefing-inicial.md` — extrai hipóteses de cliente

## Fluxo de execução (~45-60 min)

### Fase 1 — Definir o universo de busca
A partir das hipóteses do briefing, define onde pesquisar: subreddits específicos, canais YouTube, grupos Facebook, Reclame Aqui, marketplaces.

### Fase 2 — Captura de quotes reais (VoC)
Skill busca via web (com operadores tipo `site:reddit.com "[tema]"`) e copia 30-50 quotes literais. Atribui fonte.

### Fase 3 — Categorização em 3 níveis de dor
Cada quote vira: dor externa / dor interna / dor filosófica.

### Fase 4 — Mapa de Consciência de Schwartz
Identifica em qual dos 5 níveis a maioria está. Atribuído explicitamente (segundo Eugene Schwartz, *Breakthrough Advertising*, 1966).

### Fase 5 — Validação de hipóteses
Cada H do briefing → "validada / refutada / parcialmente validada / nada encontrado" + evidência.

### Fase 6 — Síntese
Avatar nomeado + 10 ganchos de copy + mapa antes/depois.

## Padrão de comunicação (Contrato B)

PT-BR direto. Quotes em VoC sempre marcadas com fonte. Termos clássicos (Schwartz, Pareto, etc.) citados com atribuição.

## Decisões com o aluno (Contrato C)

- **Universo de busca:** propõe 3-5 fontes, aluno aprova/ajusta
- **Avatar nomeado:** propõe 2 nomes, aluno escolhe
- **Hipóteses refutadas:** aluno revisa antes de marcar como "refutada" (pode haver nuance)

## Output e integração downstream (Contrato D)

Consumido por:
- `market-mapping` (1.2) — usa dores filosóficas pra detectar oceano azul
- `product-research` (1.3) — usa objeções da VoC pra mapa de provas
- `big-idea` (2.1) — vazio não-tratado vira tese
- `ideal-client` (2.3) — densidade pro F1∩F2
- `tribe-enemy` (2.4) — vilões nomeados viram inimigo simbólico
- `static-ads-ecommerce` (4.5) — 10 ganchos de copy

## Quality check (Contrato E)

- VoC tem 30+ quotes com fonte atribuída?
- 3 níveis de dor cobertos (não só externa)?
- Mapa de Schwartz aponta nível dominante claro?
- Cada hipótese do briefing recebeu veredicto explícito?

## Antipatterns

1. Inventar quotes (alucinação grave)
2. Pular níveis interno e filosófico (dor externa só vira slogan raso)
3. Não atribuir Schwartz como autor do framework
4. Tratar refutação como "fracasso" do aluno — refutar hipótese é VITÓRIA da pesquisa

## Frase-âncora

> **"A dor externa está no comentário. A dor interna está no desabafo. A dor filosófica está no silêncio entre as frases. Copy de alta conversão escava até o silêncio."**
