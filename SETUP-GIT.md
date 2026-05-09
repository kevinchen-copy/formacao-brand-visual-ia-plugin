# Setup Git — Primeira instalação

> Este arquivo te dá os comandos exatos pra inicializar o repo, criar no GitHub privado e fazer o primeiro push. Depois disso, dá pra deletar este arquivo (ou guardar pra referência).

## Pré-requisitos

- ✅ Git instalado e configurado no PC
- ✅ Conta GitHub (`kevinchen-copy`) — você confirmou que já tem
- ✅ Autenticação Git ↔ GitHub funcionando (HTTPS com token OU SSH)

## Passo 1 — Limpar a pasta `.git/` capenga (que o sandbox criou)

A pasta `.git/` dentro de `formacao-brand-visual-ia-plugin/` está parcialmente criada e quebrada. Apaga ela manualmente:

**Windows:**
```
1. Abre o Explorador de Arquivos
2. Vai em: C:\Users\Kevin\Documents\Obsidian Vault\Formacao-Branding-Visual-com-IA\formacao-brand-visual-ia-plugin\
3. Habilita "Mostrar arquivos ocultos" (View → Show → Hidden items)
4. Apaga a pasta .git\
```

**Ou via PowerShell:**
```powershell
Remove-Item -Recurse -Force "C:\Users\Kevin\Documents\Obsidian Vault\Formacao-Branding-Visual-com-IA\formacao-brand-visual-ia-plugin\.git"
```

## Passo 2 — Inicializar git, commitar e criar repo

Abre o terminal (PowerShell ou Git Bash) na pasta do plugin:

```bash
cd "C:\Users\Kevin\Documents\Obsidian Vault\Formacao-Branding-Visual-com-IA\formacao-brand-visual-ia-plugin"

# Inicializar repo
git init -b main
git config user.email "kevin.chen1913@gmail.com"
git config user.name "Kevin Chen"

# Adicionar tudo e commitar
git add .
git commit -m "chore: initial plugin structure + Onda 1 (5 skills transversais)

- Plugin manifest, README, LICENSE, CHANGELOG
- 5 skills transversais atualizadas:
  - maestro (38 skills, voice-tone reordenada, sem ChatGPT)
  - diagnostico (Figma/CapCut/Higgsfield nas perguntas 13-15)
  - troubleshooting (6 categorias, CapCut nos fixes)
  - fechamento (Blocos 0-4, sem M0-M08 MEC)
  - brand-vocabulary -> stub de redirecionamento"
```

## Passo 3 — Criar repo privado no GitHub

### Opção A — Via interface web (mais simples)

1. Vai em https://github.com/new
2. **Repository name:** `formacao-brand-visual-ia-plugin`
3. **Description:** `Plugin oficial da Formação Branding Visual com IA — 38 skills`
4. **Visibility:** Private ✅
5. **NÃO** marca "Add a README", "Add .gitignore", "Choose a license" (já tem todos)
6. Clica **Create repository**

Na próxima tela, GitHub mostra os comandos pra conectar. Roda esses dois no terminal:

```bash
git remote add origin https://github.com/kevinchen-copy/formacao-brand-visual-ia-plugin.git
git push -u origin main
```

### Opção B — Via gh CLI (se tiver instalado)

```bash
gh repo create formacao-brand-visual-ia-plugin --private --source=. --remote=origin --push
```

## Passo 4 — Confirmar

Acessa https://github.com/kevinchen-copy/formacao-brand-visual-ia-plugin

Deve ver:
- `.claude-plugin/plugin.json`
- `README.md`
- `LICENSE`
- `CHANGELOG.md`
- `.gitignore`
- `skills/` com 5 subpastas (maestro, diagnostico, troubleshooting, fechamento, brand-vocabulary)

## Passo 5 — Me avisa

Cola aqui no chat:
- ✅ Repo criado: link do GitHub
- ✅ Push funcionou

E aí a gente arranca a **Onda 2** (Bloco 0/1/2 — 8 skills estratégicas alinhadas com M01 do curso).

## Próximas Ondas — preview

A cada onda, eu:
1. Escrevo as skills no plugin local
2. Tu roda no terminal:
```bash
cd "C:\Users\Kevin\Documents\Obsidian Vault\Formacao-Branding-Visual-com-IA\formacao-brand-visual-ia-plugin"
git add .
git commit -m "<descrição da onda>"
git push
```
3. Tu instala/atualiza o plugin no Cowork pra ver as mudanças

## Bônus — Instalar plugin pra testar

Depois do push, instala o plugin no Cowork:

```bash
# No Claude Code:
claude plugin marketplace add kevinchen-copy/formacao-brand-visual-ia-plugin
claude plugin install formacao-brand-visual-ia
```

Ou no Cowork desktop: Customize → Habilidades → Add Marketplace → cola URL do repo.

---

**Esse arquivo pode ser deletado depois do primeiro push, ou movido pra `docs/` pra referência futura.**
