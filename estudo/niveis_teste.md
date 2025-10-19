# Níveis de Teste (Quando Testar?)

## Teste unitário ou de unidade

Verifica se cada parte pequena **do código** (função, método) funciona sozinha.

**Quando aplicar?**   
Logo após desenvolver cada função ou módulo.
[No BDD](bdd.md), cria-se o teste de unidade antes do código em si.  


**Por que aplicar?**  
Detecta erros cedo, antes que se espalhem.  


**Técnicas envolvidas:**  
Uso de frameworks como Jest, JUnit, pytest; mocks e stubs para isolar partes do código. Geramente é feito pelo programador (nem sempre da forma correta).

**Importante lembrar:**  
Ele **não testa integração** nem comportamento de usuário, só a lógica interna de cada função.

**Dica:**  
Deve rodar **muito rápido** e ser **altamente automatizado**.

**Erro comum:**  
Tentar testar dependências externas (API, banco) — isso já é integração.

---

## Teste de integração
Checa se diferentes partes do sistema funcionam bem juntas.

**Quando aplicar?**  
Depois que várias partes do sistema estão prontas.

**Por que aplicar?**  
Garante que os módulos funcionam bem em conjunto.  

**Técnicas envolvidas:**  
Testes de API, testes de banco de dados, [integração contínua (CI)](integracao_continua.md).  

**Importante lembrar:**  
O foco é **como os módulos se comunicam** — exemplo: front e backend.

**Dica:**  
Costuma usar mocks parciais (só o que for externo demais).

**Erro comum:**  
Confundir com teste de sistema — aqui você ainda **não testa o produto completo**, só conexões.


---

## Teste de sistema
Valida o sistema completo, como se fosse o produto final.  

**Quando aplicar?** 
Após a integração completa.  

**Por que aplicar?**  
Valida o sistema como um todo, simulando uso real.  

**Técnicas envolvidas:**  
Testes funcionais, de interface (UI), de desempenho e segurança.  

**Importante lembrar:**  
É o primeiro momento em que se testa o sistema **como o usuário o verá**.

**Dica:**  
Envolve testes de ponta a ponta (E2E).

**Erro comum:**  
Deixar de validar o ambiente completo (ex: não usar o mesmo servidor, configs ou dados reais).

---

## Teste de aceitação
Confirma se o sistema atende às necessidades do cliente  

**Quando aplicar?**  
Antes da entrega ao cliente.  

**Por que aplicar?**  
Confirma se o sistema atende aos requisitos e expectativas do usuário.

**Técnicas envolvidas:**  
Testes baseados em cenários reais e critérios de aceite (ex: [Gherkin](gherkin.md), [BDD](bdd.md)).  

**Importante lembrar:**  
Ele é guiado por **critérios de aceite** (histórias de usuário).

**Dica:**  
Pode ser feito com o cliente ou com o [PO (Product Owner)](scrum.md#product-owner)

**Erro comum:**  
Confundir com testes exploratórios — aqui o objetivo é confirmar requisitos, não descobrir bugs novos.


---

## Teste alfa
Feito internamente pela equipe antes de liberar para o público.

**Quando aplicar?**  
Em fase final, dentro da empresa.

**Por que aplicar?**  
Encontrar falhas que escaparam dos testes anteriores.

**Técnicas envolvidas:**  
Testes exploratórios e simulação de uso real por equipe interna.  

**Importante lembrar:**  
É feito **antes** do lançamento público, mas **com o sistema completo**.

**Dica:**  
Geralmente realizado por times internos simulando uso real.

**Erro comum:**  
Achar que é um teste técnico — ele é **de experiência**, não de código.

---

## Teste beta
Feito por usuários reais para encontrar falhas antes do lançamento.

**Quando aplicar?**  
Logo antes do lançamento público

**Por que aplicar?**  
Coleta feedback de usuários reais e detecta falhas em ambientes reais.

**Técnicas envolvidas:**  
Monitoramento de uso, formulários de feedback, relatórios de bugs.  

**Importante lembrar:**  
É **a primeira validação real com usuários externos.**

**Dica:**  
Serve tanto pra feedback de usabilidade quanto pra identificar erros que não aparecem em ambiente controlado.

**Erro comum:**  
Não acompanhar métricas nem feedback — o teste perde valor se não for analisado.

---

## Teste de regressão
Garante que novas mudanças não quebraram o que já funcionava.  

**Quando aplicar?**  
Sempre que há mudança no código (nova versão, correção, feature).

**Por que aplicar?**  
Garante que nada quebrou com a atualização.

**Técnicas envolvidas:** 
Automação de testes, reexecução de casos antigos, testes de smoke/sanity.  

**Importante lembrar:**  
É **recorrente**, não um tipo isolado.

**Dica:**  
Ideal automatizar o máximo possível (ex: smoke tests automatizados).

**Erro comum:**  
Testar só a nova feature e esquecer de rodar o conjunto completo de testes antigos.

---
