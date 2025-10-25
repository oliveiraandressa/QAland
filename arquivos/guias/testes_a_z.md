[⬅Voltar](../../readme.md)  

# Guia de Testes (Níveis, técnicas e tipos)

## 🧱 Níveis de Teste 
Em qual etapa do ciclo do software ocorrerá o teste?  

### Desenvolvimento:

💻 **Teste de Unidade:** Verifica se partes pequenas do **código** (funções, métodos) funcionam isoladamente.

🔗 **Teste de Integração:** Avalia se **diferentes módulos** do sistema funcionam corretamente **juntos**.

---

### Teste e Implantação:  

🧩 **Teste de Sistema** Testa o **sistema completo**, simulando uso real.

📑 **Teste de Aceitação** Confirma se o sistema atende aos requisitos e critérios de aceite do cliente e possui 2 subitipos:
- 🧍‍♂️ **Teste Alfa:** executado internamente antes do lançamento público.  
- 🌍 **Teste Beta:** executado por usuários reais antes do lançamento oficial.

---

## 🧠 Técnicas de Teste
A escolha depende do que está disponível:

📘 Tenho o código? → Caixa branca, que foca na **lógica interna e no código**.  
📄 Tenho requisitos claros? → Caixa preta, que foca no **que o sistema faz**, sem olhar o código.  
❓ Não tenho documentação? → Exploratória, que baseada na **intuição e conhecimento do testador**.  

---

## 🧩 Tipos de Teste

Os testes se dividem em **Funcionais** e **Não Funcionais**.  

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

🚅 **Teste de Desempenho:** mede velocidade e estabilidade. Inclui **carga**, **estresse** e **estabilidade**.  
🧍‍♀️ **Teste de Usabilidade:** verifica se é fácil e agradável de usar.  
🔒 **Teste de Segurança:** garante proteção de dados e autenticação.  
🌐 **Teste de Portabilidade / Compatibilidade:** verifica compatibilidade em sistemas, navegadores e dispositivos diferentes.

---

## ⚙️ Tipo de Execução 

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