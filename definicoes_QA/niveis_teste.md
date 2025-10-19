# Níveis de Teste (Quando Testar?)

### **1. Teste de Unidade**
**Definição:** Verifica se partes pequenas do código (funções, métodos) funcionam isoladamente.  
**Quando aplicar:** Logo após desenvolver cada componente. Em caso de [BDD](bdd.md), o teste é desesnvolvido antes do código em si. 
**Importância:** Detecta erros cedo e reduz custo de correção.  
**Técnicas:** Testes automatizados com [Jest](ferramentas.md#jest), [JUnit](ferramentas.md#junit), [pytest](ferramentas.md#pytest); uso de [*mocks*](glossario.md#mock) e [*stubs*](glossario.md#stub).  
**Observações:**  
- Não testa integração nem comportamento do usuário.  
- Deve rodar rápido e ser altamente automatizado.  
- Evite testar dependências externas (isso é integração).  

---

### **2. Teste de Integração**
**Definição:** Avalia se diferentes módulos do sistema funcionam corretamente juntos.  
**Quando aplicar:** Após os testes de unidade e a integração dos módulos.  
**Importância:** Garante que as partes se comuniquem de forma correta.  
**Técnicas:** Testes de [API](glossario.md#api), banco de dados, [integração contínua (CI)](integracao_continua.md).  
**Observações:**  
- Foco é a comunicação entre módulos.  
- Use [*mocks*](glossario.md#mock) apenas para partes externas.  
- Não confundir com teste de sistema — aqui o foco ainda não é o produto completo.  

---

### **3. Teste de Sistema**
**Definição:** Testa o sistema completo, simulando uso real.  
**Quando aplicar:** Após a integração total.  
**Importância:** Assegura que o produto final funcione conforme o esperado.  
**Técnicas:** Testes funcionais, de [UI](glossario.md#ui), de desempenho e segurança.  
**Observações:**  
- É o primeiro teste do sistema como um todo.  
- Envolve testes de ponta a ponta (E2E).  
- Valide o ambiente completo, com dados e configurações reais.  

---

### **4. Teste de Aceitação**
**Definição:** Confirma se o sistema atende aos requisitos e critérios de aceite do cliente.  
**Quando aplicar:** Antes da entrega ou homologação.  
**Importância:** Garante que o produto entregue cumpre o que foi solicitado.  
**Técnicas:** Testes baseados em [histórias de usuário](glossario.md#história-de-usuário-us), [BDD (Gherkin)](bdd.md).  
**Observações:**  
- Guiado por critérios de aceite definidos previamente.  
- Pode envolver o cliente ou [Product Owner](scrum.md#product-owner).  
- Diferente do teste exploratório — o foco é validar requisitos.  

---

### **5. Teste Alfa**
**Definição:** Executado internamente antes do lançamento público.  
**Quando aplicar:** Na fase final de desenvolvimento.  
**Importância:** Detecta falhas em um ambiente controlado.  
**Técnicas:** Testes exploratórios, simulações de uso real.  
**Observações:**  
- Feito por times internos.  
- Avalia experiência e comportamento, não código.  

---

### **6. Teste Beta**
**Definição:** Executado por usuários reais antes do lançamento oficial.  
**Quando aplicar:** Após o teste alfa, em ambiente real.  
**Importância:** Coleta feedback de uso e detecta falhas do mundo real.  
**Técnicas:** Monitoramento de uso, formulários de feedback, relatórios de bugs.  
**Observações:**  
- Primeira validação externa.  
- Analise métricas e feedbacks para priorizar ajustes.  

---

### **7. Teste de Regressão**
**Definição:** Reexecuta testes anteriores após mudanças no código.  
**Quando aplicar:** Após correções, novas features ou atualizações.  
**Importância:** Garante que nada quebrou com as alterações.  
**Técnicas:** Automação de testes, smoke e sanity tests.  
**Observações:**  
- É recorrente, não pontual.  
- Ideal automatizar para rodar em CI/CD.  
- Sempre revalide funcionalidades antigas.  

---