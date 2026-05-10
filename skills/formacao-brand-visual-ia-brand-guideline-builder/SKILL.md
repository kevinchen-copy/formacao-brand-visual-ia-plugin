---
name: formacao-brand-visual-ia-brand-guideline-builder
description: Consolida TODAS as decisões dos Blocos 0, 1, 2 e 3 em 3 ativos sincronizados — Página 2 do Figma (visual diagramado vivo) + brand-guideline-companion.md (machine-readable, lido por TODAS as skills do Bloco 4) + brand-guideline.pdf (A4 portrait, exportado AUTOMATICAMENTE do Figma via MCP, sempre sincronizado). Estrutura em ~18 seções cobrindo essência, posicionamento, cliente ideal, identidade visual completa, voice & tone e style block. Ativa marca como .active-brand pra próximas sessões. Use quando o aluno disser - 'brand guideline', 'consolidar marca', 'livro de marca', 'brand book', 'guideline final', 'PDF da marca', 'design system'. Bloco 3.10 do workflow Formação Branding Visual com IA — última skill da identidade visual antes da operação no Figma e da produção (Bloco 4).
---

# Brand Guideline Builder — Bloco 3.10 do Workflow

> **Cumpre Contrato Comum das Skills v2.0** — alinhado à Aula 11 do M02 (Brand Guidelines: Como Documentar a Marca) + Aula 12 (Aplicação Integrada — Ferra como exemplo canônico).

## Propósito

Esta skill é o **consolidador final do Bloco 3**. Lê TODOS os documentos dos Blocos 0, 1, 2 e 3 e gera o **Brand Guideline da marca em 3 ativos sincronizados**:

1. **Página 2 do Figma — Brand Guideline visual diagramado** (FONTE DE VERDADE) — vai sendo preenchida ao longo do Bloco 3 e finalizada aqui
2. **`brand-guideline-companion.md`** — machine-readable, lido por TODAS as skills do Bloco 4 como source of truth
3. **`brand-guideline.pdf`** — A4 portrait, exportado AUTOMATICAMENTE da Página 2 do Figma via MCP. Sempre sincronizado com o Figma.

Após geração, ATIVA a marca em `.active-brand` pra próximas sessões.

## Conexão com o curso

- **M02 Aula 11 (Brand Guidelines)** — 2 níveis (visual diagramado + Brand Vocabulary Builder operacional); 11 seções mínimas; frase-mãe; "se a marca fosse pessoa"; "a marca nunca"; checklist de estilo visual
- **M02 Aula 12 (Aplicação Integrada — Ferra)** — exemplo canônico final: Marina/Ricardo/Dona Cleusa; paleta Ferrugem #8B3A1F + Carvão #2B2B2B + Cormorant Garamond + Inter

## Quando acionar

- "Brand guideline / consolidar marca / livro de marca / brand book"
- "Guideline final / PDF da marca / design system"

## O que esta skill entrega

### 3 ativos sincronizados:

**1. Página 2 do Figma (FONTE DE VERDADE)**
Brand Guideline visual diagramado em ~18 seções:
1. Essência (Big Idea + manifesto + missão + visão + valores)
2. Posicionamento
3. Cliente Ideal F1∩F2
4. Tribo & Inimigo
5. Escada de Valor (opcional, se documentada)
6. Sistema de Logo (Components vivos)
7. Tipografia (Text Styles vivos)
8. Paleta de Cores (Color Variables vivas)
9. Brand Faces (3 rostos com 10 dimensões cada)
10. Vocabulário Visual / Keywords
11. Moodboard
12. Motion Design
13. Voice & Tom
14. Photography + Videography Signatures
15. Sistema de Provas
16. Brand Style Block paste-ready
17. Do's & Don'ts
18. Apêndices (glossário + versões + créditos)

**2. `{vault}/marcas/{slug}/brand-guideline-companion.md`**
Versão machine-readable das 18 seções em texto puro. Lida automaticamente por TODAS as skills do Bloco 4.

**3. `{vault}/marcas/{slug}/brand-guideline.pdf`**
A4 portrait, exportado AUTOMATICAMENTE via MCP Figma (`export-design` ou similar) consolidando todas as frames da Página 2 numa sequência de páginas. Sempre sincronizado: rodar a skill em modo update gera novo PDF do estado atual do Figma.

**4. `.active-brand` atualizado** — sobrescreve com o slug da marca atual.

## Pré-requisitos

TODOS os documentos dos Blocos 0-3:
- bloco-0-briefing-inicial.md
- bloco-1-1, 1-2, 1-3 (3 pesquisas)
- bloco-2-1, 2-2, 2-3, 2-4 (4 docs de tese)
- bloco-3-1 a 3-9 (9 docs de identidade visual)
- `figma-file-key.txt` (Figma Studio criado)

