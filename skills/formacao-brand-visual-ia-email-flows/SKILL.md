---
name: formacao-brand-visual-ia-email-flows
description: Skill NOVA do Bloco 4 que gera os 3 email flows fundamentais de e-commerce em modos selecionáveis - Welcome Series (5 emails pós-cadastro), Abandoned Cart (3 emails pós-abandono), Post-purchase + Win-back (5 emails pós-compra + 3 emails pra cliente sumido). Aplica voice-tone da marca + 4 padrões de subject line + microcopy + estrutura específica de cada flow. Output em Markdown pronto pra colar em Klaviyo/Mailchimp/RD Station com subject + pré-header + corpo HTML simplificado + microcopy de CTA. Use quando o aluno disser - 'email flow', 'email marketing', 'welcome series', 'abandoned cart', 'post purchase', 'win back', 'klaviyo', 'flow de email'. Bloco 4.5 do workflow Formação Branding Visual com IA — skill nova.
---

# Email Flows — Bloco 4.5 do Workflow (skill NOVA com 3 modos)

> **Cumpre Contrato Comum das Skills v2.0** — skill NOVA na v0.6.0. Preenche gap crítico: 3 aulas dedicadas no Extra-Copy (Aulas 8, 9, 10) sem skill correspondente.
>
> Alinhada às Aulas 08 (Welcome Series), 09 (Abandoned Cart), 10 (Post-purchase + Win-back) e 11 (Subject Lines + Microcopy) do Extra-Copy.

## Propósito

Email é o canal de e-commerce com **maior RPR** (Return Per Recipient — Klaviyo 2024 reporta $3.32 médio em Welcome Series). Maioria das marcas pequenas ignora ou faz mal. Esta skill gera os 3 flows fundamentais em **modos selecionáveis**:

- **Modo Welcome** — 5 emails pós-cadastro (janela emocional 72h)
- **Modo Abandoned** — 3 emails pós-abandono de carrinho (recupera 15-25%)
- **Modo Post-purchase + Win-back** — 5 emails pós-compra + 3 pra cliente sumido (LTV)

## Conexão com o curso

- **Extra-Copy Aula 02 (5 níveis de consciência DTC)** — email vive nos níveis N4-N5
- **Extra-Copy Aula 08 (Welcome Series)** — flow mais lucrativo do e-commerce
- **Extra-Copy Aula 09 (Abandoned Cart)** — pessoa que abandonou já decidiu comprar; remoção de fricção (não venda)
- **Extra-Copy Aula 10 (Post-purchase + Win-back)** — LTV mora aqui; cliente recorrente custa 5-7x menos que cliente novo via Meta
- **Extra-Copy Aula 11 (Subject Lines + Microcopy)** — Regra dos 6; 4 padrões de subject

## Quando acionar

- "Email flow / email marketing"
- "Welcome series / abandoned cart / post purchase / win back"
- "Klaviyo / flow de email"

## Os 3 modos

### Modo Welcome (Extra-Copy Aula 08) — 5 emails

| # | Quando | Conteúdo | Tom |
|---|---|---|---|
| 1 | Imediato | Boas-vindas + cupom (10%) + UMA peça-âncora | Acolhedor, sem agressão |
| 2 | 24h | História da founder + Mecanismo Único da marca | Íntimo (Email mais importante) |
| 3 | 48h | Peça-âncora destacada com narrativa (não promocional) | Curatorial |
| 4 | 4d | Prova social específica (3 depoimentos com nome/idade/cidade) | Confiança |
| 5 | 6d | Última chamada do cupom + diversificação ("se não foi essa peça, talvez essa") | Conclusivo, sem urgência fake |

**Regra de ouro:** 80% conteúdo + 20% CTA. Subjects pessoais > promocionais.

### Modo Abandoned (Extra-Copy Aula 09) — 3 emails

| # | Quando | Conteúdo | Tom |
|---|---|---|---|
| 1 | 1h | Lembrete simples SEM desconto ("Esqueceu?") | Útil, não vendedor |
| 2 | 24h | Remoção de objeção (frete grátis acima de X / garantia / política de troca) | Resolutivo |
| 3 | 48h | Cupom 5-10% + urgência genuína ("seu carrinho expira em 24h") | Final, sem agressão |

**Regra de ouro:** Email 1 SEM DESCONTO (pra não treinar abandono). Limite 3 emails (mais é assédio).

### Modo Post-purchase + Win-back (Extra-Copy Aula 10) — 5 + 3 emails

**Post-purchase (5 emails):**

| # | Quando | Conteúdo |
|---|---|---|
| 1 | Imediato | Confirmação humana (não robô) + agradecimento específico |
| 2 | Pós-envio | Como usar / cuidar do produto |
| 3 | 7-14d | Pedido de review (Trustpilot, Google, redes) |
| 4 | 21-30d | Recomendação cruzada (produto complementar) |
| 5 | 45-60d | Programa de fidelidade ou cashback |

