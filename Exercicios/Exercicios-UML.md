# UML

## 100 Exercícios sobre UML

### [1. Conceitos Fundamentais (1-10)](./Exercicios-UML/Conceitos-Fundamentais.md)

### [2. Diagrama de Classes (11-30)](./Conceitos-UML/Conceitos-Diagrama-De-Classes.md)

### 3. Diagrama de Casos de Uso (31-50)

1. O que é um **Ator** em um diagrama de casos de uso?
1. O que é um **Caso de Uso**?
1. Qual a função da fronteira do sistema?
1. Identifique os atores e os casos de uso para um sistema de banco online.
1. Identifique os atores e os casos de uso para um sistema de caixa eletrônico.
1. Explique a relação `include`. Quando ela deve ser usada?
1. Modele os casos de uso `Comprar Produto` e `Processar Pagamento`, usando a relação `include`.
1. Explique a relação `extend`. Quando ela deve ser usada?
1. Modele os casos de uso `Comprar Produto` e `Comprar Parcelado`, usando a relação `extend`.
1. Qual a diferença entre as relações `include` e `extend`?
1. Identifique os atores e casos de uso para um sistema de aluguel de filmes online.
1. Modele o caso de uso `Acessar Relatório de Vendas`. Inclua um ator `Gerente`.
1. Adicione o caso de uso `Gerar Relatório de Vendas` ao exercício anterior.
1. Identifique atores e casos de uso para um sistema de agendamento de consultas médicas.
1. Modele o caso de uso `Agendar Consulta`, usando `include` para o caso de uso `Verificar Disponibilidade`.
1. Modele o caso de uso `Agendar Consulta`, usando `extend` para o caso de uso `Enviar Lembrete`.
1. Identifique os atores e casos de uso para um sistema de biblioteca.
1. Modele o caso de uso `Fazer Empréstimo`. Use a relação `include` para `Verificar Status de Membro`.
1. Identifique os atores e casos de uso para um sistema de controle de tráfego aéreo.
1. Adicione um caso de uso `Notificar Atraso de Voo` ao exercício anterior, usando a relação `extend`.

---

### 4. Diagrama de Sequência (51-70)

1. O que é uma **Linha de Vida (Lifeline)**?
1. O que é uma **Mensagem**? Dê exemplos.
1. O que representa uma **Barra de Ativação (Activation Bar)**?
1. Modele uma interação de login: um `Usuário` envia uma mensagem de `login(usuario, senha)` para a `Tela de Login`. A tela envia uma mensagem para o `Sistema de Autenticação`.
1. Crie um diagrama de sequência para a compra de um produto: `Cliente` -> `Carrinho` -> `SistemaDePagamento`.
1. O que é um **fragmento de ciclo (loop)**?
1. Modele uma iteração em um diagrama de sequência que representa um `loop` de compra de vários produtos.
1. O que é um **fragmento de alternativa (alt)**?
1. Modele uma `alt` para um login que pode ser `bem-sucedido` ou `falhar`.
1. O que é um **fragmento opcional (opt)**?
1. Modele uma ação opcional de `enviar e-mail de confirmação` após a compra.
1. Crie um diagrama de sequência para o processo de um empréstimo, onde o `Cliente` interage com o `Sistema`, que por sua vez interage com o `Gerente`.
1. Modele uma interação onde um `Serviço` invoca o método de outro `Serviço` em um ambiente de microsserviços.
1. Adicione um fragmento `opt` para `solicitarCupom()` à sequência de compra do exercício 55.
1. Crie um diagrama de sequência para o envio de uma mensagem em um chat: `Remetente` -> `Servidor` -> `Destinatário`.
1. Modele uma sequência onde um `Gateway` distribui uma mensagem para vários `Serviços` (use o fragmento `par`).
1. Crie um diagrama de sequência para um cadastro de usuário, incluindo a `Tela de Cadastro` e o `Sistema de Usuários`.
1. Adicione um `alt` para `usuário já existe` no diagrama do exercício 67.
1. Modele uma interação entre um cliente, a interface e o banco de dados para a busca de um produto.
1. Crie um diagrama de sequência para um processo de reset de senha.

---

### 5. Diagrama de Atividades (71-85)

1. Qual o propósito de um diagrama de atividades?
1. O que são os nós de **Ação (Action)** e de **Atividade (Activity)**?
1. O que é um nó de **Decisão (Decision Node)**?
1. O que é um nó de **Fusão (Merge Node)**?
1. Modele um fluxo de atividade para o processo de login, com uma decisão para "credenciais válidas".
1. Modele um fluxo de atividade para o processo de um pedido, com ações para `Verificar Estoque`, `Processar Pagamento` e `Enviar Pedido`.
1. O que são os nós de **Divisão (Fork)** e **Junção (Join)**?
1. Modele um fluxo de atividade que executa `Enviando E-mail de Confirmação` e `Atualizando o Estoque` em paralelo.
1. Modele um fluxo de atividade para o processo de um `download` de arquivo que pode ser cancelado a qualquer momento.
1. Modele um fluxo de atividade para o processo de um empréstimo bancário, com uma decisão para "aprovar" ou "rejeitar".
1. Modele um fluxo para um processo de votação online.
1. Use `lanes` para modelar um fluxo de atividade onde um `Cliente` e o `Sistema` interagem.
1. Crie um diagrama de atividade para o processo de agendamento de consultas médicas.
1. Adicione uma decisão ao diagrama do exercício 83 para `cancelamento` da consulta.
1. Modele o fluxo de um processo de compras online, incluindo a navegação, seleção de produtos e pagamento.

---

### 6. Diagrama de Máquina de Estado (86-100)

1. O que é um estado em um diagrama de máquina de estado?
1. O que é uma **Transição (Transition)**?
1. Explique a diferença entre um evento e uma ação em um diagrama de máquina de estado.
1. Modele o ciclo de vida de uma `Lâmpada` com os estados `Ligada` e `Desligada`.
1. Modele o ciclo de vida de um `Pedido` em um sistema de e-commerce, com os estados `Aguardando Pagamento`, `Pago`, `Enviado` e `Entregue`.
1. Qual a função de um estado de **início** e de **fim**?
1. O que é uma **condição de guarda (guard condition)**?
1. Modele uma transição de estado de `Aguardando Pagamento` para `Pago` com uma condição de guarda `[valor > 0]`.
1. O que é uma ação de **entrada (entry)** e de **saída (exit)**?
1. Adicione uma ação de `entry` para `enviar e-mail de confirmação` ao estado `Pago` do exercício 90.
1. Modele o ciclo de vida de um `Ticket de Suporte` com os estados `Aberto`, `Em Andamento`, `Resolvido` e `Fechado`.
1. Modele o ciclo de vida de um `Leilão Online` com os estados `Aberto`, `Em Andamento` e `Encerrado`.
1. Modele o ciclo de vida de uma `Reserva de Voo`, considerando os estados `Reservado`, `Confirmado` e `Cancelado`.
1. Modele o ciclo de vida de um `Semáforo` em um cruzamento, incluindo os estados `Verde`, `Amarelo` e `Vermelho` com seus respectivos temporizadores.
1. Modele o ciclo de vida de um `Robô Aspirador`, com os estados `Parado`, `Aspirando` e `Carregando`.
