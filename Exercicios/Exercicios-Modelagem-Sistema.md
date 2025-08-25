# Exercicio de Modelagem de Sistema

## 100 Perguntas Essenciais sobre Modelagem de Sistemas

### Conceitos Fundamentais

1. O que é modelagem de sistemas? Qual seu propósito principal?
1. Qual a diferença entre modelar e programar um sistema?
1. Explique a importância da abstração na modelagem de sistemas.
1. O que é um modelo de sistema?
1. Quais são os principais benefícios da modelagem de sistemas para o ciclo de vida do software?

---

### Modelagem de Processos de Negócio

1. O que é um processo de negócio?
1. Qual a diferença entre modelagem "as-is" e "to-be"?
1. Quais são os principais elementos de um diagrama de fluxo de dados (DFD)?
1. O que é uma notação de modelagem de processo de negócio (BPMN)?
1. O que representam os *pools* e *lanes* em um diagrama BPMN?
1. Como um processo de negócio é modelado para identificar gargalos?
1. O que é um evento e uma atividade em BPMN?
1. Qual a diferença entre um *Gateway* inclusivo e exclusivo em BPMN?
1. Como você modelaria a interação entre sistemas e usuários em um processo de negócio?
1. O que é a modelagem de casos de uso e como ela se relaciona com os processos de negócio?

---

### Modelagem Orientada a Objetos com UML

1. O que é UML (Unified Modeling Language)? Qual sua importância?
1. Qual a diferença entre um diagrama estrutural e um diagrama comportamental na UML?
1. O que é um diagrama de classes? Quais são seus componentes principais?
1. Explique os conceitos de **classe**, **atributo** e **método**.
1. O que são os tipos de relacionamento **associação**, **agregação** e **composição** em um diagrama de classes?
1. Qual a diferença entre agregação e composição?
1. O que é **generalização** (herança) em um diagrama de classes?
1. Explique a **realização** (interface) na UML.
1. O que é um diagrama de objetos? Qual sua relação com o diagrama de classes?
1. O que é um diagrama de pacotes e para que ele serve?

---

### Modelagem de Comportamento

1. O que é um diagrama de casos de uso? Quais são seus elementos?
1. Explique os relacionamentos `include` e `extend` em um diagrama de casos de uso.
1. O que é um diagrama de sequência e para que ele é usado?
1. Qual a diferença entre um diagrama de sequência e um diagrama de comunicação?
1. O que é um diagrama de máquina de estados?
1. Quais são os elementos principais de um diagrama de máquina de estados?
1. Quando você usaria um diagrama de máquina de estados em vez de um diagrama de atividades?
1. O que é um diagrama de atividades? Para que ele é usado?
1. Qual a diferença entre um diagrama de atividades e um fluxograma tradicional?
1. Como um diagrama de atividades pode representar paralelismo?
1. O que é um diagrama de tempo?
1. O que é um *Lifeline* e uma *Message* em um diagrama de sequência?
1. Explique o conceito de `loop` e `alt` em um diagrama de sequência.
1. Como você modelaria a interação entre um usuário e a interface de um sistema?
1. O que é um diagrama de interações e como ele se diferencia dos outros diagramas comportamentais?

---

### Modelagem de Arquitetura e Estrutura

1. O que é um diagrama de componentes?
1. Como um diagrama de componentes representa a arquitetura de um sistema?
1. O que é uma **porta** em um diagrama de componentes?
1. O que é um diagrama de implantação (ou *deployment*)?
1. Quais são os elementos principais de um diagrama de implantação?
1. Como você modelaria a distribuição física de componentes de software em um hardware?
1. O que é um **nó** e um **artefato** em um diagrama de implantação?
1. Qual a diferença entre um diagrama de componentes e um diagrama de classes?
1. Como a modelagem de arquitetura pode ajudar a evitar falhas de sistema?
1. O que é um diagrama de estrutura composta? Para que ele serve?

---

### Ferramentas e Metodologias

1. Cite três ferramentas de modelagem UML populares.
1. O que é uma metodologia de desenvolvimento de software e como ela se relaciona com a modelagem?
1. Como a modelagem é adaptada em metodologias ágeis como o Scrum?
1. Qual a diferença entre modelagem *top-down* e *bottom-up*?
1. O que é **Domain-Driven Design (DDD)**? Como a modelagem é central para ele?
1. O que são as **arquiteturas de referência** e como elas influenciam a modelagem?
1. Como a modelagem de sistemas é usada na abordagem de *Microservices*?
1. O que é um *Design Pattern*? Como ele se relaciona com a modelagem?
1. Qual a importância do **padrão MVC** (Model-View-Controller) na modelagem de sistemas web?
1. Como a modelagem de sistemas se integra à engenharia de requisitos?

---

### Modelagem de Dados

1. O que é um modelo de dados? Qual sua relação com a modelagem de sistemas?
1. Qual a diferença entre modelo de dados **conceitual**, **lógico** e **físico**?
1. O que é uma **entidade** e um **relacionamento** em um Diagrama de Entidade-Relacionamento (DER)?
1. Explique o conceito de cardinalidade em um DER.
1. Qual a diferença entre um DER e um diagrama de classes UML?
1. O que é **normalização** de dados? Por que é importante?
1. O que é uma **chave primária** e uma **chave estrangeira**?
1. Como a modelagem de dados influencia a performance de um sistema?
1. O que é um **dicionário de dados** e qual sua função?
1. Como você modelaria dados para um sistema com requisitos de *Big Data*?

---

### Desafios e Boas Práticas

