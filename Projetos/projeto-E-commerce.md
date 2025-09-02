# Projeto de E-Commerce

## Diagrama de classe

1. Crie um diagrama de classes para um sistema de e-commerce com as classes `Produto`, `CarrinhoDeCompras` e `ItemDoCarrinho`, `Pedido` e `Cliente`.
    - Caracteristicas do Cliente:
        - **Atributos(Propriedades)**
            - **Informações de Conta**:
                - `id_cliente`: um identificador único para o cliente.
                - `nome`: Nome completo do cliente.
                - `email`: O e-mail usado para login e comunicação.
                - `senha_hash`: A senha criptogafada do cliente (nunca armazene a senha em texto simples)
            - **Histórico e Localização**:
                - `enderecos`: Uma lista de objetos `Endereco` associados ao cliente.
                - `historico_pediso`: Uma lista de objetos `Pedido` que o cliente já realizou.
        - **Métodos(Comportamentos)**
            - `autenticar(senha_senha)`: Verifica se a senha fornecidad corresponde à senha armazenada.
            - `mudar_senha(nova_senha)`: Permite que o cliente altere seu nome, e-mail, etc.
            - `mudar_senha(nova_senha)`: Altera a senha do cliente.
            - `obter_historico_pedidos()`: Retorna a lista de todos os pedidos feitos pelo cliente.
            - `adicionar_endereco(novo_endereco)`: Adiciona um novo endereço de entega ou faturamento.
    - Caracteristicas do Pedido:
        - **Atributos(Propriedades)**:
            - **Identificação:**
                - `id_pedido`: Um identificar único para o pedido.
                - `data_pedido`: A data e a hora em que o pedido foi finalizado
            - **Relação com o cliente**:
                - `id_cliente`
            - **Valores e Pagamentos**:
                - `valor_subtotal`: O valor total dos itens antes de taxas e frete
                - `valor_frete`: O custo do envio.
                - `valor_desconto`: O valor total de descontos aplicados.
                - `valor_total`: O valor final do pedido.
                - `status_pagamento`: O estado do pagamentos (ex: `pendente`, `aprovado`, `rejeitado`).
            - **Logistica e Entrega**:
                - `endereco_entrega`: O endereço para onde o pedio será enviado.
                - `status_envio`: O estado da entrega (ex: `processando`, `enviado`, `entregue`)
                - `codigo_rastreio`: O código para rastrear o envio.
            - **Conteúdo**:
                - `itens`: Uma lista de objetos `ItemDoPedido`, que registram o `Produto` e a `quantidade` comprada, com o preço fixado no momento da compra.
        - **Métodos(Comportamentos)**: Os métodos definem o que um pedido **faz**
            - `atualizar_status_pagamentos(novo_status)`: Altera o estado do pagamento.
            - `atualizar_status_envio(novo_stauts)`: Altera o estado do envio.
            - `obter_valor_total()`: Retorna o valor final do pedido.
            - `cancelar_pedido()`: Cancela o pedido (se as regra de negócio permitirem).
            - `gerar_nota_fiscal()`: Cria um documento fiscal a partir dos dados do pedido.
    - Caracteristicas de produto:
        - **Atributos(Propriedades)**:
            - **Identificação**:
                - `id`: Um identificador único e interno para o sistema
                - `sku`: (Stock Keeping unit): Um código único do  produto, usado apra controle de estoque
                - `ean`: (European Article Number) ou upc (Universal Product Code): Códigos de barras universais.
            - **Descrição**:
                - `nome`: O nome completo do produto.
                - `descricao`: Uma descriçaõ detalhada do produto.
                - `marca`: A marca ou fabricante do produto.
                - `categoria`: A categoria à qual o produto pertence (ex: "Eletrônicos", "Moda").
                - `tags`: Uma lista de palavras-cheve para pesquisa.
            - **Valores e Preco**:
                - `preco`: O preço de venda original do produto.
                - `preco_promocional`: O preço reduzido, se houver uma promoção.
                - `data_inicio_promocao`: Data emque a promoção começa.
                - `data_fim_promocao`: Data em que a promoção termina.
            - **Estoque**:
                - `quantidade_em_estoque`: O número de unidades disponível.
                - `disponível`: Um booleano que indica se o produto está em estoque ou não.
            - **Informações Visuais e de Midia**:
                - `url_imagem_principal`: Link para a imagem principal do produto.
                - `url_imagens_adicionais`: Uma lista de links para imagens secundárias ou galeria de fotos.
            - **Avaliação e Feedback**:
                - `media_avaliacao`: A nota média atribuída pelos clientes
                - `numero_avaliações`: A contagem de quatnas avaliações o produto recbeu.
        - **Métodos(Comportamentos)**:
            - `obter_preco_final()`: calcula o proeco de vendo, considerando promoções ou descontos aplicados.
            - `verificar_disponibilidade()`: Retorna um valor booleando baseado na quantidade em estoque
            - `adicionar_estoque(quantidade)`: Aumenta a quantidade em estoque do produto.
            - `remover_estoque(quantidades)`: Diminui a quantidade em estoque após uma venda.
            - `adicionar_avaliação(nota, comentario)`: Atualiza a nota média e o número de avaliações.
            - `obter_detalhes_completos()`: Retorna todas as informações do produto, incluindo imagens e descrições.

    - Carrinho de Compras:
        - Atributos:
            - **Identificação**:
                - `id_carrinho`: Um identificador único para o carrinho.
                - `id_cliente`: Um identificador para o cliente, associando o carrinho a uma conta.
            - **Conteúdo**:
                - `itens`: Uma lista ou coleção de objetos ItemDoCarrinho. Está é apropriedade masi importante, pois cada ItemDocarrinho é uma classe auxiliar que armazena a referência a um Produto e a quantidade desejada.
            - **Estado e Valores**:
                - `status`: O estado atual do carrinho (ex: ativo, finalizado, abandonado).
                - `valor_subtotal`: O valor total dos intens antes de descontos e taxas.
                - `valor_desconto`: O valor total de descontos aplicados.
                - `valor_total`: O valor final a ser pago, após todos os cálculos.
            - Timestamps:
                - `data_criacao`: A data em que o carrinho foi criado.
                - `data_ultima_atualização`: A data da última vez que um item foi adicionado ou removido.
        - **Métodos**: Os métodos definem o que um carrinho **faz**.
            - `**adicionar_item(produto, quantidade)`: Adiciona um produto à lista de itens do carrinho. Se o produto já estiver no carrinho, atualiza a quantidade.
            - `remover_item(produto)`: Remove um produto do carrinho.
            - `atualizar_quantidade(produto, nova_quantidade)`: Altera a quantidade de um produto específico.
            - `calcular_subtotal()`: Recalcular o valor dos itens no carrinho. Este método é geralmente chamado após qualquer alteração no conteúdo do carrinho.
            - `aplicar_cupon(codigo)`: Adiciona um cupon de desconto, que afeta o cálculo do valor total.
            - `obter_valor_total()`: Retorna o valor finla, considerando subtotal e descontos.
            - `limpar_carrinho`: Remove todos os itens do carrinho, geralmente após a finalização da compra.
            - `finalizar_compra()`: inicia o processo de checkout e, geralmente, cria uma nova instânica da classe `Pedido` a partir dos dados do carrinho.
    - IntemDoCarrinho:
        - `nome`:
        - `quantidade`:
        - `preco_unitario`:

