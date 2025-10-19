# A
## API
Interface de programação de aplicações.

**Exemplo prático:**  
Um aplicativo de previsão do tempo no celular pede ao servidor a previsão para sua cidade. Esse pedido e a resposta (dados do tempo) são feitos por uma API — você vê apenas o app, a API é a “conversa” entre o app e o serviço de dados.

# B
## Backlog
Lista priorizada de tarefas ou requisitos a serem entregues.

**Exemplo prático:**  
Imagine uma lista de compras onde os itens mais importantes vêm primeiro. Em um time, o backlog é essa lista: "corrigir bug X", "adicionar busca", ordenada por prioridade para a equipe trabalhar.

# C
## Cache
Armazenamento temporário para acesso mais rápido a dados.

**Exemplo prático:**  
No navegador, ao visitar um site, imagens e dados são guardados localmente. Na próxima visita, o site carrega mais rápido porque usou o cache em vez de baixar tudo novamente.


## CI/CD
Conjunto de práticas e ferramentas que automatizam a integração contínua (CI) — integrar alterações e executar testes automaticamente — e a entrega/implantação contínua (CD) — disponibilizar builds aprovados em ambientes como staging ou produção.

**Exemplo prático:**  
Ao fazer um push para a branch main, um pipeline do GitHub Actions roda: 1) instala dependências e executa testes automatizados; 2) builda a aplicação; 3) se os testes passarem, faz o deploy para o ambiente de staging; 4) após validação, o mesmo pipeline ou um passo manual promove a versão para produção. Para leigos: é como um esteira automática que testa e coloca novas versões do site no ar sem intervenção manual diária.

# D
## Deploy
Processo de publicar uma versão da aplicação em um ambiente.

**Exemplo prático:**  
Quando um desenvolvedor envia novas funcionalidades para o site da empresa, ele faz o deploy — equivalente a “colocar a nova versão no ar” para os usuários verem.

# E
## Endpoint
URL ou rota que expõe uma funcionalidade de uma API.

**Exemplo prático:**  
Ao fazer login num site, o app chama um endpoint como /api/login. Esse endpoint recebe email e senha e responde se o acesso foi autorizado.

# F
## Feature
Funcionalidade nova ou melhoria implementada no sistema.

**Exemplo prático:**  
Adicionar um botão "Compartilhar" para postar conteúdo nas redes sociais é uma feature — algo novo que passa a fazer parte do produto.

# G
## Git
Sistema de controle de versão distribuído.

**Exemplo prático:**  
Como um histórico automático do trabalho: você salva versões do código, pode voltar a uma versão antiga ou trabalhar em paralelo (branch) sem mexer no trabalho principal.

# H
## Hotfix
Correção urgente aplicada diretamente em produção.

**Exemplo prático:**  
Se a página de pagamento parou de aceitar cartões, um hotfix é a correção rápida aplicada imediatamente para restabelecer as vendas.

## História de usuário (US)
Descrição curta de uma necessidade do usuário escrita do ponto de vista do usuário final. Geralmente segue o formato: "Como [tipo de usuário], eu quero [ação/objetivo] para [benefício/valor]". Histórias de usuário orientam o que deve ser desenvolvido e servem de base para critérios de aceitação e testes.

**Exemplo prático:**  
Joana, dona de uma pequena loja, precisa acompanhar vendas enquanto não está no computador. Uma história de usuário poderia ser: "Como proprietária da loja, eu quero receber uma notificação no celular quando uma venda for concluída, para acompanhar o faturamento em tempo real." Critérios de aceitação associados poderiam incluir: receber notificação em menos de 30 segundos após a confirmação de pagamento e ver os detalhes do pedido na notificação. Essa história ajuda desenvolvedores, QA e produto a entenderem claramente o que entregar e como validar.


# I
## Issue
Registro de problema, bug ou tarefa em um sistema de acompanhamento.

**Exemplo prático:**  
Um usuário relata que ao clicar em "Salvar" o sistema trava. Isso vira uma issue com descrição, passos para reproduzir e prioridade para a equipe investigar.

# J
## JWT
Token compacto usado para autenticação e autorização.

**Exemplo prático:**  
Depois de fazer login, o site entrega um token (JWT). O navegador guarda esse token e o envia em cada pedido ao servidor para provar que você está autenticado, sem precisar pedir email/senha toda vez.

# K
## KPI
Indicador-chave de desempenho usado para medir resultados.

**Exemplo prático:**  
Para uma loja online, um KPI pode ser "taxa de conversão" (quantas visitas viram compra). Serve para avaliar se mudanças estão funcionando.