Se faltar algum: skill PARA e oferece rodar a skill faltante antes.

## Leitura inicial obrigatória (Contrato A)

1. `{vault}/.active-brand`
2. TODOS os 13+ documentos pré-requisito acima
3. `figma-file-key.txt`

## Fluxo de execução (~45-60 min)

### Fase 1 — Verificação dos pré-requisitos
Skill checa quais docs existem. Lista o que falta. Aluno decide se preenche ou marca como `[pendente]`.

### Fase 2 — Consolidação no companion MD
Skill compõe o `brand-guideline-companion.md` em 18 seções puxando dos arquivos anteriores. Sem inventar — apenas estruturar e referenciar.

### Fase 3 — Diagramação na Página 2 do Figma
Via MCP, skill cria/atualiza frames na Página 2 do Figma com cada uma das 18 seções diagramadas:
- Logo System (puxa Components da Página Brand Guideline já criados pelo `logo-system`)
- Tipografia (mostra Text Styles em uso)
- Paleta (mostra Color Variables aplicadas em swatches)
- Brand Faces (board com 3 rostos)
- Reference shots de photography/videography
- Motion Style Block
- Voice & Tom em tabela
- Etc.

Cada seção um frame ou conjunto de frames numerados (Section 01, Section 02...).

### Fase 4 — Export do PDF A4
Via MCP Figma, exportar TODAS as frames da Página 2 em ordem como PDF A4 portrait. Salvar como `brand-guideline.pdf` em `{vault}/marcas/{slug}/`.

### Fase 5 — Atualização de .active-brand
Sobrescreve `{vault}/.active-brand` com slug da marca.

### Fase 6 — Apresentação dos 3 ativos + próximos passos
Skill mostra:
1. Link do Figma (Página 2)
2. Path do companion MD
3. Path do PDF gerado

E sugere próxima skill: `figma` (Bloco 3.11) pra modo Operação OU direto Bloco 4 se aluno quer pular pra produção.

## Padrão de comunicação (Contrato B)

PT-BR. Quando mostrar HEX, fonte, frase técnica, sempre formato técnico legível. Cita Aula 11 e 12 do M02 como referência didática.

## Decisões com o aluno (Contrato C)

- **Documentos faltantes:** se algum Bloco anterior não foi feito, skill pergunta se prefere PARAR e completar OU gerar com `[pendente]` marcado
- **Versão do guideline:** se já existe v1.0, pergunta se é v2.0 ou se sobrescreve
- **Aprovação visual da Página 2 do Figma:** aluno revisa antes do export do PDF

## Output e integração downstream (Contrato D)

Salva:
- `{vault}/marcas/{slug}/brand-guideline-companion.md` (machine-readable, TODAS as skills do Bloco 4 leem)
- `{vault}/marcas/{slug}/brand-guideline.pdf` (apresentável, sincronizado com Figma)
- Página 2 do Figma atualizada
- `.active-brand` atualizado

Consumido por:
- TODAS as skills do Bloco 4 — leem o companion MD como source of truth
- `figma` (Bloco 3.11) — opera o estúdio que esta skill consolidou
- `rapid-prototyping` (3.12) — usa Página 2 como referência pra Claude Design

## Quality check (Contrato E)

- 18 seções existem (mesmo que algumas marcadas `[pendente]`)?
- Página 2 do Figma diagramada visualmente (não só texto)?
- PDF A4 exportado AUTOMATICAMENTE do Figma (não geração paralela em weasyprint)?
- Companion MD coerente com Figma e PDF (3 ativos sincronizados)?
- `.active-brand` foi atualizado?
- Versão registrada (1.0, 1.1, 2.0)?

## Antipatterns

1. Inventar conteúdo pra preencher seção faltante — sempre marca `[pendente]`
2. Pular geração do PDF — só MD não é apresentável
3. Não atualizar `.active-brand` — quebra todas as skills downstream
4. Gerar PDF via weasyprint paralelo (a v2.0 mudou: PDF é EXPORT do Figma, não build separado)
5. Sobrescrever versão antiga sem versionar (perde histórico)
6. Companion MD divergente do Figma (3 ativos precisam estar sincronizados — fonte de verdade é o Figma)

## Frase-âncora

> **"Brand Guideline é o ativo alavancador infinito. Uma vez sólido, alimenta todas as skills downstream — geração de imagem, vídeo, edição, ads. Sem ele, IA produz ruído bonito. Com ele, IA amplifica identidade replicável."**
