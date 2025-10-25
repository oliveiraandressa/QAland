[⬅Voltar](../../readme.md)  

# 🧭 Guia de Estratégia de Teste  

Este guia define **como planejar e direcionar os testes** de forma eficiente, garantindo que o esforço de QA traga o máximo de valor ao projeto.

---

## 🎯 Objetivo
Descrever **a abordagem, critérios e prioridades** usadas na execução dos testes, considerando o escopo, riscos e recursos disponíveis.

---

## 🧩 Tipos de Estratégia

| Estratégia | Descrição | Quando Usar |
|-------------|------------|--------------|
| **Baseada em Risco** ⚠️ | Priorização de testes conforme a probabilidade e impacto de falhas. | Quando o prazo é curto e é preciso testar o essencial primeiro. |
| **Baseada em Requisitos** 📋 | Cada requisito funcional é validado por casos de teste específicos. | Quando há documentação clara e completa do sistema. |
| **Exploratória** 🧠 | Testes manuais guiados pela experiência e comportamento do sistema. | Quando o produto está em evolução constante ou sem documentação. |
| **Automatizada** ⚙️ | Scripts executam testes repetitivos de forma contínua. | Quando há necessidade de regressão frequente ou CI/CD. |
| **Baseada em Dados** 🧮 | Variações de entradas são testadas para validar o comportamento do sistema. | Quando o sistema depende fortemente de regras de negócio e dados. |

---

## 🪜 Níveis de Teste
Defina os níveis que serão aplicados no projeto:

- **Unitário** – valida funções e componentes isolados  
- **Integração** – verifica comunicação entre módulos  
- **Sistema (E2E)** – garante que o sistema funcione como um todo  
- **Aceitação (UAT)** – valida o produto com o cliente ou usuário final  
- **Smoke/Sanity** – confirma se o sistema está estável para testes mais profundos  

---

## ⚡ Critérios de Priorização
Usados para decidir **o que testar primeiro**:

- 🔺 Alta prioridade: funcionalidades críticas e fluxos principais  
- 🔸 Média prioridade: recursos importantes, mas com baixo risco de impacto  
- 🔹 Baixa prioridade: itens estéticos ou pouco usados  

---

## 🧮 Critérios de Saída (Exit Criteria)
Define quando os testes podem ser **considerados concluídos**:

- Cobertura mínima de testes atingida (ex: 90%)  
- Nenhum bug crítico aberto  
- Todos os casos de alta prioridade executados  
- Ambiente estável e pronto para entrega  

---

## 🧱 Riscos e Mitigações
| Risco                     | Impacto | Estratégia de Mitigação                               |
|---------------------------|---------|------------------------------------------------------|
| Prazos curtos             | Alto    | Priorização baseada em risco e smoke tests           |
| Mudanças constantes no código | Médio  | Automação de regressão e testes parciais            |
| Falta de documentação     | Médio   | Abordagem exploratória e entrevistas com devs       |
| Dependência de APIs externas | Alto  | Mock de serviços e testes de fallback               |

---

## 🧰 Ferramentas e Abordagem Técnica
- **Testes manuais:** [Checklist, Exploratório, TestRail, Excel etc.]  
- **Automação:** [Cypress, Playwright, Jest, Postman etc.]  
- **Gestão de bugs:** [Jira, Trello, Notion etc.]  
- **Integração contínua:** [GitHub Actions, Jenkins etc.]  

---

## 📊 Acompanhamento e Relatórios
Os resultados devem ser consolidados em relatórios periódicos contendo:
- Casos executados x casos planejados  
- Percentual de sucesso  
- Bugs por severidade  
- Status geral de qualidade  

---

## 🧠 Recomendações Finais
- Sempre alinhar as expectativas do teste com o time de desenvolvimento.  
- Focar em **testar o que gera mais valor ao usuário final**.  
- Revisar a estratégia a cada release — ela deve evoluir junto com o produto.  

---

[⬅Voltar](../../readme.md)  