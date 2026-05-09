---
name: formacao-brand-visual-ia-troubleshooting
description: Skill de debug pra quando output da Formação vier fora do Brand Vocabulary, apresentar problema técnico, ou quando skill atualizada não pegar comportamento novo na conversa atual (cache de sessão). Cobre 6 categorias - humano irreal, logo errado, scale/posição errada, vídeo com bug, content restriction, e skill atualizada não pega + pipeline Claude→Figma quebrado. Aplica fix protocols específicos + mentalidade 'It is not the AI - it is you'. Inclui Multi-Reference Workaround V7→V6.1 + Pro Realism Layer + Logo Fix Workflow + CapCut masking. Use quando o aluno disser - 'troubleshooting', 'output ruim', 'imagem deu errado', 'logo errado', 'video com bug', 'content restriction', 'conta flagada', 'prompt não funciona', 'skill atualizada não pega', 'figma não atualizou', 'pipeline quebrado'. Skill auxiliar — chamada quando algo vai errado.
---

# Troubleshooting — Debug da Formação Branding Visual com IA

> **Cumpre Contrato Comum das Skills v2.0.**

## Propósito

Quando algo no pipeline dá errado — imagem fora do Brand Vocabulary, logo errado, vídeo com bug, content restriction, ou comportamento estranho da skill — esta skill triagem em **6 categorias** e aplica fix protocol específico.

Mentalidade central: **"It's not the AI — it's you."** A maioria dos outputs ruins vem de prompts mal formulados, brand vocabulary fraco, ou pipeline mal montado.

## Quando acionar

- "Troubleshooting / debug"
- "Output ruim / imagem deu errado"
- "Logo errado"
- "Video com bug"
- "Content restriction / conta flagada"
- "Prompt não funciona"
- "Skill atualizada não pega"
- "Figma não atualizou / pipeline Claude→Figma quebrado"

## O que esta skill entrega

- Triagem em 6 categorias com fix protocol específico
- Snapshot do prompt original + diagnóstico do que está fraco
- Workaround técnico documentado por categoria
- Update do Brand Vocabulary quando o problema indica gap

## Pré-requisitos

Output problemático (URL/descrição) + prompt original.

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. `{vault}/marcas/{slug}/brand-guideline.md` (companion MD)
3. Se for problema de pipeline Figma: `figma-file-key.txt`

## As 6 categorias de problema

### Categoria 1 — Humano irreal / plastificado

**Sintomas:** rosto muito polido, sem poros, sem assimetria; pele uniforme demais; expressão "modelo de catálogo Shutterstock"; uncanny valley.

**Fix Protocol — Pro Realism Layer (5 keywords):**
1. `--raw` (Midjourney)
2. `vellus hair` (peluginha facial)
3. `subsurface scattering` (luz penetrando a pele)
4. `small imperfections` (assimetria natural)
5. `unedited photograph` ou `documentary style`

**Combinação:** prompt + `--raw --stylize 100-200`. Em Higgsfield: incluir as keywords no description natural.

### Categoria 2 — Logo errado

**Sintomas:** logo distorcido, com letra errada, posição errada, cor invertida, ou ausente.

**Fix Protocol — Logo Fix Workflow:**
1. **Nano Banana via Higgsfield** pra refazer só a área do logo (instrução: "Replace logo area with reference, keep everything else exactly the same")
2. Se persistir: **recortar logo limpo no Figma → exportar PNG → colar via inpainting**
3. **NUNCA** deixar IA "imaginar" o logo — sempre fornecer referência exata

### Categoria 3 — Scale / posição errada

**Sintomas:** anel "tamanho de prato"; perfume gigantesco no rosto; produto flutuando sem ancoragem física.

**Fix Protocol — Especificar dimensões:**
1. Adicionar **dimensões reais** ao prompt: "8mm ring fitting on ring finger of an adult woman"
2. Adicionar **objeto de referência de escala**: "next to a 5cl coffee cup for scale"
3. Adicionar **constraint físico**: "naturally resting on surface, casting realistic shadow"

