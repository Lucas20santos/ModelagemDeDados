# UML

## 100 Exercícios sobre UML

### Conceitos Fundamentais (1-10)

1. O que significa a sigla UML?
    - A sigla UML significa Unified Modeling Language, ou Linguagem de Modelagem Unificada em português. É uma linguagem padrão para modelagem de sitemas de software, utilizada para visualizar, especificar, construir e documentar a estrutura e o comportamento de sistemas complexos.

1. Qual o propósito principal da UML na engenharia de software?
    - A UML é uma ferramenta visual que ajuda desenvolvedores e outra partes interessadas a entender e comunicar como um sistema de software funciona, incluindo seus componentes, interações e processos.

    A UML foi criada para resolver a falta de padronização na modelagem de sistemas de software na década de 1990, e hoje é amplamente utilizada no desenvolvimento de software orientado a objetos e em outras áreas.
1. Qual a diferença entre um diagrama estrutural e um diagrama comportamental?
    - A diferença fundamental é que os diagramas estruturais mostram a estrutura estática de um sistema, delineando como os componentes se organizam e se relacionam, enquanto os diagramas comportamentais exibem o dinamismo do sistema, mostrando como os componentes interagem e processam informações ao longo do tempo. Em resumo, um descreve o "o quê" do sistema e o outro "como".
    - **Diagramas Estruturais (Estáticos)**
        - Foco: A estrutura e os relacionamentos entre os elementos de um sistema.
        - Visualização: Os componentes que compõem o sistema, como classes, objetos e suas relações.
        - Objetivo: Detalhar a organização e a arquitetura de um sistema.
        - Exemplos:
            - Diagramas classes: Mostra as classes, seus atributos, métodos e as relações
            - Diagrama de Componentes: Representa os componentes do sistema e como eles são organizados.
    - Diagrams Comportamentias (Dinãmicos)
        - Foco: A dinâmica e o fluxo de controle de um sistema, detalhando como os componetnes interagem.
        - Visualização: O comportamento do sistema em resposta a eventos e ações, incluindo as interações entre objetos.
        - Objetivo: Modelar o fluxo de trabalho, processos de negócio e a interação entre os elementos do sistema.
        - Exemplos:
            - Diagrama de Sequência: Mostra a ordem das interações entre objetos ao longo do tempo em um cenário específio.
            - Diagrama de Atividade: Representa o fluxo de trabalho e os processos dentro de um sitema.
1. Cite os diagramas estruturais e os diagramas comportamentais da UML.
    - A UML tem 14 diagrams divididos em duas categorias: 7 diagrams estruturais (que mostram a estrutura estática de um sistema) e 7 diagrams comportamentias (que mostram o comportamento dinâmico de um sistema). Os diagrams estruturais incluem: Classe, Componente, Implantação, Objeto, Pacote, Perfil e Estrutura COmposta. Os diagramas comportamentais incluem: Caso de Uso, Atividade, Estado, Sequeância, Comunicação, Visão Geral de Interação e Tempo.
    - **Diagramas Estruturais(Estáticos)**
        - Estes diagramas focam na arquitetura de um sistema, mostrando seus componentes e as relações entre eles.
        - **Diagrama de classe**: Descreve a estrutura de um sitema em termos de classes, interfaces, seus atributos, métodos e os relacionamentos entre eles.
        - **Diagrama de Componente**: Mostra os componentes de um sistema, como as partes modulares, e as dependências entre eles.
        - **Diagrama de implantação**: Ilustra a disposição do hardware e software, mostrando como os componentes de software são distribuídos no hardware do sistema.
        - **Diagrama de Objeto**: Apresenta um instantãneo de uma estrutura em um ponto específico do tempo, mostrando objetos e suas relações.
        - **Diagrama de Pacote**: Organiza os elementos da UML em grupos lógicos, mostrando as dependências entre esses pacotes.
        - **Diagrama de Perfil**: Permite a criação de extensões da UML para modelar elementos específicos de um domínio.
        - **Diagrama de Estrutura composta**: Detalha a estrutura interna de um classificador, mostrando suas partes, portas e os relacionamentos que definem seu comportamento.
    - Diagramas Comportamentais (Dinâmicos): Estes diagrams representam o comportamento de um sistema, mostrando como os componentes interagem e mudam ao longo do tempo.
        - **Diagrama de Atividade**: Mostra o fluxo de trabalho, os passos sequenciais, ramificados ou simultâneos que compõem um processo ou um cado de uso.
        - **Diagrama de Estado**: Descreve os diferentes estados de um objeto e as transições que ocorrem entre eles em resposta a eventos.
        - **Diagrama de Sequência**: Ilustra a ordem das interações entre os objetos ao longo do tempo.
        - **Diagrama de comunicação**: Também conhecido como diagrama de colaboração, mostra como os objetos se relacionam e colaboram para realizzar uma função.
        - **Diagrama de Visão Geral da Interação**: Apresenta a visão geral da interação entre múltiplos diaagrams de sequência, mostrando como eles se conectam e se relacionam.