## Relacionamentos entre as classes

### Passo 1: A Conexão Direta entre Cliente e CarrinhoDeCompras

O CarrinhoDeCompras é o primeiro ponto de contato entre o cliente e os produtos que ele deseja adquirir.

- Relação: O Cliente usa/tem um CarrinhoDeCompras.
- Cardinalidade:
  - Um Cliente pode ter 0 ou 1 CarrinhoDeCompras ativo a qualquer momento (um cliente não tem dois carrinhos ao mesmo tempo).
  - Um CarrinhoDeCompras pertence a exatamente 1 Cliente.
- Tipo de Relacionamento: Associação simples. É uma relação de "um para um".

### Passo 2: Como o CarrinhoDeCompras e o Pedido se Conectam aos Produtos

Um `CarrinhoDeCompras` e um `Pedido` não se conectam diretamente ao `Produto`. Eles precisam de uma classe intermediária para registrar a quantidade de cada produto, já que a relação é de "muitos para muitos":

- Um carrinho tem muitos produtos.
- Um produto pode estar em muitos carrinhos.

A solução é usar classes auxiliares, que carregam as informações específicas de cada transação.

- ItemDoCarrinho: Esta classe é criada para registrar a quantidade de um produto específico em um CarrinhoDeCompras.
- ItemDoPedido: Esta classe registra a quantidade de um produto específico em um Pedido, mas também armazena o preço do produto no momento da compra (para evitar problemas caso o preço mude depois).

#### Relacionamento: `CarrinhoDeCompras` com `ItemDoCarrinho` e `Produto`

- `CarrinhoDeCompras` -> `ItemDoCarrinho`: A relação é de Composição. O `ItemDoCarrinho` não pode existir sem o `CarrinhoDeCompras` ao qual pertence. Se o carrinho for esvaziado ou excluído, o item também é.
  - Cardinalidade: Um `CarrinhoDeCompras` tem 0 ou muitos `ItemDoCarrinho`. Um `ItemDoCarrinho` pertence a exatamente um CarrinhoDeCompras.
- `ItemDoCarrinho` -> `Produto`: A relação é de Associação simples. O `ItemDoCarrinho` apenas se refere a um Produto. O Produto pode continuar a existir mesmo que não esteja em nenhum carrinho.
- Cardinalidade: Um `ItemDoCarrinho` está associado a exatamente 1 `Produto`. Um `Produto` pode estar em 0 ou muitos `ItemDoCarrinho`.

#### Relacionamento: `Pedido` com `ItemDoPedido` e `Produto`

- `Pedido` -> `ItemDoPedido`: A relação é de Composição. O `ItemDoPedido` não pode existir sem o `Pedido` ao qual pertence. Se um pedido for cancelado, os itens dele também perdem sua existência no sistema.
  - Cardinalidade: Um `Pedido` tem 1 ou muitos `ItemDoPedido` (um pedido precisa ter pelo menos um item). Um `ItemDoPedido` pertence a exatamente 1 `Pedido`.
- `ItemDoPedido` -> `Produto`: A relação é de Associação simples. O `ItemDoPedido` se refere a um `Produto` do catálogo.
  - Cardinalidade: Um `ItemDoPedido` está associado a exatamente 1 `Produto`. Um `Produto` pode estar em 0 ou muitos `ItemDoPedido`.

### Passo 3: O Relacionamento Final entre `Cliente` e `Pedido`

O `Pedido` é a materialização da compra. Ele é um registro do que foi comprado, quando e por quem.

- Relação: O `Cliente` faz um `Pedido`.
- Cardinalidade:
  - Um `Cliente` pode ter 0 ou muitos `Pedidos` ao longo do tempo (seu histórico de compras).
  - Um `Pedido` pertence a exatamente 1 `Cliente`.
- Tipo de Relacionamento: Associação simples. É uma relação de "um para muitos".

### Diagrama Final de Classes

Aqui está o diagrama completo, unindo todos os relacionamentos que acabamos de discutir.
