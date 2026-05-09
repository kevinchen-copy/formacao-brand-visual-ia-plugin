---
name: formacao-brand-visual-ia-diagnostico
description: Conduz o aluno pelo Brand AI-Readiness Assessment da Formação Branding Visual com IA — 20 perguntas em 5 dimensões (Brand Foundation, Content Creation, Technical Readiness, Market Positioning, Mindset) que diagnosticam se a marca tem fundação pra produzir conteúdo com IA de forma consistente. Calcula score 0-60, classifica em 4 níveis (Starting Line / Foundation First / Almost There / AI-Ready Champion) e entrega plano de ação personalizado indicando exatamente qual skill ativar a seguir. Funciona como co-piloto interativo — pergunta uma de cada vez, calcula automaticamente, entrega diagnóstico completo. Acione SEMPRE que o aluno mencionar diagnóstico de marca, brand readiness, AI readiness, avaliação de prontidão pra IA, assessment de marca, minha marca está pronta pra IA, quero saber meu nível, diagnóstico inicial, antes de começar a formação, por onde devo começar a formação.
---

# Diagnóstico — Brand AI-Readiness Assessment

> **Skill auxiliar de onboarding.** Cobre o assessment inicial. Porta de entrada após o Maestro: diagnostica em que nível a marca do aluno está e indica exatamente por onde começar a jornada.

## COMO ESTA SKILL OPERA

### Modo Co-piloto (DEFAULT — quando aluno quer fazer o assessment)

Quando o aluno disser *"quero fazer o diagnóstico"*, *"qual meu nível"*, *"por onde começo"*, ou aceitar a sugestão do Maestro de fazer o assessment, **você (Claude) conduz o assessment passo a passo**:

1. Apresenta a estrutura (20 perguntas, 5 dimensões, ~10 minutos)
2. Faz **uma pergunta por vez** com as 3 opções de resposta (YES / SOMEWHAT / NO)
3. Acumula a pontuação internamente sem mostrar entre perguntas
4. No fim, calcula o score total, classifica o nível, e entrega o **diagnóstico personalizado** com plano de ação específico pro nível
5. Roteia pra próxima skill da formação

### Modo Ensino (reativo — quando aluno só quer entender)

Quando o aluno perguntar *"o que é o assessment?"* / *"como funciona o diagnóstico?"* / *"quais as dimensões?"*, **explica** a estrutura sem rodar o assessment, e oferece rodar em seguida.

## O QUE O ASSESSMENT MEDE

| Dimensão | O que mede | # perguntas |
|---|---|---|
| **Brand Foundation** | Identidade documentada, paleta, persona, consistência visual | 5 |
| **Content Creation** | Frequência, eficiência, satisfação atual com qualidade | 3 |
| **Technical Readiness** | Sistemas, organização, conforto com Figma/Higgsfield/Midjourney/CapCut/Claude | 7 |
| **Market Positioning** | Conhecimento de concorrência, diferenciação, alinhamento com goals | 3 |
| **Mindset** | Abertura a mudar workflow, prioridade pro visual | 2 |

**Total:** 20 perguntas. Score máximo: 60 pontos.

## ESCALA DE PONTUAÇÃO

- **YES (3 pontos)** — situação ideal, totalmente atendido
- **SOMEWHAT (1 ponto)** — parcial, em desenvolvimento
- **NO (0 pontos)** — gap, ainda não atendido

**Atenção — Pergunta 7 tem escala invertida:** gasta mais de 2h por peça — *YES significa NO efetivo* (problema, score 0).

## OS 4 NÍVEIS DE PRONTIDÃO

| Faixa | Nível | Significado |
|---|---|---|
| **50-60** | 🏆 **AI-Ready Champion** | Fundação sólida, sistemas organizados, técnico-confortável |
| **35-49** | 🎯 **Almost There** | Boa fundação, gaps pontuais |
| **20-34** | 🏗️ **Foundation First** | Identidade precisa de clarificação |
| **0-19** | 🌱 **Starting Line** | Início da jornada |

## AS 20 PERGUNTAS

### Brand Foundation (1-5)

**1. Você tem documento de identidade visual da sua marca?**
- YES (3): brand guidelines documentado com cores, fontes, direção visual
- SOMEWHAT (1): alguns elementos definidos mas não documentados
- NO (0): ainda definindo identidade

**2. Você consegue descrever a personalidade da sua marca em 5 palavras?**
- YES (3): nomeio traços de personalidade na hora
- SOMEWHAT (1): tenho ideia geral mas não claramente definida
- NO (0): personalidade pouco clara

**3. Você tem audiência-alvo definida com demografia E psicografia específicas?**
- YES (3): sei exatamente quem + o que valorizam
- SOMEWHAT (1): ideia geral
- NO (0): atendendo todo mundo

**4. As cores da sua marca estão definidas com códigos HEX específicos?**
- YES (3): especificações exatas documentadas
- SOMEWHAT (1): conheço a paleta geral
- NO (0): escolho cores aleatoriamente

