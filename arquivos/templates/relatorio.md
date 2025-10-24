# 🧪 Relatório de Teste

**Projeto:** [Nome do Projeto]  
**Versão do Sistema:** [vX.X.X]  
**Data:** [DD/MM/AAAA]  
**Responsável:** [Nome do QA]  

---

## 1. Resumo do Teste
Breve descrição do objetivo do teste, escopo e tipo de teste realizado (Unitário, Integração, Sistema, Aceitação, Regressão, E2E etc.).

**Exemplo:**  
> Teste de regressão da funcionalidade de login para verificar se as alterações recentes não afetaram o fluxo de autenticação.

---

## 2. Ambiente de Teste
- **Sistema Operacional:** [Windows/Linux/macOS]  
- **Navegador/Versão:** [Chrome 120, Firefox 115 etc.]  
- **Base de Dados:** [MySQL/PostgreSQL/Outro]  
- **API/Serviços:** [Versão ou endpoint utilizado]  
- **Ferramentas de Teste:** [Cypress, Playwright, Jest etc.]

---

## 3. Casos de Teste Com Falha
| ID | Caso de Teste | Pré-condição | Passos | Resultado Esperado | Resultado Obtido | Status |
|----|---------------|--------------|--------|------------------|-----------------|--------|
| CT-001 | Login válido | Usuário cadastrado | 1. Acessar login <br> 2. Inserir credenciais <br> 3. Clicar Entrar | Acesso permitido | Acesso recusado | ⛔ Falhou  |
| CT-002 | Login inválido | Usuário cadastrado | 1. Acessar login <br> 2. Inserir senha errada <br> 3. Clicar Entrar | Mensagem de erro | Mensagem não foi exibida | ⛔ Falhou  |


> Você pode adicionar quantas linhas forem necessárias para todos os casos de teste.

---

## 4. Bugs Registrados
| ID | Caso de Teste | Severidade | Descrição | Status |
|----|---------------|------------|-----------|--------|
| BUG-001 | CT-001 | Alta | Login não funciona | Aberto |
| BUG-002 | CT-002 | Média | Mensagem de erro do login não é exibida | Corrigido |

---

## 5. Métricas do Teste
- **Total de Casos de Teste:** [X]  
- **Passaram:** [Y]  
- **Falharam:** [Z]  
- **Percentual de Sucesso:** [Y/X * 100%]  
- **Cobertura de Teste:** [XX%]  

---

## 6. Observações / Comentários
- Pontos importantes durante a execução dos testes  
- Recomendações para melhorias futuras  
- Análise de riscos ou comportamento inesperado  

---

## 7. Conclusão
Breve resumo do resultado geral, indicando se o teste foi satisfatório, quais áreas precisam de atenção e recomendações para a próxima rodada de testes.  

**Exemplo:**  
> A funcionalidade de login passou em 95% dos casos. Alguns bugs menores foram encontrados na recuperação de senha. Recomendamos correção antes do próximo deploy.