### Categoria 4 — Vídeo com bug

**Sintomas:** physics quebrada, movimento robótico, lipsync falhado, transição cortada brusca.

**Fix Protocol:**
1. **Regra dos 3 segundos por clipe** — clipes de 3-5s têm taxa de bug 70% menor que 8-10s
2. **Always image-to-video** — nunca text-to-video puro
3. Se persistir: **masking no CapCut** (default) ou DaVinci Resolve — cortar problema visual e substituir por outro shot
4. Pra lipsync: usar Veo 3 (não Kling) — diferença material na qualidade

### Categoria 5 — Content restriction / conta flagada

**Sintomas:** "moisturizer" trigger NSFW; nome de pessoa real bloqueia; logo de marca conhecida bloqueia; modelo bloqueia categoria sem motivo claro.

**Fix Protocol:**
1. **Renomear**: "moisturizer" → "face cream"; "perfume bottle" → "fragrance container"
2. **Generalizar pessoas reais**: "[Nome]" → "woman 40, similar to [Nome]"
3. **Logos de terceiros**: cortar do prompt, adicionar via Figma depois
4. **Se conta foi flagada**: parar geração, esperar 24h, voltar com prompts mais conservadores
5. Em casos extremos: trocar de plataforma (MJ → Higgsfield ou vice-versa)

### Categoria 6 — Skill atualizada não pega / pipeline Claude→Figma quebrado

**Sintomas:**
- (a) Editou SKILL.md mas Claude age como versão antiga (cache de sessão)
- (b) Claude tentou criar frame no Figma e deu erro
- (c) Figma MCP não autenticado / desconectado
- (d) Tokens de Variable não estão sendo aplicados nos frames novos

**Fix Protocol:**
1. **(a) Cache de skill:** instruir aluno a iniciar **nova conversa** com Claude. Skills carregam no início da conversa, não dinamicamente.
2. **(b) Erro Figma:** rodar `whoami` do MCP Figma pra confirmar autenticação. Se falhar, pedir reconexão.
3. **(c) Desautenticação:** Customize → Connections → Figma → Reconnect.
4. **(d) Variables não aplicadas:** verificar se skill usou `figma.variables.setBoundVariableForPaint()` em vez de fill direto. Se não, refazer com bind correto.

## Padrão de comunicação (Contrato B)

PT-BR direto. Identificar categoria → aplicar fix → validar resultado. Sem floreio.

## Decisões com o aluno (Contrato C)

- **Categoria identificada:** confirmar com aluno antes de aplicar fix (1 pergunta de checkpoint)
- **Fix de plataforma cruzada:** se sugestão é trocar MJ↔Higgsfield, perguntar antes
- **Update do Brand Vocabulary:** se o problema indica gap de documentação, oferecer rodar `brand-guideline-builder` em modo update

## Output e integração downstream (Contrato D)

Salva opcionalmente: `{vault}/marcas/{slug}/troubleshooting/log-{data}.md` com:
- Categoria
- Prompt original
- Fix aplicado
- Resultado
- Lição aprendida

## Quality check (Contrato E)

- Categoria foi corretamente identificada?
- Fix aplicado é o mínimo necessário (não over-engineering)?
- Aluno entendeu a causa-raiz, não só a solução pontual?

## Antipatterns

1. Aplicar fix sem identificar categoria (chute)
2. Pular o checkpoint de confirmação com aluno
3. Recomendar trocar de ferramenta antes de tentar fix dentro da ferramenta atual
4. Não atualizar Brand Vocabulary quando problema é recorrente
5. Tratar IA como culpada sem revisar prompt/setup do aluno

## Frase-âncora

> **"It's not the AI — it's you. A maioria dos outputs ruins vem de prompts mal formulados, brand vocabulary fraco, ou pipeline mal montado. Cada erro é uma chance de dominar o ofício."**
