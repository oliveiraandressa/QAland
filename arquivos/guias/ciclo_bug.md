---
layout: default
title: ''
hide_title: true
---

[  <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg">
    <path d="M15 18l-6-6 6-6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  </svg>Voltar](../../readme.md)  

# 🐞 Guia de Registro e Ciclo de Bug  

Este guia define **como identificar, registrar, acompanhar e encerrar defeitos (bugs)** de forma padronizada e eficiente.

---

## 🎯 Objetivo  
Garantir que todos os defeitos sejam **reportados de forma clara**, **priorizados corretamente** e **resolvidos com rastreabilidade completa**, fortalecendo a comunicação entre QA e desenvolvimento.

---

## 🧭 Ciclo de Vida do Bug  

1. **Novo** 🟢  
   - O bug é identificado e registrado no sistema de gestão.  

2. **Em Análise** 🔍  
   - O time de QA ou desenvolvimento revisa as informações e confirma a validade do bug.  

3. **Confirmado** 🧩  
   - O bug é aceito como válido e encaminhado para correção.  

4. **Em Correção** 🔧  
   - O desenvolvedor está trabalhando na solução do problema.  

5. **Corrigido** 🧠  
   - O bug foi resolvido e a correção está disponível em ambiente de teste.  

6. **Em Validação** 🧪  
   - O QA executa novamente o cenário para confirmar a correção.  

7. **Fechado** ✅  
   - O bug foi validado com sucesso.  

8. **Reaberto** 🔁  
   - O erro persiste após a correção e é devolvido ao time de desenvolvimento.  

---

## 🧩 Campos do Registro de Bug  

| Campo | Descrição | Exemplo |
|--------|------------|----------|
| **ID** | Identificador único | BUG-001 |
| **Título** | Breve descrição do problema | Erro ao fazer login com credenciais válidas |
| **Descrição Detalhada** | Explicação completa do defeito | O sistema retorna erro 500 ao autenticar usuário válido |
| **Passos para Reproduzir** | Sequência para reproduzir o bug | 1. Acessar /login <br> 2. Inserir credenciais válidas <br> 3. Clicar em "Entrar" |
| **Resultado Esperado** | O que deveria acontecer | Login realizado com sucesso |
| **Resultado Obtido** | O que ocorreu de fato | Erro 500 exibido |
| **Severidade** | Impacto técnico no sistema | Alta |
| **Prioridade** | Urgência para correção | Alta |
| **Ambiente** | Onde o bug foi detectado | Homologação |
| **Responsável** | Pessoa ou time designado | Dev Team |
| **Status** | Etapa atual do ciclo | Em correção |
| **Data de Registro** | Data de abertura | 20/10/2025 |

---

## 🧮 Classificação de Severidade  

| Nível | Descrição | Exemplo |
|-------|------------|----------|
| **Crítica** | Impede uso total do sistema | Página principal não carrega |
| **Alta** | Bloqueia fluxo principal | Login não funciona |
| **Média** | Impacta fluxo secundário | Botão de filtro não responde |
| **Baixa** | Erro visual ou de texto | Ícone desalinhado |

---

## ⚡ Classificação de Prioridade  

| Nível | Descrição | Exemplo |
|-------|------------|----------|
| **Alta** | Deve ser corrigido imediatamente | Bug crítico em produção |
| **Média** | Corrigir antes da próxima release | Erro funcional em ambiente de teste |
| **Baixa** | Pode aguardar próximas sprints | Ajuste estético |

---

## 📋 Boas Práticas  

- Registrar **prints, vídeos ou logs** para facilitar reprodução.  
- Descrever o bug **de forma objetiva e impessoal**.  
- Evitar duplicidades — **pesquise antes de criar um novo bug.**  
- Atualizar status sempre que o bug mudar de fase.  
- Validar a **causa raiz** em bugs recorrentes.  

---

## 🧠 Ferramentas Recomendadas  

| Categoria | Ferramentas |
|------------|-------------|
| **Gestão de Bugs** | Jira, Trello, Azure DevOps, ClickUp |
| **Captura de Evidências** | Loom, Lightshot, OBS |
| **Integração com CI/CD** | GitHub Issues, GitLab, Jenkins |

---

## 🧾 Exemplo de Registro  

**ID:** BUG-012  
**Título:** Página de checkout não atualiza o total após aplicar cupom  
**Descrição:** Valor total permanece igual mesmo após aplicar cupom de desconto válido  
**Passos:**  
1. Acessar /checkout  
2. Inserir cupom “PROMO10”  
3. Clicar em “Aplicar”  
**Resultado Esperado:** Total atualizado com 10% de desconto  
**Resultado Obtido:** Total permanece o mesmo  
**Severidade:** Média  
**Prioridade:** Alta  
**Status:** Confirmado  
**Responsável:** Dev Frontend  
**Data:** 22/10/2025  

---

## ✅ Conclusão  

Um bom controle de bugs garante **transparência, priorização eficaz e histórico de qualidade.**  
Mantenha o ciclo de vida bem definido e use métricas para acompanhar tendências (bugs reabertos, densidade, tempo médio de correção, etc.).

---

[  <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg">
    <path d="M15 18l-6-6 6-6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  </svg>Voltar](../../readme.md)  