1. Qual o maior desafio na modelagem de sistemas complexos?
1. Como garantir que um modelo seja preciso e consistente?
1. O que é um modelo de sistema **dinâmico** e como ele se diferencia de um **estático**?
1. Como a comunicação entre os *stakeholders* e os modeladores pode ser otimizada?
1. Qual o papel da **prototipagem** na modelagem de sistemas?
1. Como a modelagem de sistemas pode ser usada para identificar riscos e vulnerabilidades?
1. O que é um **modelo de sistema de tempo real**?
1. Como a modelagem pode ajudar na refatoração de um sistema legado?
1. O que é a modelagem de sistemas distribuídos?
1. Como a modelagem ajuda na **escalabilidade** e **manutenibilidade** de um sistema?

---

### Cenários Práticos

1. Modele o processo de compra online de um cliente.
Para modelar um sistema de compras online, você precisaria identificar as entidades (no contexto de modelagem de dados) ou classes (no contexto de modelagem orientada a objetos) que representam os principais elementos e atores do processo.

Aqui estão as entidades ou classes essenciais, com suas características e relacionamentos.

### Entidades/Classes Essenciais

#### 1. Cliente (ou Usuário)

Representa a pessoa que está fazendo a compra. É a entidade central para rastrear a atividade do usuário.

* **Atributos:** `id_cliente`, `nome`, `email`, `senha`, `data_cadastro`, `telefone`.

#### 2. Produto

Representa o item que está sendo vendido. É a base do catálogo da loja.

* **Atributos:** `id_produto`, `nome_produto`, `descricao`, `preco`, `sku` (código de estoque), `url_imagem`.

#### 3. Pedido

Representa a transação de compra em si. Um `Pedido` é um conjunto de produtos comprados por um `Cliente` em um determinado momento.

* **Atributos:** `id_pedido`, `data_criacao`, `status_pedido` (ex: `pendente`, `processando`, `enviado`, `entregue`, `cancelado`), `valor_total`.

#### 4. Item do Pedido (ou Linha do Pedido)

Essa é uma classe crucial que faz a conexão entre um `Pedido` e um `Produto`. Como um pedido pode ter vários produtos e um produto pode estar em vários pedidos, essa entidade resolve o relacionamento muitos-para-muitos.

* **Atributos:** `id_item_pedido`, `quantidade`, `preco_unitario_na_compra`.

#### 5. Pagamento

Representa a transação financeira para o pagamento do pedido.

* **Atributos:** `id_pagamento`, `metodo_pagamento`, `valor`, `status_pagamento` (ex: `pendente`, `aprovado`, `rejeitado`), `data_pagamento`.

#### 6. Endereço

Representa os endereços de entrega e faturamento do cliente. Um cliente pode ter vários endereços registrados.

* **Atributos:** `id_endereco`, `rua`, `numero`, `complemento`, `cidade`, `estado`, `cep`, `tipo_endereco` (ex: `entrega`, `faturamento`).

---

#### Relacionamentos entre as Entidades

Os relacionamentos são tão importantes quanto as entidades. Eles definem como as informações se conectam.

* Um **Cliente** faz **N** (muitos) **Pedidos**. (Relacionamento de 1 para N)
* Um **Pedido** contém **N** (muitos) **Itens do Pedido**. (Relacionamento de 1 para N)
* Um **Produto** pode estar em **N** (muitos) **Itens do Pedido**. (Relacionamento de 1 para N)
* Um **Pedido** pode ter **1** (um) **Pagamento** (e um `Pagamento` pertence a um `Pedido`). (Relacionamento de 1 para 1)
* Um **Cliente** tem **N** (muitos) **Endereços**. (Relacionamento de 1 para N)

#### Entidades Adicionais (Para Modelos Mais Complexos)

* **Estoque:** Para gerenciar a disponibilidade de produtos.
* **Categoria:** Para organizar os produtos (ex: "Eletrônicos", "Moda").
* **Avaliação:** Para armazenar as opiniões e notas dos clientes sobre os produtos.
* **Cupom de Desconto:** Para gerenciar promoções.
* **Envio:** Para rastrear a entrega do pedido (transportadora, código de rastreio, status).
* **Carrinho de Compras:** Uma classe temporária que armazena os itens que o usuário selecionou antes de finalizar o pedido.

---

1. Modele um diagrama de classes para um sistema de gerenciamento de biblioteca.
1. Crie um diagrama de sequência para o login de um usuário.
1. Como você modelaria um sistema de controle de acesso a um prédio?
1. Modele um sistema de reserva de um restaurante usando um diagrama de estado.
1. Como você modelaria a arquitetura de um aplicativo de transporte como o Uber?
1. Modele o processo de aprovação de uma despesa em uma empresa.
1. Qual seria o diagrama mais adequado para modelar a interação entre um chatbot e um usuário?
1. Como você modelaria um sistema de monitoramento de IoT?
1. Modele a interação entre diferentes microsserviços em um sistema de e-commerce.

---

### Tópicos Avançados

1. O que é a **Ontologia de Sistemas** e como ela se aplica à modelagem?
1. O que é a **Linguagem de Modelagem de Sistemas (SysML)** e qual sua relação com a UML?
1. Como a modelagem é utilizada na engenharia de sistemas *baseada em modelos* (MBSE)?
1. O que é um **modelo de simulação** e qual sua importância?
1. Qual o papel da modelagem na **arquitetura orientada a serviços (SOA)**?
1. O que é um **metamodelo**?
1. Como a inteligência artificial pode ser usada para auxiliar na modelagem de sistemas?
1. O que é um **gemelo digital** (*digital twin*) e como ele se relaciona com a modelagem?
1. Como a modelagem de sistemas é usada em ambientes de *cloud computing*?
1. Qual o futuro da modelagem de sistemas na era do *Big Data* e da **IA**?
