---
layout: default
title: ''
hide_title: true
---

[⬅Voltar](../../readme.md)  

# 🧪 STLC - Guia Completo com Checklists

O **STLC (Software Testing Life Cycle)** é o conjunto de fases que estruturam o processo de teste de software, desde o planejamento até o encerramento.  
Cada fase tem entregas e objetivos claros — abaixo, um guia completo com **checklists práticos** para o dia a dia do QA.

---

## 🧭 1. Planejamento do Teste (Test Planning)

**Objetivo:** Definir a estratégia, escopo, cronograma e recursos de teste.  
É a base de todo o ciclo — define *como* o teste será feito.

### O que é feito:
- Analisar requisitos do projeto.
- Definir escopo (o que será e não será testado).
- Identificar riscos e dependências.
- Definir papéis e responsabilidades da equipe.
- Selecionar ferramentas e ambiente.
- Estimar tempo, custo e esforço.
- Criar e aprovar o **Plano de Teste**.

### ✅ Checklist:
- [ ] Requisitos analisados e compreendidos  
- [ ] Escopo definido (in/out)  
- [ ] Estratégia de teste documentada  
- [ ] Riscos e dependências identificados  
- [ ] Papéis e responsabilidades atribuídos  
- [ ] Ferramentas selecionadas  
- [ ] Cronograma e estimativas definidos  
- [ ] Plano de teste revisado e aprovado  

---

## 🔍 2. Análise do Teste (Test Analysis)

**Objetivo:** Identificar *o que* precisa ser testado e garantir que os requisitos sejam testáveis.

### O que é feito:
- Revisar requisitos funcionais e não funcionais.
- Identificar condições de teste com base em requisitos.
- Validar critérios de aceitação.
- Determinar tipos de teste necessários (funcional, integração, performance, etc).
- Iniciar matriz de rastreabilidade entre requisitos e condições de teste.

### ✅ Checklist:
- [ ] Requisitos revisados e validados  
- [ ] Condições de teste identificadas  
- [ ] Critérios de aceitação revisados  
- [ ] Tipos de teste definidos  
- [ ] Requisitos ambíguos reportados  
- [ ] Itens de rastreabilidade criados  

---

## 🧩 3. Design do Teste (Test Design)

**Objetivo:** Criar casos de teste detalhados, preparar dados de teste e garantir cobertura adequada.

### O que é feito:
- Escrever casos de teste (pré-condições, passos, dados, resultados esperados).  
- Aplicar técnicas de teste (valor limite, equivalência, decisão, etc).  
- Criar dados de teste válidos e inválidos.  
- Mapear requisitos → casos de teste (matriz de rastreabilidade).  
- Priorizar casos de teste (críticos, médios, baixos).  
- Planejar automação de testes (quando aplicável).

### ✅ Checklist:
- [ ] Casos de teste criados e revisados  
- [ ] Cobertura de requisitos verificada  
- [ ] Massa de dados preparada e documentada  
- [ ] Matriz de rastreabilidade atualizada  
- [ ] Casos priorizados (crítico, médio, baixo)  
- [ ] Scripts automatizados revisados (se houver)  

---

## 🧱 4. Configuração do Ambiente (Test Environment Setup)

**Objetivo:** Garantir que o ambiente de teste esteja funcional e estável antes da execução.

### O que é feito:
- Configurar servidores, bancos de dados, APIs e dependências.  
- Instalar o build ou versão a ser testada.  
- Configurar ferramentas de integração, logs e rastreamento.  
- Verificar compatibilidade de versões e acessos.  
- Executar **Smoke Test** para validar estabilidade inicial.

### ✅ Checklist:
- [ ] Ambiente configurado e acessível  
- [ ] Build correto instalado  
- [ ] Banco de dados e APIs configurados  
- [ ] Ferramentas integradas (Jira, Jenkins, etc)  
- [ ] Smoke test executado com sucesso  
- [ ] Acesso liberado para testadores  

---

## ▶️ 5. Execução do Teste (Test Execution)

**Objetivo:** Executar casos de teste, registrar resultados e reportar defeitos.

### O que é feito:
- Executar casos de teste (manuais e/ou automatizados).  
- Registrar status (Pass, Fail, Blocked, Not Executed).  
- Coletar evidências (prints, logs, vídeos).  
- Abrir bugs com detalhes e severidade.  
- Retestar após correções.  
- Executar testes de regressão.  
- Atualizar status e métricas no sistema de testes.

### ✅ Checklist:
- [ ] Casos de teste executados  
- [ ] Evidências coletadas e anexadas  
- [ ] Defeitos documentados e priorizados  
- [ ] Retestes realizados  
- [ ] Testes de regressão executados  
- [ ] Status atualizado no sistema  

---

## 📊 6. Encerramento do Teste (Test Closure)

**Objetivo:** Finalizar o ciclo, avaliar métricas e documentar resultados.

### O que é feito:
- Garantir que todos os requisitos foram cobertos.  
- Coletar e analisar métricas (defeitos, tempo, densidade, taxa de sucesso).  
- Criar relatório final de testes (resumo, status, bugs críticos, pendências).  
- Conduzir retrospectiva e lições aprendidas.  
- Arquivar evidências e documentos.  

### ✅ Checklist:
- [ ] Todos os testes planejados executados  
- [ ] Cobertura total dos requisitos validada  
- [ ] Defeitos críticos resolvidos ou aceitos  
- [ ] Relatório final entregue  
- [ ] Métricas coletadas e analisadas  
- [ ] Reunião de lições aprendidas realizada  
- [ ] Artefatos arquivados  

---

[⬅Voltar](../../readme.md)  