**Win-back (3 emails — pra clientes sumidos 60-120d):**

| # | Quando | Conteúdo |
|---|---|---|
| 1 | Dia 60-90 | "Sentimos sua falta" SEM oferta (apenas conexão) |
| 2 | +14d | Novidades / lançamentos desde a última compra |
| 3 | +30d | Cupom 15%+ (cliente antigo merece desconto melhor que novo) |

## O que esta skill entrega

Pra cada modo selecionado, em `{vault}/marcas/{slug}/emails/{modo}/`:
- Cada email em `.md` com:
  - **Subject** (30-50 chars, 4 padrões: curiosidade contida / promessa específica / pergunta pessoal / menção pessoal)
  - **Pré-header** (segunda chance de abrir)
  - **Body** em HTML simplificado (pronto pra colar em editor de email)
  - **Microcopy CTAs** (verbo + benefício, não "saiba mais")
  - **Microcopy alt-text** de imagens (acessibilidade + cliente com imagens bloqueadas)

## Pré-requisitos

- `brand-guideline-companion.md` (CRÍTICO — voice-tone + Big Idea)
- `bloco-2-3-ideal-client.md` (avatar + auto-imagem)
- `bloco-1-3-product-research.md` (Mecanismo Único + provas)

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `brand-guideline-companion.md`
3. Ideal Client + Product Research

## Fluxo de execução (~60-90 min por modo)

### Fase 1 — Modo selecionado
Aluno escolhe Welcome / Abandoned / Post-purchase. Skill confirma estrutura.

### Fase 2 — Aplicar voice-tone da marca em cada email
Voz permanente + tom variável por contexto. Welcome usa tom mais íntimo; Abandoned mais resolutivo; Post-purchase mais celebrativo.

### Fase 3 — Subject lines (Regra dos 6 da Aula 11 Extra-Copy)
Cada email recebe 2-3 subject candidatos. Aplica 4 padrões:
1. Curiosidade contida
2. Promessa específica
3. Pergunta pessoal
4. Menção pessoal

Anti-padrões evitados: CAIXA ALTA, !!!, "Re:" falso, símbolos demais, genérico.

### Fase 4 — Body em HTML simplificado
HTML responsive simples (não framework — pra colar em editor de email):
- 1 coluna
- Hero image (sugerida)
- Headline H1
- Body 200-400 palavras (Welcome)
- CTA button
- Pré-footer (links sociais + opt-out)

### Fase 5 — Microcopy CTAs
Verbo imperativo + benefício específico. NUNCA "saiba mais" / "compre agora".

### Fase 6 — Salvar estrutura
Em `{vault}/marcas/{slug}/emails/{modo}/email-XX.md` (5 emails Welcome / 3 Abandoned / 5 Post-purchase + 3 Win-back).

## Padrão de comunicação (Contrato B)

PT-BR. Cita Klaviyo como referência de benchmark sem assumir que aluno usa (pode ser Mailchimp, RD Station, Brevo).

## Decisões com o aluno (Contrato C)

- **Modo:** aluno seleciona qual flow rodar primeiro (Welcome é mais comum)
- **Voice modulation:** valida tom escolhido (mais íntimo? mais formal?)
- **Cupom value:** Welcome 10% é padrão; Abandoned 5-10%; Win-back 15%+; aluno aprova

## Output e integração downstream (Contrato D)

Output não tem skill downstream — vai pra plataforma de email do aluno (Klaviyo / Mailchimp / RD Station / Brevo / etc.).

## Quality check (Contrato E)

- Voice-tone da marca aplicado consistentemente nos 5 (ou 3) emails?
- Subjects passam Regra dos 6?
- Pré-header presente em cada email?
- Body responsive (1 coluna)?
- Microcopy CTAs específicos?
- Email 1 do Abandoned SEM desconto (anti-treinamento)?
- Email 2 do Welcome é o mais íntimo (founder story)?

## Antipatterns

1. Welcome 1 com desconto agressivo (treina cliente a esperar 20%)
2. Abandoned mais que 3 emails (vira spam)
3. Post-purchase só com pedido de review (esquece relacionamento)
4. Win-back direto com cupom (sem reconectar antes)
5. Subject genérico em CAIXA ALTA com !!!! (filtro de spam)
6. Body com 5 colunas + 12 imagens (quebra em mobile, vira ilegível)
7. CTA "saiba mais" (perde 30%+ de click)
8. Mencionar plataformas que não existem mais (Mailchimp Mandrill etc.) — usa nomes atuais

## Frase-âncora

> **"Email é o flow mais lucrativo do e-commerce. Email 2 do Welcome (founder story) é o que define se a marca virou marca ou ficou loja."**
