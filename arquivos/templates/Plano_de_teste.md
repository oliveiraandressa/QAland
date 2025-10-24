# 🤖 Plano de Teste

## 📘 Informações Gerais
- **Projeto:** Sistema de Gestão de Portfólio
- **Responsável:** Andressa Oliveira
- **Data de Criação:** 23/10/2025
- **Versão:** 1.0

---

## 🎯 Objetivo
Definir a estratégia, os tipos e critérios de testes, garantindo a **qualidade, cobertura funcional e estabilidade** dos fluxos críticos do sistema. Este plano serve como guia para a equipe de QA e permite rastreabilidade de defeitos e métricas de execução.

---

## 📦 Resumo do Projeto
Sistema de portfólio online, que permite ao usuário visualizar projetos, documentação e interagir com conteúdos estáticos. O sistema deve garantir login seguro, navegação intuitiva e consistência de dados.

---

## ⚙️ Ambiente de Execução

| Item              | Descrição                  |
|------------------|----------------------------|
| Ambiente          | Homologação                |
| URL / Endpoint    | {preencher}                |
| Sistema Operacional | Windows / Linux / MacOS  |
| Navegador         | Chrome, Firefox, Edge      |
| Ferramentas       | Selenium, Postman, Cypress |

---

## 🔗 Dependências e Pré-Requisitos
- Conta de usuário válida para testes de login  
- Acesso à base de dados de teste  
- Sistema já implantado no ambiente de homologação

---

## 🧩 Tipos de Teste
- [x] **Testes Funcionais (E2E)** – valida funcionalidades críticas  
- [x] **Testes de Integração** – valida integração entre módulos  
- [ ] **Testes de Regressão** – para validação de mudanças  
- [ ] **Testes de Performance** – tempo de resposta e carga  
- [ ] **Testes de Segurança** – valida vulnerabilidades  
- [ ] **Testes de Usabilidade** – valida experiência do usuário  

---

## 🧠 Critérios de Aceite
- Todos os testes críticos devem passar em **≥95% das execuções**.  
- Falhas intermitentes devem ser documentadas como *instáveis* até correção.  
- Sistema deve estar de acordo com os protótipos do [Figma](https://www.figma.com/{preencher}).  
- Defeitos de **alta severidade** bloqueiam release; média e baixa devem ser avaliadas pelo Product Owner.  

---

## 📋 Casos de Teste

### 💡 Cenário 1: Login de Usuário
**Pré-condições:** Usuário cadastrado no sistema

**Dado que** o usuário deseja fazer login  
**Quando** insere email e senha válidos e clica em login  
**Então** o sistema permite acesso ao dashboard

**Passos:**
1. Abrir página de login  
2. Inserir email válido: `teste@dominio.com`  
3. Inserir senha válida: `123456`  
4. Clicar em 'Login'

**Resultado esperado:**  
- Redireciona para o dashboard  
- Mensagem de boas-vindas exibida  

**Resultado obtido:** ✅ Passou / ⛔ Falhou  
**Observações:** ...

---

### 💡 Cenário 2: Cadastro de Projeto
**Pré-condições:** Usuário logado no sistema

**Dado que** o usuário deseja cadastrar um projeto  
**Quando** preenche todos os campos obrigatórios e clica em salvar  
**Então** o projeto é registrado e listado na página principal

**Passos:**
1. Navegar até a seção “Meus Projetos”  
2. Clicar em “Adicionar Projeto”  
3. Preencher título, descrição e categoria  
4. Clicar em “Salvar”

**Resultado esperado:**  
- Novo projeto aparece na lista  
- Mensagem de sucesso exibida  

**Resultado obtido:** ✅ Passou / ⛔ Falhou  
**Observações:** ...

---

### 💡 Cenário 3: Visualização de Documentação
**Pré-condições:** Usuário logado

**Dado que** o usuário deseja acessar a documentação  
**Quando** clica no link de um projeto  
**Então** a documentação completa é exibida corretamente

**Passos:**
1. Abrir página do projeto  
2. Clicar em “Documentação”  
3. Conferir conteúdo exibido

**Resultado esperado:**  
- Documentação correta e formatada  
- Todos os links internos funcionam  

**Resultado obtido:** ✅ Passou / ⛔ Falhou  
**Observações:** ...

---

## 🧾 Registro de Defeitos

| ID      | Descrição                                     | Tipo        | Severidade | Status     | Responsável | Data       |
| ------- | --------------------------------------------- | ----------- | ---------- | ---------- | ----------- | ---------- |
| BUG-001 | Login falha por timeout intermitente          | Funcional   | Média      | Em análise | QA Team     | 16/10/2025 |
| BUG-002 | Endpoint de produtos retorna 500              | Integração  | Alta       | Corrigido  | Dev Team    | 17/10/2025 |
| BUG-003 | Layout de dashboard quebrado no Firefox       | UI/Usabilidade | Baixa   | Em análise | QA Team     | 23/10/2025 |

---

## 🧮 Métricas de QA

| Métrica                      | Valor  |
| ---------------------------- | ------ |
| Total de Casos de Teste      | 15     |
| Casos Executados             | 15     |
| Casos Aprovados              | 13     |
| Casos Reprovados             | 2      |
| Taxa de Sucesso              | 87%    |
| Defeitos Abertos             | 2      |
| Defeitos Corrigidos          | 1      |

---

## 🧩 Considerações Finais
O produto apresentou **2 falhas críticas e 1 falha média**. Recomenda-se que as correções sejam realizadas antes do release.  
O sistema está parcialmente pronto para homologação, com funcionalidades principais operando conforme esperado.  

---

