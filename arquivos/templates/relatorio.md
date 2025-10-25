[⬅Voltar](../../readme.md)  

# 🧪 Template de Relatório de Teste

**Projeto:** {preencher}  
**Versão do Sistema:** {vX.X.X}  
**Data:** {DD/MM/AAAA}  
**Responsável:** {preencher}  

---

## 1. Resumo do Teste
Breve descrição do objetivo, escopo e tipo de teste realizado.  

**Exemplo:**  
> Teste de regressão da funcionalidade de login para verificar se alterações recentes não afetaram o fluxo de autenticação.

---

## 2. Níveis e Tipos de Teste (Checklist)

**Níveis de Teste:**  
- [ ] Unitário  
- [ ] Integração  
- [ ] Sistema / E2E  
- [ ] Aceitação  

**Tipos de Teste:**  
- [ ] Funcional  
- [ ] Regressão  
- [ ] Performance  
- [ ] Segurança  
- [ ] Usabilidade  
- [ ] Automatizado  
- [ ] Manual  

---

## 3. Ambiente de Teste
- **Sistema Operacional:** {Windows/Linux/macOS}  
- **Navegador / Versão:** {Chrome, Firefox, Edge etc.}  
- **Base de Dados:** {MySQL, PostgreSQL, Outro}  
- **API / Serviços:** {Versão ou endpoint}  
- **Ferramentas de Teste:** {Cypress, Playwright, Jest etc.}  

---

## 4. Casos de Teste com Falha

| ID | Caso de Teste | Pré-condição | Passos | Resultado Esperado | Resultado Obtido | Status | Responsável | Data |
|----|---------------|--------------|--------|------------------|-----------------|--------|-------------|------|
| CT-001 | Login válido | Usuário cadastrado | 1. Acessar login <br> 2. Inserir credenciais <br> 3. Clicar Entrar | Acesso permitido | Acesso recusado | ⛔ Falhou | QA Team | {preencher} |
| CT-002 | Login inválido | Usuário cadastrado | 1. Acessar login <br> 2. Inserir senha errada <br> 3. Clicar Entrar | Mensagem de erro | Mensagem não exibida | ⛔ Falhou | QA Team | {preencher} |

> Adicione quantas linhas forem necessárias para todos os casos de teste.

---

## 5. Bugs Registrados

| ID | Caso de Teste | Severidade | Prioridade | Descrição | Status | Responsável | Data |
|----|---------------|------------|------------|-----------|--------|-------------|------|
| BUG-001 | CT-001 | Alta | Alta | Login não funciona | Aberto | QA Team | {preencher} |
| BUG-002 | CT-002 | Média | Média | Mensagem de erro do login não exibida | Corrigido | QA Team | {preencher} |

---

## 6. Métricas do Teste

| Métrica                      | Valor |
|-------------------------------|-------|
| Total de Casos de Teste       | {preencher} |
| Casos Executados              | {preencher} |
| Casos Aprovados               | {preencher} |
| Casos Reprovados              | {preencher} |
| Percentual de Sucesso (%)     | {preencher} |
| Cobertura de Requisitos (%)   | {preencher} |
| Cobertura de Funcionalidades (%) | {preencher} |
| Defeitos Abertos              | {preencher} |
| Defeitos Corrigidos           | {preencher} |

---

## 7. Observações / Comentários
- Pontos importantes durante a execução dos testes  
- Riscos identificados  
- Sugestões de melhoria para QA/Dev  
- Comportamentos inesperados observados  

---

## 8. Conclusão
Resumo do resultado geral do teste, áreas críticas, recomendações e status para release.  

**Exemplo:**  
> A funcionalidade de login passou em 95% dos casos. Alguns bugs menores foram encontrados na recuperação de senha. Recomendamos correção antes do próximo deploy.  
> **Recomendação para release:** [Liberar / Não liberar / Liberar parcialmente]  

---

## ✅ Checklist de Aprovação do Relatório
- [ ] Projeto preenchido  
- [ ] Níveis de teste selecionados  
- [ ] Tipos de teste selecionados  
- [ ] Casos de teste registrados  
- [ ] Bugs documentados  
- [ ] Métricas atualizadas  
- [ ] Observações adicionadas  
- [ ] Conclusão finalizada