**5. Você tem elementos visuais consistentes em todo seu conteúdo atual?**
- YES (3): conteúdo coeso e reconhecível
- SOMEWHAT (1): alguma consistência com espaço pra melhorar
- NO (0): conteúdo disperso

### Content Creation (6-8)

**6. Você cria conteúdo visual regularmente (pelo menos 3x/semana)?**
- YES (3): consistente
- SOMEWHAT (1): irregular
- NO (0): esporádico

**7. Você gasta MAIS de 2 horas criando uma única peça?** ⚠️ *(escala invertida)*
- YES (0): muito tempo por peça (problema)
- SOMEWHAT (1): às vezes demora
- NO (3): processos eficientes

**8. Está satisfeito com a qualidade visual do seu conteúdo atual?**
- YES (3): profissional e on-brand
- SOMEWHAT (1): decente
- NO (0): precisa melhorar

### Technical Readiness (9-15)

**9. Tem calendário ou sistema de planejamento de conteúdo?**
- YES (3): planejo com antecedência
- SOMEWHAT (1): algum planejamento
- NO (0): reativo

**10. Adapta rapidamente conteúdo pra diferentes plataformas?**
- YES (3): facilmente
- SOMEWHAT (1): adapto mas dá trabalho
- NO (0): posto o mesmo em todo lugar

**11. Confortável aprendendo novas ferramentas digitais?**
- YES (3): gosto de explorar
- SOMEWHAT (1): aprendo quando necessário
- NO (0): tecnologia me intimida

**12. Tem sistema pra organizar e armazenar assets visuais?**
- YES (3): organização clara
- SOMEWHAT (1): bagunçado
- NO (0): difícil de achar

**13. Usa Figma com algum nível de conforto?**
- YES (3): confortável (Variables, Components, Auto Layout)
- SOMEWHAT (1): básico (criar frames, editar texto)
- NO (0): nunca usei

**14. Usa CapCut (ou DaVinci Resolve) pra editar vídeo?**
- YES (3): confortável (timeline, transitions, color grading básico)
- SOMEWHAT (1): básico
- NO (0): evito

**15. Já usa alguma ferramenta de IA visual (Midjourney, Higgsfield, Nano Banana)?**
- YES (3): confortável com pelo menos uma
- SOMEWHAT (1): testei mas não uso regularmente
- NO (0): nunca usei IA pra imagem/vídeo

### Market Positioning (16-18)

**16. Sabe que estilo visual seus concorrentes usam?**
- YES (3): analiso regularmente
- SOMEWHAT (1): vejo ocasionalmente
- NO (0): não presto atenção

**17. Identifica o que faz sua marca visualmente diferente dos concorrentes?**
- YES (3): diferenciadores claros
- SOMEWHAT (1): alguns elementos
- NO (0): difícil de me diferenciar

**18. Tem estratégia de conteúdo alinhada com objetivos de negócio?**
- YES (3): suporta objetivos diretamente
- SOMEWHAT (1): alinha vagamente
- NO (0): sem propósito claro

### Mindset (19-20)

**19. Está aberto a mudar workflow atual de criação de conteúdo?**
- YES (3): aberto a abordagens novas
- SOMEWHAT (1): algumas mudanças
- NO (0): quero manter processo

**20. Acredita que conteúdo visual vai se tornar mais importante pro negócio?**
- YES (3): crítico pro crescimento
- SOMEWHAT (1): importante
- NO (0): não é prioridade

## DIAGNÓSTICO POR NÍVEL — O QUE ENTREGAR APÓS O CÁLCULO

### 🌱 STARTING LINE (0-19)

**Mensagem-chave:** *Você está no começo da jornada — perfeito. Tem potencial enorme construindo certo desde o começo.*

**Plano de ação:**
1. **Não pula direto pra Bloco 4 (produção com IA).** Marca sem fundação + IA = ruído bonito mais rápido.
2. **Próxima skill:** `formacao-brand-visual-ia-briefing-inicial` (Bloco 0)
3. Sequência: Bloco 0 → Bloco 1 (pesquisas) → Bloco 2 (tese) → Bloco 3 (identidade visual + Figma) → Bloco 4 (produção)
4. **Tempo estimado pra ficar pronto pra IA:** 3-5 semanas focadas

**Foco imediato:**
- Definir personalidade da marca em 5 palavras
- Definir audiência-alvo específica
- Estabelecer ritmo regular de criação (3x/semana mínimo)
- Aprender Figma básico (Variables, Components)

### 🏗️ FOUNDATION FIRST (20-34)

**Mensagem-chave:** *Você já tem direção, mas a fundação ainda precisa ser solidificada antes de escalar com IA.*

**Plano de ação:**
1. **Próxima skill:** `formacao-brand-visual-ia-briefing-inicial` (Bloco 0) pra organizar hipóteses
2. Foca nas dimensões que você tirou 0-1 pontos
3. Após Bloco 0, segue: Bloco 1 → 2 → 3 → 4
4. **Tempo estimado pra evoluir pro próximo nível:** 2-4 semanas