1. O que é um **modelo** UML?
    - É um conjunto de elementos e símbolos gráficos (em diagramas) para representar a arquitetura, e design e a estrtura de um sistema, facilitando a comunicação entre desenvolvedores e outrs stakeholders, transformando ideias complexas em modelos claros e compreensíveis.
1. Qual a relação entre um diagrama e um modelo?
    - Um diagrama é uma representação visual e simplificada de um aspecto ou parte de um modelo, que é uma representação mais completa e detalhada de um sistema, processo ou conceito. Os diagrams servem como "fotografias" para ilustrar elementos específicos do modelo, enquanto o modelo como um todo unifica esses diagramas e informações adicionais, proporcionando uma visão mais profunda e, por vezes, executável do objeto de estudo.
1. Por que a UML é importante para a comunicação em um projeto de software?
    - Porque fornece uma linguagem visual e padronizada para descrever sistemas complexos, facilitando a compreensão e colaboração entre desenvolvedores, analistas e outras parte interessadas. Ela melhora a clareza da documentação, ajuda a identificar requisitos e erros precocemente e permite que equipes entendam a estrutura e o comportamenteo do sistema, mesmo em projetos de grande escala.
1. Explique o conceito de **abstração** na UML.
    - Na UML, abstração é um relacionamenteo que conecta elementos que representam o mesmo conceito emdiferentes níveis de detalhe ou perspectiva, como uma especificação e a sua implementação. É um pilar da orientação a objetos que permite focar nos detalhes essenciais, ignorando o irrelevante, sendo expressa em classes abstratas (com nomes em itálico) e como um relacionamente de dependência, muitas vezes denotado pr uma linha tracejada com uma seta abert e a palavra-chave "<<abstração>>"
1. O que é a notação e o que é a semântica de um diagrama?
    - A notação de um diagrama são os símbolos e elementos gráficos que o compõem, como formas, linhas ee setas, que representam conceitos e relacionamentos. Já a semântica é o significado e a interpretação desses elementos, ou seja, o que cada símbolo representa e como a sua relação com outros elementos transmite uma mensagem compreensível sobre o sistema ou processo modelado.
1. Como a UML pode ser útil para sistemas não orientados a objetos?
    - A UML é útil para sistemas nmão orientados a objetos porque sua notação é flexível, permitindo que se modele a estrutura (componetnes, nós) e o comportamento (fluxos de atividades, casos de uso) desses sistemas de forma independente de linguagem de programação ou paradigma. Diagramas como o de atividades, casos de uso e componentes são especialmente eficazes para visualizar a organização, a lógica e as interações de processos em sistemas não orientados a objetos, facilitando a comunicação, a documentação e a manutenção.

---

### 2. Diagrama de Classes (11-30)

1. O que é uma classe em UML? Liste seus três compartimentos.
1. Crie uma classe `Livro` com os atributos `título` e `autor`.
1. Adicione o método `exibirDetalhes()` à classe `Livro`.
1. Explique a diferença entre um atributo público (`+`), privado (`-`) e protegido (`#`).
1. Defina a relação de **Associação**. Dê um exemplo.
1. Represente a relação entre as classes `Cliente` e `Pedido`. Qual a cardinalidade?
1. O que é **Associação de Agregação**? Dê um exemplo e desenhe o símbolo.
1. O que é **Associação de Composição**? Dê um exemplo e desenhe o símbolo.
1. Qual a principal diferença entre Agregação e Composição?
1. Crie um diagrama de classes para um sistema de biblioteca com as classes `Livro`, `Membro` e `Empréstimo`.
1. Explique a relação de **Generalização (Herança)**.
1. Modele a relação de herança entre `Animal`, `Cachorro` e `Gato`.
1. O que é a relação de **Realização (Implementação)**?
1. Modele a relação onde a classe `Carro` implementa a interface `Dirigível`.
1. Crie um diagrama de classes para um sistema de e-commerce com as classes `Produto`, `CarrinhoDeCompras` e `ItemDoCarrinho`.
1. Adicione a classe `Pagamento` ao diagrama do e-commerce.
1. Modele a relação entre uma classe `Curso` e a classe `Aluno`. Considere que um curso pode ter muitos alunos.
1. Adicione um atributo estático `proximoId` à classe `Pedido`.
1. Crie um diagrama de classes para um sistema de gerenciamento de hotel com `Quarto`, `Hóspede` e `Reserva`.
1. Adicione a classe `ServiçoAdicional` (como café da manhã ou spa) ao diagrama do hotel e a relacione com `Reserva`.

---

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
