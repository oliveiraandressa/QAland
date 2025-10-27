---
layout: content
title: ''
hide_title: true
---

# 📝 Checklist - QA

Este guia serve como referência prática para novos analistas de QA acompanharem todas as **etapas do processo de teste** — desde o planejamento até o encerramento. Cada seção traz **descrições claras**, **objetivos** e **checklists detalhados** para garantir qualidade, rastreabilidade e padronização.

---

## 🧭 **1. Antes de Iniciar os Testes**
**Objetivo:** confirmar que todo o ambiente, documentação e escopo estão prontos para iniciar as atividades.

**Checklist:**
- [ ] Compreender o escopo e os objetivos do projeto (quais módulos e funcionalidades serão testados)  
- [ ] Ler e validar os requisitos funcionais e não funcionais  
- [ ] Confirmar que o ambiente de testes está disponível e atualizado  
- [ ] Garantir que o versionamento de código e build estejam corretos  
- [ ] Solicitar acesso a ferramentas, bancos de dados e credenciais  
- [ ] Definir quais tipos de testes serão aplicados (funcional, regressão, performance etc.)  
- [ ] Alinhar prazos, prioridades e entregas com o time de QA e desenvolvimento  

---

## 🗂️ **2. Ao Criar o Plano de Teste**
**Objetivo:** documentar como os testes serão conduzidos, quem será responsável e quais critérios definem sucesso.

**Checklist:**
- [ ] Definir o escopo dos testes e o que está **fora** do escopo  
- [ ] Descrever o ambiente de teste (hardware, software, navegador, versão, rede)  
- [ ] Determinar **critérios de entrada e saída** (quando iniciar e quando encerrar)  
- [ ] Selecionar ferramentas de execução e automação  
- [ ] Estabelecer responsabilidades da equipe (QA, dev, PO)  
- [ ] Definir riscos conhecidos e planos de mitigação  
- [ ] Documentar a estratégia de regressão e automação  

---

## 🧠 **3. Ao Definir Cenários de Teste**
**Objetivo:** transformar os requisitos em **situações práticas** que validem o comportamento do sistema.

**Checklist:**
- [ ] Mapear cada requisito a pelo menos um cenário de teste  
- [ ] Criar cenários que representem o **uso real do usuário**  
- [ ] Incluir cenários **positivos, negativos e alternativos**  
- [ ] Validar os cenários com o time de produto e desenvolvimento  
- [ ] Escrever de forma clara e objetiva (ex.: Dado / Quando / Então)  

---

## 🧾 **4. Ao Criar Casos de Teste**
**Objetivo:** detalhar os passos, dados e resultados esperados para execução manual ou automatizada.

**Checklist:**
- [ ] Criar **IDs únicos** e padronizados (ex.: CT-001, CT-002)  
- [ ] Incluir **pré-condições** e **pós-condições**  
- [ ] Especificar **dados de teste** necessários  
- [ ] Descrever **passos claros e reproduzíveis**  
- [ ] Definir **resultado esperado** para cada caso  
- [ ] Revisar cobertura completa dos requisitos  
- [ ] Validar com outro QA ou revisor técnico  

---

## ⚙️ **5. Execução dos Testes**
**Objetivo:** validar o sistema conforme os casos criados, registrando os resultados e eventuais falhas.

**Checklist:**
- [ ] Executar casos conforme o plano de teste  
- [ ] Registrar o **resultado obtido** (Passou / Falhou)  
- [ ] Coletar evidências: prints, logs ou gravações  
- [ ] Reportar bugs no sistema de rastreamento (com ID, descrição e passos)  
- [ ] Reexecutar após correções (testes de revalidação)  
- [ ] Atualizar status e métricas de execução  

---

## 🔹 **6. Funcionalidades Principais**
**Objetivo:** verificar se as funções centrais do sistema operam corretamente. Ex:

**Checklist:**
- [ ] Login e autenticação de usuário  
- [ ] Logout funcional  
- [ ] Cadastro e atualização de dados de usuário  
- [ ] Recuperação de senha  
- [ ] Dashboard / Tela inicial carregando corretamente  
- [ ] Upload e download de arquivos  
- [ ] Visualização e edição de informações  
- [ ] Exclusão de dados com confirmação  
- [ ] Notificações e alertas funcionando  

---

## 🔗 **7. Testes de Integração**
**Objetivo:** validar a comunicação entre módulos e serviços conectados.

**Checklist:**
- [ ] Comunicação entre front-end e back-end  
- [ ] Endpoints da API retornando status corretos  
- [ ] Dados salvos corretamente no banco  
- [ ] Integração com serviços externos (pagamento, autenticação etc.)  
- [ ] Tratamento de erros em chamadas externas  

---

## 🖱️ **8. Testes de Usabilidade**
**Objetivo:** garantir que o sistema seja intuitivo e fácil de usar.

