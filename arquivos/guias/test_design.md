---
layout: content
title: ''
hide_title: true
---


# 🎯 Técnicas de Design de Casos de Teste 
Cada técnica ajuda a escolher **quais dados, situações e combinações** devem ser testadas para cobrir o sistema de forma eficiente.  

**✅ Resumo Rápido**

| Técnica | Foco principal | Quando usar |
|----------|----------------|-------------|
| [Particionamento](#particionamento-de-equivalência) | Faixas de valores | Validação de campos |
| [Valor Limite](#análise-de-valor-limite) | Bordas numéricas | Campos com limites |
| [Tabela de decisão](#️tabelas-de-decisão) | Combinações de regras | Lógicas condicionais |
| [Transição de estado ](#transição-de-estados) | Etapas e fluxos | Processos com estados |
| [Caso de uso](#caso-de-uso-use-case-testing)  | Jornada do usuário | Testes ponta a ponta |
| [Pairwise](#teste-combinatório-pairwise) | Combinações reduzidas | Muitos parâmetros |
| [Exploratório](#teste-exploratório) | Descoberta livre | Sistemas novos |
| [Baseado em requisitos](#teste-baseado-em-requisitos) | Especificações | Projetos documentados |
| [Fluxo de dados](#teste-de-fluxo-de-dados) | Manipulação de dados | CRUDs e integrações |
| [Baseado em erros](#teste-baseado-em-erros) | Falhas prováveis | Validação geral |

---
## 🎯 Diferença entre Cenário e Caso de Teste

| Termo | O que é | Nível de detalhe | Exemplo |
|-------|----------|------------------|----------|
| **Cenário de Teste** | Uma **situação geral** que será verificada. | Mais **alto nível**, descreve o **contexto**. | “Verificar se o usuário consegue fazer login com credenciais válidas.” |
| **Caso de Teste** | O **passo a passo detalhado** para validar um cenário. | Mais **específico**, com **dados, ações e resultados esperados**. | 1️⃣ Abrir página de login <br> 2️⃣ Inserir `email@teste.com` e `senha123` <br> 3️⃣ Clicar em “Entrar” <br> ✅ Esperado: redirecionar para a página inicial. |

💡 **Resumindo:**  
- **Cenário = o que testar**  
- **Caso = como testar**

---

## Particionamento de Equivalência  
Divide os dados possíveis em **grupos (partições)** que se comportam do mesmo jeito.  
Você testa **um exemplo de cada grupo**, em vez de todos os valores possíveis.

**Exemplo prático:**  
Campo “idade” aceita valores de **18 a 60 anos**.  
- Valor **válido:** `30`  
- Valor **inválido abaixo:** `15`  
- Valor **inválido acima:** `70`

**Uso:** quando o campo tem **faixas, categorias ou regras claras de validação**.

---

## Análise de Valor Limite
Foca nos **limites exatos** onde o comportamento muda — é comum encontrar falhas “nas bordas”.

**Exemplo prático:**  
Campo “idade” aceita de **18 a 60 anos**.  
- `17` → abaixo do limite  
- `18` → no limite mínimo  
- `60` → no limite máximo  
- `61` → acima do limite  

**Uso:** quando há **intervalos numéricos** ou **quantidades mínimas/máximas**.

---

## Tabelas de Decisão
Organiza **regras e ações** em uma tabela para visualizar todas as combinações possíveis.

**Exemplo prático:**  

| Usuário correto | Senha correta | Resultado esperado |
|------------------|----------------|--------------------|
| Não              | Não            | Erro de login      |
| Sim              | Não            | Senha incorreta    |
| Não              | Sim            | Usuário inválido   |
| Sim              | Sim            | Login bem-sucedido |

**Uso:** quando há **múltiplas condições** que influenciam o resultado.

---

## Transição de Estados
Modela o comportamento de um sistema que **muda de estado** com base em ações ou eventos.

**Exemplo prático:**  

| Estado atual     | Ação            | Próximo estado |
|------------------|------------------|----------------|
| Pedido criado    | Pagamento aprovado | Pedido confirmado |
| Pedido confirmado | Pedido enviado     | A caminho       |
| A caminho        | Pedido entregue     | Concluído       |

**Uso:** quando o sistema tem **etapas sequenciais** ou **condições dependentes** do que veio antes.

---

## Caso de Uso (Use Case Testing)
Cria testes baseados em **fluxos de uso reais** do usuário.

**Exemplo prático:**  
Cenário: “Usuário faz uma compra com sucesso.”  
1. Acessa o site  
2. Adiciona produto ao carrinho  
3. Faz login  
4. Finaliza o pagamento  
✅ Resultado esperado: Pedido confirmado.

**Uso:** para validar **processos de ponta a ponta**.

---

## Teste Combinatório (Pairwise)
Usa combinações representativas de variáveis, evitando testar **todas as possíveis**.

**Exemplo prático:**  
Combinações de:
- Navegador (Chrome, Edge, Firefox)
- Sistema (Windows, Linux, Mac)
- Idioma (PT, EN)

Em vez de testar 3×3×2 = 18 combinações, escolhem-se **as mais relevantes** para cobrir as interações principais.

**Uso:** quando há **muitas variáveis de entrada**.

---

## Teste Exploratório
O testador **explora o sistema livremente**, observando o comportamento e criando casos de teste em tempo real.

**Exemplo prático:**  
Experimentar inserir dados incorretos, realizar ações fora de ordem, tentar fluxos incomuns.

**Uso:** quando o sistema é **novo, instável ou pouco documentado**.

---

## Teste Baseado em Requisitos
Cada requisito documentado se transforma em um ou mais casos de teste.

**Exemplo prático:**  
Requisito: “O campo de senha deve ter no mínimo 8 caracteres.”  
Casos de teste:
- Inserir 7 caracteres → erro  
- Inserir 8 caracteres → sucesso

**Uso:** quando o projeto tem **documentação formal ou histórias de usuário**.

---

## Teste de Fluxo de Dados
Verifica **como os dados são criados, modificados e eliminados** ao longo do sistema.

**Exemplo prático:**  
Testar se:
- Ao criar um usuário → o registro é salvo corretamente.  
- Ao deletar o usuário → o registro é removido do banco.  

**Uso:** quando há **muito processamento de dados** ou integrações entre módulos.

---

## Teste Baseado em Erros
Cria casos de teste inspirados em **erros comuns** que costumam ocorrer.

**Exemplo prático:**  
- Deixar campos obrigatórios em branco.  
- Inserir dados com caracteres especiais.  
- Quebrar uma sequência de etapas.

**Uso:** para **descobrir falhas prováveis** sem precisar de especificações formais.

---