# L
## Log
Registro de eventos ou mensagens geradas pela aplicação.

**Exemplo prático:**  
Quando um usuário tenta fazer login e falha, o sistema grava um log com hora, usuário e erro. Isso ajuda o time a entender o que aconteceu e quando.

# M
## Mock
Simulação de dados usada em testes.

**Exemplo prático:**  
Ao testar a tela que mostra usuários, em vez de chamar o servidor real você usa um mock que devolve uma lista pré-definida — assim o teste roda rápido e sem depender da rede.

# N
## Node
Ambiente de execução JavaScript (Node.js) ou nó em uma rede.

**Exemplo prático:**  
Para desenvolver uma API localmente, você roda um servidor com Node que responde às requisições; é o "motor" que executa JavaScript fora do navegador.

# O
## ORM
Mapeamento objeto-relacional para facilitar acesso a bancos de dados.

**Exemplo prático:**  
Em vez de escrever SQL, você usa um ORM para dizer "crie um usuário com nome X" e o ORM transforma isso em comandos para o banco, facilitando o trabalho do desenvolvedor.

# P
## Pull request
Solicitação de integração de mudanças no repositório.

**Exemplo prático:**  
Você fez ajustes numa funcionalidade e abre um pull request para que colegas revisem o código antes de mesclar essas mudanças ao projeto principal.

# Q
## QA
Garantia de qualidade; práticas e testes para assegurar confiabilidade.

**Exemplo prático:**  
Antes de lançar uma versão, a equipe de QA testa fluxos críticos (login, compra) manualmente e com automação para garantir que tudo funciona como esperado.

# R
## Regressão
Falha que reaparece após alterações no sistema.

**Exemplo prático:**  
Um bug no relatório foi corrigido, mas depois de uma atualização ele voltou a ocorrer — isso é uma regressão. Testes automatizados ajudam a detectar regressões cedo.

# S
## Staging
Ambiente de pré-produção para validação antes do deploy em produção.

**Exemplo prático:**  
Staging é um site igual ao de produção onde QA e stakeholders validam as mudanças antes de liberar ao público, evitando surpresas.

## Stub
Implementação mínima ou substituta usada durante desenvolvimento ou testes que devolve respostas pré-definidas, sem executar a lógica completa.

**Exemplo prático:**  
Suponha que o serviço de pagamento ainda não esteja pronto. Para que a equipe possa desenvolver e testar a tela de finalização de pedido, cria-se um stub que sempre responde "pagamento aprovado". Com isso, desenvolvedores e testadores conseguem avançar sem depender do serviço real. Outro exemplo: ao construir a lista de contatos, um stub pode fornecer três contatos fictícios para testar a interface sem conectar ao servidor.


# T
## Teste
Verificação que valida comportamento e requisitos do sistema.

**Exemplo prático:**  
Um teste pode checar se, ao inserir email e senha corretos e clicar em "Entrar", o usuário é levado ao painel — confirmando que o login funciona.

# U
## UI
Interface do usuário; elementos visuais e interativos.

**Exemplo prático:**  
Campos de formulário, botões e menus que você vê numa tela são a UI — tudo aquilo com que o usuário interage.

# V
## Versionamento
Controle e organização das versões do software.

**Exemplo prático:**  
Colocar tags como v1.0, v1.1 nas versões do software ajuda a saber exatamente qual código rodava numa data ou em uma implantação específica.

# W
## Webhook
Notificação HTTP enviada a uma URL quando um evento ocorre.

**Exemplo prático:**  
Um serviço de pagamento envia um webhook ao seu sistema assim que uma cobrança é confirmada; com isso você atualiza o pedido automaticamente sem precisar consultar o pagamento sempre.

# X
## XML
Linguagem de marcação extensível para troca de dados.

**Exemplo prático:**  
Alguns sistemas legados enviam notas fiscais em XML. Para processar a nota, sua aplicação lê o XML e extrai informações como valor e CNPJ.

# Y
## YAML
Formato de serialização legível por humanos, usado em configurações.

**Exemplo prático:**  
Arquivos de configuração de pipelines (por exemplo GitHub Actions) costumam ser em YAML — é um jeito simples de definir passos que o sistema deve executar.

# Z
## Zero-downtime
Estratégia de atualização sem interromper o serviço.

**Exemplo prático:**  
Num blue-green deployment, você prepara uma versão nova (green) enquanto a atual (blue) segue atendendo usuários; ao validar a green, redireciona o tráfego para ela sem desligar o serviço.