**Checklist:**
- [ ] Navegação fluida entre telas  
- [ ] Botões e links acessíveis e funcionais  
- [ ] Mensagens de erro claras e informativas  
- [ ] Feedbacks visuais (loaders, alertas, validações)  
- [ ] Responsividade em diferentes resoluções e dispositivos  

---

## 🔐 **9. Testes de Segurança**
**Objetivo:** assegurar proteção contra acessos indevidos e vazamento de dados.

**Checklist:**
- [ ] Validação de credenciais no login  
- [ ] Controle de permissões por perfil  
- [ ] Testes de injeção (SQL, XSS)  
- [ ] Armazenamento seguro de senhas e tokens  
- [ ] Encriptação e HTTPS ativos  

---

## ⚡ **10. Testes de Performance**
**Objetivo:** medir velocidade, estabilidade e resposta sob diferentes cargas.

**Checklist:**
- [ ] Tempo de carregamento abaixo do esperado  
- [ ] Resposta da API sob volume alto de requisições  
- [ ] Teste de stress e endurance  
- [ ] Avaliação de gargalos (CPU, memória, rede)  

---

## ♻️ **11. Testes de Regressão**
**Objetivo:** confirmar que novas alterações não quebraram funcionalidades já existentes.

**Checklist:**
- [ ] Reteste de bugs corrigidos  
- [ ] Execução dos fluxos principais após deploy  
- [ ] Validação de integrações após atualizações  
- [ ] Automação de casos recorrentes  

---

## 🧮 **12. Após a Execução dos Testes**
**Objetivo:** consolidar resultados, gerar métricas e encerrar o ciclo.

**Checklist:**
- [ ] Atualizar status dos casos (Passou / Falhou / Bloqueado)  
- [ ] Registrar bugs com evidências anexadas  
- [ ] Validar correções com novo ciclo de testes  
- [ ] Calcular métricas de sucesso e cobertura  
- [ ] Elaborar relatório final de testes  

---

## 📊 **13. Métricas de Qualidade (Opcional)**
**Objetivo:** medir eficiência e cobertura dos testes.

| Métrica                        | Descrição |
|--------------------------------|------------|
| **Casos de Teste Criados**     | Total de casos documentados |
| **Casos Executados**           | Quantidade testada até o momento |
| **Percentual de Sucesso (%)**  | Relação entre casos aprovados e executados |
| **Cobertura de Requisitos (%)**| Quantos requisitos foram testados |
| **Defeitos Abertos / Corrigidos** | Acompanhamento da resolução |

---

📅 **Versão:** 1.0  
👤 **Responsável pela verificação:** {preencher}  
🧱 **Última atualização:** {data}

---


## Template em markdown

