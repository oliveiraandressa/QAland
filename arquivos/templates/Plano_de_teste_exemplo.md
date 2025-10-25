---
layout: default
title: ''
hide_title: true
---

[⬅Voltar](../../readme.md)  

# 🤖 Plano de Teste - Sistema de Portfólio Online

## 📘 Informações Gerais
- **Projeto:** Sistema de Portfólio Online  
- **Responsável:** Andressa Oliveira  
- **Data de Criação:** 23/10/2025  
- **Versão:** 1.0  

---

## 🎯 Objetivo
Garantir que o Sistema de Portfólio Online funcione corretamente, atendendo aos requisitos de login, cadastro de projetos e visualização de documentação. O plano define tipos e níveis de teste, critérios de aceitação e registro de métricas.

---

## 📦 Resumo do Projeto
O sistema permite que usuários criem, visualizem e compartilhem projetos em um portfólio online. Cada projeto pode conter descrição, imagens e documentação em PDF. O sistema possui login seguro e dashboard para gerenciamento de projetos.

---

## ⚙️ Ambiente de Execução

| Item              | Descrição                  |
|------------------|----------------------------|
| Ambiente          | Homologação                |
| URL / Endpoint    | https://portfolio.test.com |
| Sistema Operacional | Windows 10, MacOS        |
| Navegador         | Chrome, Firefox            |
| Ferramentas       | Selenium, Postman, Cypress |

---

## 🔗 Dependências e Pré-Requisitos
- Conta de usuário válida  
- Documentos de teste disponíveis (.pdf, imagens)  
- Sistema implantado no ambiente de homologação

---

## 🏗️ Níveis de Teste
- [x] Unitário – Testa funções ou módulos isolados  
- [x] Integração – Testa comunicação entre módulos  
- [x] Sistema / E2E – Testa fluxo completo do usuário  
- [ ] Aceitação – Confirma requisitos e estabilidade  

---

## 🧩 Tipos de Teste
- [x] Funcional – Valida funcionalidades críticas  
- [x] Regressão – Garante que mudanças não quebrem o sistema  
- [ ] Performance – Testa tempo de resposta e carga  
- [x] Segurança – Valida vulnerabilidades de login  
- [x] Usabilidade – Testa experiência do usuário  
- [x] Automatizado – Executado por scripts / ferramentas  
- [x] Manual – Executado manualmente por QA  

---

## 📋 Casos de Teste

### 💡 Cenário: Login de Usuário
**Pré-condições:** Usuário cadastrado no sistema

**Dado que** o usuário deseja fazer login  
**Quando** insere email `usuario@test.com` e senha `Senha123` e clica em login  
**Então** o sistema permite acesso ao dashboard

**Passos:**
1. Abrir página de login  
2. Inserir email válido  
3. Inserir senha válida  
4. Clicar em 'Login'

**Dados de teste:**  
- Email: usuario@test.com  
- Senha: Senha123

**Resultado esperado:**  
- Redireciona para dashboard  
- Mensagem de boas-vindas exibida  

**Status:** ✅ Passou  
**Observações:** Nenhuma

---

### 💡 Cenário: Cadastro de Projeto
**Pré-condições:** Usuário logado no sistema

**Dado que** o usuário deseja cadastrar um projeto  
**Quando** preenche todos os campos obrigatórios e clica em salvar  
**Então** o projeto é registrado e listado na página principal

**Passos:**
1. Navegar até “Meus Projetos”  
2. Clicar em “Adicionar Projeto”  
3. Preencher título, descrição e categoria  
4. Clicar em “Salvar”

**Dados de teste:**  
- Título: “Portfólio Front-End”  
- Descrição: “Exemplo de projetos de front-end”  
- Categoria: “Web”

**Resultado esperado:**  
- Novo projeto aparece na lista  
- Mensagem de sucesso exibida  

**Status:** ✅ Passou  
**Observações:** Nenhuma

---

### 💡 Cenário: Visualização de Documentação
**Pré-condições:** Usuário logado

**Dado que** o usuário deseja acessar a documentação  
**Quando** clica no link de um projeto  
**Então** a documentação completa é exibida corretamente

**Passos:**
1. Abrir página do projeto  
2. Clicar em “Documentação”  
3. Conferir conteúdo exibido

**Dados de teste:** PDF com documentação do projeto

**Resultado esperado:**  
- Documentação correta e formatada  
- Todos os links internos funcionam  

**Status:** ✅ Passou  
**Observações:** Nenhuma

---

## 🧾 Registro de Defeitos

| ID      | Descrição                                     | Tipo        | Severidade | Status     | Responsável | Data       |
| ------- | --------------------------------------------- | ----------- | ---------- | ---------- | ----------- | ---------- |
| BUG-001 | Login falha intermitente ao usar Firefox     | Funcional   | Média      | Em análise | QA Team     | 23/10/2025 |
| BUG-002 | Dashboard quebra layout em resolução 1366x768 | UI          | Baixa      | Corrigido  | QA Team     | 23/10/2025 |
| BUG-003 | Upload de PDF maior que 5MB não funciona     | Funcional   | Alta       | Aberto     | Dev Team    | 23/10/2025 |

---

## 🔥 Severidade / Prioridade de Defeitos
- [x] Baixa  
- [x] Média  
- [x] Alta  
- [ ] Crítica  

---

## 🧮 Métricas de QA

| Métrica                      | Valor |
|-------------------------------|-------|
| Total de Casos de Teste       | 15    |
| Casos Executados              | 15    |
| Casos Aprovados               | 13    |
| Casos Reprovados              | 2     |
| Taxa de Sucesso (%)           | 87%   |
| Defeitos Abertos              | 1     |
| Defeitos Corrigidos           | 1     |

---

## 📝 Considerações Finais
O sistema está **funcionando de forma estável** nos fluxos de login, cadastro e visualização de documentação.  
Defeitos críticos e altos devem ser corrigidos antes do release.  
Funcionalidades adicionais podem passar por testes de aceitação posteriormente.

---

## ✅ Checklist de Aprovação do Plano
- [x] Projeto preenchido  
- [x] Níveis de teste selecionados  
- [x] Tipos de teste selecionados  
- [x] Casos de teste prontos  
- [x] Métricas de QA incluídas  
- [x] Registro de defeitos revisado  
