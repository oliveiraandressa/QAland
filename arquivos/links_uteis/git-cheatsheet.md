---
layout: default
title: ''
hide_title: true
---

[  <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg">
    <path d="M15 18l-6-6 6-6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  </svg>Voltar](../../readme.md)  

# 🧭 Git & Versionamento 

## 🔹 Comandos Básicos
```bash
git init                # Inicializa um repositório
git clone <url>         # Clona um repositório remoto
git status              # Mostra alterações
git add .               # Adiciona todas as alterações
git commit -m "msg"     # Cria um commit
git push                # Envia alterações
git pull                # Atualiza repositório local
```

## 🔹 Branches
```bash
git branch              # Lista branches
git checkout -b nome    # Cria e muda para nova branch
git switch nome         # Alterna de branch
git merge nome          # Mescla branch atual com outra
```

## 🔹 Commits Convencionais (Conventional Commits)
| Tipo | Uso |
|------|-----|
| feat | Nova funcionalidade |
| fix | Correção de bug |
| docs | Alterações em documentação |
| style | Formatação (sem impacto no código) |
| refactor | Refatoração de código |
| test | Adição ou ajuste de testes |
| chore | Tarefas gerais (build, deps etc.) |

📝 Exemplo:  
```bash
git commit -m "feat(login): add OAuth2 integration"
```

## 🔹 Versionamento Semântico (SemVer)
Formato: **MAJOR.MINOR.PATCH**
- **MAJOR** – Quebra de compatibilidade
- **MINOR** – Novas features compatíveis
- **PATCH** – Correções ou ajustes pequenos

Exemplo: `v2.4.1`

## 🔹 Estrutura de CHANGELOG
```markdown
# Changelog
## [1.1.0] - 2025-10-19
### Added
- Novo fluxo de login com OAuth2

### Fixed
- Bug na tela de reset de senha
```

[  <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg">
    <path d="M15 18l-6-6 6-6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  </svg>Voltar](../../readme.md)