```md
# 🧩 **Checklist - QA**

## 🧭 **1. Antes de Iniciar os Testes**
**Objetivo:** confirmar que todo o ambiente, documentação e escopo estão prontos para iniciar as atividades.

**Checklist:**
- [ ] Compreender o escopo e os objetivos do projeto (quais módulos e funcionalidades serão testados)  
- [ ] Ler e validar os requisitos funcionais e não funcionais  
- [ ] Confirmar que o ambiente de testes está disponível e atualizado  
- [ ] Garantir que o versionamento de código e build estejam corretos  
- [ ] Solicitar acesso a ferramentas, bancos de dados e credenciais  
- [ ] Definir quais tipos de testes serão aplicados (funcional, regressão, performance etc.)  
- [ ] Alinhar prazos, prioridades e entregas com o time de QA e desenvolvimento  

---

## 🗂️ **2. Ao Criar o Plano de Teste**
**Objetivo:** documentar como os testes serão conduzidos, quem será responsável e quais critérios definem sucesso.

**Checklist:**
- [ ] Definir o escopo dos testes e o que está **fora** do escopo  
- [ ] Descrever o ambiente de teste (hardware, software, navegador, versão, rede)  
- [ ] Determinar **critérios de entrada e saída** (quando iniciar e quando encerrar)  
- [ ] Selecionar ferramentas de execução e automação  
- [ ] Estabelecer responsabilidades da equipe (QA, dev, PO)  
- [ ] Definir riscos conhecidos e planos de mitigação  
- [ ] Documentar a estratégia de regressão e automação  

---

## 🧠 **3. Ao Definir Cenários de Teste**
**Objetivo:** transformar os requisitos em **situações práticas** que validem o comportamento do sistema.

**Checklist:**
- [ ] Mapear cada requisito a pelo menos um cenário de teste  
- [ ] Criar cenários que representem o **uso real do usuário**  
- [ ] Incluir cenários **positivos, negativos e alternativos**  
- [ ] Validar os cenários com o time de produto e desenvolvimento  
- [ ] Escrever de forma clara e objetiva (ex.: Dado / Quando / Então)  

---

## 🧾 **4. Ao Criar Casos de Teste**
**Objetivo:** detalhar os passos, dados e resultados esperados para execução manual ou automatizada.

**Checklist:**
- [ ] Criar **IDs únicos** e padronizados (ex.: CT-001, CT-002)  
- [ ] Incluir **pré-condições** e **pós-condições**  
- [ ] Especificar **dados de teste** necessários  
- [ ] Descrever **passos claros e reproduzíveis**  
- [ ] Definir **resultado esperado** para cada caso  
- [ ] Revisar cobertura completa dos requisitos  
- [ ] Validar com outro QA ou revisor técnico  

---

## ⚙️ **5. Execução dos Testes**
**Objetivo:** validar o sistema conforme os casos criados, registrando os resultados e eventuais falhas.

**Checklist:**
- [ ] Executar casos conforme o plano de teste  
- [ ] Registrar o **resultado obtido** (Passou / Falhou)  
- [ ] Coletar evidências: prints, logs ou gravações  
- [ ] Reportar bugs no sistema de rastreamento (com ID, descrição e passos)  
- [ ] Reexecutar após correções (testes de revalidação)  
- [ ] Atualizar status e métricas de execução  

---

## 🔹 **6. Funcionalidades Principais**
**Objetivo:** verificar se as funções centrais do sistema operam corretamente.

**Checklist:**
- [ ] Login e autenticação de usuário  
- [ ] Logout funcional  
- [ ] Cadastro e atualização de dados de usuário  
- [ ] Recuperação de senha  
- [ ] Dashboard / Tela inicial carregando corretamente  
- [ ] Upload e download de arquivos  
- [ ] Visualização e edição de informações  
- [ ] Exclusão de dados com confirmação  
- [ ] Notificações e alertas funcionando  

---

## 🔗 **7. Testes de Integração**
**Objetivo:** validar a comunicação entre módulos e serviços conectados.

**Checklist:**
- [ ] Comunicação entre front-end e back-end  
- [ ] Endpoints da API retornando status corretos  
- [ ] Dados salvos corretamente no banco  
- [ ] Integração com serviços externos (pagamento, autenticação etc.)  
- [ ] Tratamento de erros em chamadas externas  

---

## 🖱️ **8. Testes de Usabilidade**
**Objetivo:** garantir que o sistema seja intuitivo e fácil de usar.

**Checklist:**
- [ ] Navegação fluida entre telas  
- [ ] Botões e links acessíveis e funcionais  
- [ ] Mensagens de erro claras e informativas  
- [ ] Feedbacks visuais (loaders, alertas, validações)  
- [ ] Responsividade em diferentes resoluções e dispositivos  

---

## 🔐 **9. Testes de Segurança**
**Objetivo:** assegurar proteção contra acessos indevidos e vazamento de dados.

**Checklist:**
- [ ] Validação de credenciais no login  
- [ ] Controle de permissões por perfil  
- [ ] Testes de injeção (SQL, XSS)  
- [ ] Armazenamento seguro de senhas e tokens  
- [ ] Encriptação e HTTPS ativos  

---

## ⚡ **10. Testes de Performance**
**Objetivo:** medir velocidade, estabilidade e resposta sob diferentes cargas.

**Checklist:**
- [ ] Tempo de carregamento abaixo do esperado  
- [ ] Resposta da API sob volume alto de requisições  
- [ ] Teste de stress e endurance  
- [ ] Avaliação de gargalos (CPU, memória, rede)  

---

## ♻️ **11. Testes de Regressão**
**Objetivo:** confirmar que novas alterações não quebraram funcionalidades já existentes.

**Checklist:**
- [ ] Reteste de bugs corrigidos  
- [ ] Execução dos fluxos principais após deploy  
- [ ] Validação de integrações após atualizações  
- [ ] Automação de casos recorrentes  

---

## 🧮 **12. Após a Execução dos Testes**
**Objetivo:** consolidar resultados, gerar métricas e encerrar o ciclo.

**Checklist:**
- [ ] Atualizar status dos casos (Passou / Falhou / Bloqueado)  
- [ ] Registrar bugs com evidências anexadas  
- [ ] Validar correções com novo ciclo de testes  
- [ ] Calcular métricas de sucesso e cobertura  
- [ ] Elaborar relatório final de testes  

---

## 📊 **13. Métricas de Qualidade (Opcional)**
**Objetivo:** medir eficiência e cobertura dos testes.

| Métrica                        | Descrição |
|--------------------------------|------------|
| **Casos de Teste Criados**     | Total de casos documentados |
| **Casos Executados**           | Quantidade testada até o momento |
| **Percentual de Sucesso (%)**  | Relação entre casos aprovados e executados |
| **Cobertura de Requisitos (%)**| Quantos requisitos foram testados |
| **Defeitos Abertos / Corrigidos** | Acompanhamento da resolução |

---

📅 **Versão:** 1.0  
👤 **Responsável pela verificação:** {preencher}  
🧱 **Última atualização:** {data}

---

```