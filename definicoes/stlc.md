# 🧭 Ciclo de Vida do Teste de Software (STLC)
As **fases** ou **STLC** são as etapas que organizam o processo de teste do início ao fim.

 🗓️ **Planejamento:** definir o que será testado, prazos e ferramentas.  
 📋 **Análise:** entender os requisitos e identificar o que precisa de teste.  
 ✍️ **Design:** criar casos de teste e dados necessários.  
 ⚙️ **Implementação:** preparar o ambiente e as ferramentas.  
 🧪 **Execução:** rodar os testes e registrar resultados.  
 🐞 **Registro de defeitos:** reportar erros encontrados.  
 ✅ **Encerramento:** revisar resultados e registrar aprendizados.

💡 **Resumo:** garante que os testes sejam bem organizados, completos e úteis para validar a qualidade do software.

> 🔁 O STLC ocorre dentro do SDLC (Ciclo de Vida do Software) e se repete a cada nova entrega ou versão.

---

# 🗓️ Fase de Planejamento 
# 📋 Fase de Análise
# ✍️ Fase de Design:
# ⚙️ Implementação:
# 🧪 Execução:
# 🐞 Registro de defeitos:
# ✅ Encerramento:


## 🧱 Níveis de Teste – Em qual etapa ocorre o teste?

### Desenvolvimento:

💻 **Teste de Unidade:** Verifica se partes pequenas do **código** (funções, métodos) funcionam isoladamente.

🔗 **Teste de Integração:** Avalia se **diferentes módulos** do sistema funcionam corretamente **juntos**.

### Teste:  

🧩 **Teste de Sistema** Testa o **sistema completo**, simulando uso real.

📑 **Teste de Aceitação** Confirma se o sistema **atende aos requisitos** e **critérios de aceite** do cliente.

### Implantação
Subtipos do teste de aceitação:  
🧍‍♂️ **Teste Alfa:** executado internamente antes do lançamento público.  
🌍 **Teste Beta:** executado por usuários reais antes do lançamento oficial.

---



 


---

## 🧠 Técnicas de Teste – Como o teste vai ser feito?

A escolha depende do que está disponível:

📘 Tenho o código? → **Caixa branca**  
📄 Tenho requisitos claros? → **Caixa preta**  
❓ Não tenho documentação? → **Exploratória / Experiência**

---

### ⚫ Caixa Preta (Funcional)  
Foca no **que o sistema faz**, sem olhar o código.  
**Uso:** validar se o software atende aos requisitos.  


### ⚪ Caixa Branca (Estrutural)  
Foca na **lógica interna e no código**.  
**Uso:** garantir que partes do código sejam testadas.  
**Exemplos:**  
🔹 Cobertura de instruções  
🔹 Cobertura de decisões  
🔹 Cobertura de caminhos

---

### 🎯 Experiência (Exploratória)  
Baseada na **intuição e conhecimento do testador**.  
**Uso:** quando não há documentação ou o sistema é novo.  
**Exemplos:**  
🔹 Teste exploratório  
🔹 Teste baseado em erro  
🔹 Teste baseado em checklist

---

## 🧩 Tipos de Teste – O que está sendo avaliado?

Os testes se dividem em **Funcionais** e **Não Funcionais**.

---

### ⚙️ Funcionais

#### ✅ Teste de Funcionalidade  
Verifica se o sistema faz o que foi planejado.

**Subtipos:**

🚀 **Teste de Fumaça (Smoke Test)**  
  Verifica se o sistema funciona minimamente após uma nova build.  
  **Foco:** funcionalidades principais.

🔧 **Teste de Sanidade (Sanity Test)**  
  Valida se um bug corrigido ou uma funcionalidade específica está ok.  
  **Foco:** alterações recentes.

🔁 **Teste de Regressão**  
  Garante que novas mudanças **não quebrem** o que já funcionava.  
  **Foco:** estabilidade após modificações.

🔄 **Teste Ponta a Ponta (E2E)**  
  Simula o fluxo completo do sistema como um usuário real.  
  **Foco:** funcionamento total e integração de sistemas.

---

### ⚡ Não Funcionais

🚅 **Teste de Desempenho:** mede velocidade e estabilidade.  
  Inclui **carga**, **estresse** e **estabilidade**.  
🧍‍♀️ **Teste de Usabilidade:** verifica se é fácil e agradável de usar.  
🔒 **Teste de Segurança:** garante proteção de dados e autenticação.  
🌐 **Teste de Portabilidade / Compatibilidade:** verifica compatibilidade em sistemas, navegadores e dispositivos diferentes.

---

## ⚙️ Tipo de Execução – Como o teste é realizado?

### 🧑‍💻 Testes Manuais  
**Quando usar:** testes exploratórios, de usabilidade e validação visual.  
**Vantagens:** flexível, detecta falhas visuais e UX.  
**Desvantagens:** mais lento e sujeito a erro humano.  
**Ideal:** nas fases iniciais ou quando automatizar seria caro.

