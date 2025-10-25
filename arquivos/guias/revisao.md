---
layout: default
title: ''
hide_title: true
---

[  <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg">
    <path d="M15 18l-6-6 6-6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  </svg>Voltar](../../readme.md)  

# 🧠 Guia de Revisão e Validação de Testes  

Este guia estabelece **como revisar, validar e aprovar artefatos de teste** (planos, casos, execuções e resultados), garantindo qualidade e consistência em todo o processo de QA.

---

## 🎯 Objetivo  
Garantir que todos os artefatos de teste estejam **claros, completos e rastreáveis**, e que os resultados obtidos reflitam com precisão a **qualidade real do sistema** antes da liberação.

---

## 🧩 Etapas da Revisão de Teste  

### 1️⃣ **Revisão do Plano de Teste**
Verifica se o plano cobre o escopo e define critérios de sucesso adequados.

**Checklist:**
- [ ] Escopo claramente definido  
- [ ] Critérios de entrada e saída documentados  
- [ ] Tipos e níveis de teste especificados  
- [ ] Ambiente e ferramentas descritos  
- [ ] Responsabilidades atribuídas  
- [ ] Cronograma de testes definido  

---

### 2️⃣ **Revisão dos Casos de Teste**
Avalia se os casos estão bem escritos, compreensíveis e cobrindo todas as funcionalidades críticas.

**Checklist:**
- [ ] ID único e padronizado  
- [ ] Título descritivo e objetivo  
- [ ] Pré-condições definidas  
- [ ] Passos claros e sequenciais  
- [ ] Resultados esperados bem descritos  
- [ ] Critérios de aceitação alinhados  
- [ ] Status inicial (“Aguardando execução”)  

---

### 3️⃣ **Revisão de Execução**
Confere se a execução foi conduzida corretamente e com evidências suficientes.

**Checklist:**
- [ ] Evidências anexadas (prints, logs, vídeos)  
- [ ] Resultados registrados com clareza  
- [ ] Desvios documentados  
- [ ] Casos bloqueados ou não executados justificados  
- [ ] Reexecuções registradas (quando aplicável)  

---

### 4️⃣ **Validação de Resultados**
Confirma se o comportamento do sistema após correções é o esperado e se o produto está pronto para release.

**Checklist:**
- [ ] Todos os bugs críticos e altos resolvidos  
- [ ] Casos de teste falhos reexecutados  
- [ ] Critérios de saída atingidos  
- [ ] Testes de regressão concluídos  
- [ ] Aprovação formal registrada (via ferramenta ou documento)  

---

## ⚙️ Responsabilidades  

| Papel | Responsabilidade |
|-------|-------------------|
| **QA** | Criar e revisar casos de teste; executar e validar resultados |
| **Revisor QA Sênior / Líder** | Garantir qualidade dos artefatos e rastreabilidade |
| **Dev** | Corrigir defeitos identificados e apoiar revalidação |
| **Gerente / PO** | Aprovar entrega após validação de QA |

---

## 🧮 Exemplo de Fluxo de Validação  

1. QA executa os testes.  
2. Bugs são registrados e atribuídos ao Dev.  
3. Após correção, QA revalida os casos afetados.  
4. Revisor QA confirma evidências e resultados.  
5. QA Líder ou PO aprova a liberação.  


[  <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true" focusable="false" xmlns="http://www.w3.org/2000/svg">
    <path d="M15 18l-6-6 6-6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
  </svg>Voltar](../../readme.md)  