**Pontos de atenção:**
- Se tirou NO em #4 (HEX), prioriza paleta documentada (vai aparecer em `color-palette` no Bloco 3)
- Se tirou NO em #2 (personalidade), prioriza voice-tone (Bloco 3)
- Se tirou NO em #13 (Figma), considere antes de começar: tutorial básico Figma (1-2h) ou usa Canva enquanto evolui

### 🎯 ALMOST THERE (35-49)

**Mensagem-chave:** *Fundação sólida. Falta refinar pontos específicos e estruturar pra produzir em escala com IA.*

**Plano de ação:**
1. **Identifica os gaps específicos** — quais perguntas tirou 0-1?
2. **Se gaps em Brand Foundation:** rode `briefing-inicial` ou pule pra `figma-setup` se já tem identidade
3. **Se gaps em Technical Readiness:** começa `figma-setup` direto pra montar o estúdio Figma
4. **Próxima skill recomendada:** `formacao-brand-visual-ia-figma-setup` (Bloco 3.0) — monta o estúdio Figma com 12 páginas
5. **Tempo estimado pra atingir Champion:** 2-4 semanas de prática consistente

**Pontos de atenção:**
- Você já tem o suficiente pra começar a produzir com IA — não fica preso em "preparar pra sempre"
- Refina enquanto produz: cada peça nova revela mais do que precisa documentar

### 🏆 AI-READY CHAMPION (50-60)

**Mensagem-chave:** *Sua marca tem fundação forte e você está tecnicamente pronto. Bora construir o motor de produção imediatamente.*

**Plano de ação:**
1. **Próxima skill:** `formacao-brand-visual-ia-figma-setup` (montar estúdio se ainda não tem) OU `formacao-brand-visual-ia-storyboard` (Bloco 4) se já tem
2. **Foco imediato:** construir biblioteca de prompts canônicos da marca + pipeline Claude → HTML → Figma rodando
3. Pode rodar a formação em **velocidade acelerada** — domine 1 bloco por semana
4. **Tempo estimado pra escala plena:** 4-8 semanas de execução

## ROTEIRO PARA CONDUZIR O ASSESSMENT

### Etapa 1 — Abertura

> "Vou te conduzir pelo Brand AI-Readiness Assessment — 20 perguntas em 5 dimensões. Leva entre 8-12 minutos. Pra cada pergunta, você responde **YES / SOMEWHAT / NO**. No final, te dou o score, classifico em 1 dos 4 níveis, e mostro exatamente por onde começar na formação. Bora?"

Aguarda confirmação. Se aluno hesitar, oferece versão rápida ("posso te dar uma versão de 5 perguntas mais críticas").

### Etapa 2 — Conduzir as 20 perguntas

**Faça uma de cada vez.** Numera (ex: "Pergunta 1 de 20...") pra manter senso de progresso.

**Anota internamente** a pontuação a cada resposta. NÃO mostra running score entre perguntas.

A cada 5 perguntas, dá um respiro: *"5 de 20 ✅."*

### Etapa 3 — Cálculo

```
Brand Foundation: ___ / 15
Content Creation: ___ / 9
Technical Readiness: ___ / 21
Market Positioning: ___ / 9
Mindset: ___ / 6

SCORE TOTAL: ___ / 60
NÍVEL: [Champion / Almost There / Foundation First / Starting Line]
```

### Etapa 4 — Diagnóstico personalizado + plano de ação

Entrega na ordem:
1. Score breakdown por dimensão
2. Nível com explicação
3. Plano de ação imediato (próxima skill)
4. Pontos de melhoria específicos

## REVALIDAÇÃO PERIÓDICA

Sugere ao aluno **revalidar a cada 60-90 dias**. Marca evolui, score sobe.

## INTEGRAÇÃO COM AS OUTRAS SKILLS

| Nível detectado | Próxima skill recomendada | Por quê |
|---|---|---|
| Starting Line | `briefing-inicial` (Bloco 0) | Fundação não-negociável |
| Foundation First | `briefing-inicial` (Bloco 0) | Refinar onde tem gaps |
| Almost There | `figma-setup` (Bloco 3.0) ou `briefing-inicial` seletivo | Montar estúdio + avançar |
| Champion | `figma-setup` (Bloco 3.0) ou `storyboard` (Bloco 4.1) | Produção em escala |

**Sempre confirma com o aluno antes de rotear:** *"Quer ir agora pra próxima skill, ou prefere pausar e revisitar depois?"*

## REGRAS DE COMUNICAÇÃO

- PT-BR sempre
- Tom direto e supportive — diagnóstico não é julgamento, é mapa
- Uma pergunta por turno
- Numera o progresso
- NUNCA mostra running score entre perguntas
- NUNCA julga respostas
- Termina com plano de ação concreto

## O QUE ESTA SKILL NÃO FAZ

- ❌ Não ensina conteúdo dos blocos — apenas diagnostica e roteia
- ❌ Não tenta resolver gaps na hora
- ❌ Não roteia pra `brand-vocabulary` (skill aposentada)
- ❌ Não cita ChatGPT/Custom GPT (fora do stack)

## Frase-âncora

> **"Diagnóstico não é julgamento — é mapa. Quanto mais preciso o diagnóstico, mais rápido o caminho."**
