# 🤖 Plano de Teste 

## 📘 Informações Gerais
- **Projeto:**  {preencher}
- **Responsável:**  {preencher}
- **Data de Criação:**  {preencher}
- **Versão:**  1.0

---

## 🎯 Objetivo
Definir a estratégia e os critérios de testes, garantindo a cobertura funcional e a estabilidade dos fluxos críticos do sistema.

---

## 📦 Resumo do Projeto
{preencher}
---

## ⚙️ Ambiente de Execução

| Item | Descrição |
|------|------------|
| Ambiente | homologação |
| URL / Endpoint | {preencher} |
| Sistema Operacional | Windows |
| Navegador  | Chrome |

---

## 🔗 Dependências e Pré-Requisitos
- Não possui

---

## 🧩 Tipos de Teste
- [x] Testes Funcionais (E2E)  
- [ ] Testes de Regressão  
- [x] Testes de Integração

---

## 🧠 Critérios de Aceite
- Todos os testes devem passar em **100% das execuções**.  
- Falhas intermitentes devem ser investigadas e marcadas como *instáveis* até correção.  
- O sistema deve estar de acordo com o protótipo do [Figma](https://www.figma.com/{preencher})

---

## 📋 Casos de Teste


### 💡 Cenário: Login de usuário 
**Dado que** o usuario deseja fazer login **quando** insere suas informações corretamente e clica em login  **então** o sistema permite o acesso

**Passos:**
1. Insere email e senha válidos
2. Clica em 'login'

**Resultado esperado:** <br>
Redireciona para o dashboard

**Status** <br>
✅ Passou ou ⛔ Falhou 

---

## 🧾 Registro de Defeitos

| ID      | Descrição                                     | Severidade | Status     | Responsável | Data       |
| ------- | --------------------------------------------- | ---------- | ---------- | ----------- | ---------- |
| BUG-001 | Teste de login falha por timeout intermitente | Média      | Em análise | QA Team     | 16/10/2025 |
| BUG-002 | Endpoint de produtos retornando 500           | Alta       | Corrigido  | Dev Team    | 17/10/2025 |

---

## 🧮 Métricas de QA

| Métrica                      | Valor  |
| ---------------------------- | ------ |
| Total de Casos de Teste      | 15     |
| Casos Testados               | 15     |
| Casos Aprovados              | 13     |
| Casos Reprovados             | 2      |
| Taxa de Sucesso              | 85%    |

---
## 🧩 Considerações Finais

Produto reprovado após testes blablabla