---

### 🤖 Testes Automatizados  
**Quando usar:** regressões, testes repetitivos e pipelines CI/CD.  
**Vantagens:** rápidos, consistentes e escaláveis.  
**Desvantagens:** exigem manutenção e investimento inicial.  
**Ideal:** sistemas grandes ou com entregas contínuas.

---

## 🗂️ Resumo Geral

| 📚 Categoria | ❓ Pergunta-chave                 | 💡 Exemplos                                |
| ------------- | -------------------------------- | ------------------------------------------ |
| 🧱 Nível      | “Em que etapa ocorre o teste?”  | Unidade, Integração, Sistema, Aceitação   |
| ⚙️ Tipo       | “O que está sendo avaliado?”    | Funcional, Desempenho, Segurança          |
| 🧠 Técnica    | “Como será testado?”            | Caixa preta, Caixa branca, Exploratória   |
| 🧑‍💻 Execução | “De que forma será executado?”  | Manual, Automatizado                      |

> 🔗 As classificações se combinam — um teste de regressão (tipo) pode ser automatizado (execução) e baseado em caixa preta (técnica).

---

# Sobre o design dos testes

## 🎯 Técnicas de Design de Casos de Teste

**Particionamento de Equivalência**  
Dividir os dados possíveis em **grupos que se comportam do mesmo jeito** no sistema.  
Em vez de testar todos os valores, testamos **um exemplo de cada grupo**.

**Exemplo:**  
Um campo aceita idades de **18 a 60 anos**.  
Você pode testar:
- Um valor **válido** → `30`
- Um valor **inválido abaixo** → `15`
- Um valor **inválido acima** → `70`

Assim, você cobre as três “partições” (faixas de comportamento).

---

**Análise de Valor Limite**  
Foca nos **limites exatos** onde o comportamento pode mudar.  
Erros costumam acontecer **nas bordas** dos intervalos.

**Exemplo:**  
Se o sistema aceita idades de **18 a 60**, você testa:
- `17` → abaixo do limite  
- `18` → **limite mínimo**  
- `60` → **limite máximo**  
- `61` → acima do limite

Esses testes garantem que o sistema trate bem as “pontas”.

---

**Tabelas de Decisão**  
Uma **tabela** que combina **condições** (regras) e mostra **qual ação** o sistema deve tomar em cada cenário.

**Exemplo:**  
Login com duas regras:  
- Usuário digitou o nome certo  
- Usuário digitou a senha certa  

| Usuário certo | Senha certa | Resultado         |
|----------------|--------------|------------------|
| Não            | Não          | Erro de login    |
| Sim            | Não          | Senha incorreta  |
| Não            | Sim          | Usuário inválido |
| Sim            | Sim          | Login bem-sucedido |

---

**Transição de Estados  
Mostra como o sistema **muda de estado** conforme as ações do usuário ou eventos.  
Usado quando o comportamento **depende do que aconteceu antes**.

**Exemplo:**  
Fluxo de um pedido em um app de delivery:

| Estado atual     | Ação do usuário      | Próximo estado   |
|------------------|----------------------|------------------|
| Pedido criado    | Pagamento aprovado   | Pedido confirmado |
| Pedido confirmado| Pedido enviado       | A caminho         |
| A caminho        | Pedido entregue      | Concluído         |

Você testa se o sistema **muda direitinho de um estado pro outro**.

---

**🧾 Comparativo Resumido**

| Técnica                   | Quando usar                                      | O que testa                        | Exemplo prático                     |
|----------------------------|--------------------------------------------------|------------------------------------|-------------------------------------|
| **Particionamento de equivalência** | Quando há faixas de entrada válidas e inválidas | Grupos de dados com mesmo comportamento | Idade 18–60                        |
| **Análise de valor limite** | Quando há limites definidos                      | Bordas de comportamento             | 17, 18, 60, 61                      |
| **Tabelas de decisão**      | Quando há várias combinações de regras           | Lógica condicional e cenários       | Login com usuário/senha             |
| **Transição de estados**    | Quando o sistema muda conforme ações anteriores  | Sequência e fluxo de estados        | Pedido → confirmado → entregue      |

---


## 🧩 Boas Práticas

### 🧷 Gerais
🗂️ Usar nomenclaturas e documentações padronizadas.  
💾 Versionar todos os documentos no Git.  
💬 Manter comunicação constante com o time de desenvolvimento.

### 🧠 Planejamento
🧩 Garantir que os requisitos estão claros e completos.  
📝 Criar cenários e casos de teste detalhados (simule erros e exceções).  
⏱️ Priorizar cenários conforme o tempo e impacto.

### 🧪 Execução
📸 Registrar resultados e evidências.

### 🔁 Pós-Teste
🐞 Acompanhar bugs até a correção.  
📘 Documentar lições aprendidas para os próximos ciclos.

---
