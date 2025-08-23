# Exercicios BPMN

## 100 Exercícios sobre Modelagem de Processos de Negócio (BPMN)

### Conceitos Fundamentais (1-10)

1. Qual a diferença entre um evento de início e um evento de fim em BPMN?
1. Descreva a função de uma **Atividade (Task)**.
1. O que é um **Gateway**? Explique a diferença entre um Gateway Exclusivo e um Gateway Paralelo.
1. Qual a função de um **Pool** e de uma **Lane** em um diagrama BPMN?
1. Explique o que é um fluxo de sequência (`Sequence Flow`).
1. O que é um fluxo de mensagem (`Message Flow`) e quando ele deve ser usado?
1. Descreva um **Evento de Mensagem** de início e um de fim.
1. O que é um **Artefato** e cite dois exemplos de artefatos em BPMN.
1. Qual a diferença entre uma Tarefa e um **Sub-processo**?
1. Explique o conceito de **Token** em BPMN.

---

### Modelagem Básica (11-25)

**Modele os seguintes processos usando os elementos BPMN corretos:**

1. Um cliente faz um pedido. Um funcionário verifica o estoque. Se houver estoque, o pedido é enviado.
1. Um usuário faz login. O sistema verifica as credenciais. Se estiverem corretas, o acesso é concedido.
1. Um funcionário solicita férias. O gestor aprova ou nega o pedido.
1. O alarme de incêndio dispara. O alarme avisa a equipe e a brigada de incêndio é acionada.
1. O cliente escolhe um produto. Ele pode pagar com cartão de crédito ou por boleto. O processo termina após o pagamento.
1. Um e-mail de suporte é recebido. O sistema o classifica como "urgente" ou "normal". Um técnico lida com a solicitação.
1. Um formulário online é submetido. O sistema valida os dados. Se forem inválidos, uma mensagem de erro é exibida.
1. Um novo colaborador é contratado. Ele recebe um contrato e assina-o.
1. Um usuário solicita um reset de senha. O sistema envia um e-mail com um link para a redefinição.
1. Um produto é fabricado. Ele passa por um controle de qualidade. Se for aprovado, é embalado; se for rejeitado, é descartado.
1. O dia de pagamento chega. Os salários são processados e os depósitos são realizados.
1. Um ticket de suporte é aberto. O sistema cria um registro e envia uma notificação ao usuário.
1. Um funcionário registra horas extras. O supervisor aprova ou nega.
1. O processo de um pedido de pizza: o pedido é recebido, a pizza é preparada e a pizza é entregue.
1. Uma avaliação de produto é enviada pelo cliente. O sistema a armazena e exibe a nota na página do produto.

---

### Modelagem Intermediária (26-50)

**Modele os seguintes processos, incluindo pools e lanes:**

1. **Pedido de Compra:** Um `Cliente` envia um pedido. A `Equipe de Vendas` o recebe, verifica e envia uma confirmação ao `Cliente`.
1. **Processo de Contratação:** A `Equipe de RH` recebe um currículo. Um `Gerente` o avalia. O `Gerente` decide se o candidato vai para a entrevista.
1. **Processo de Reserva de Voo:** Um `Passageiro` busca por voos. O `Sistema de Reservas` verifica a disponibilidade. Se o voo estiver disponível, o `Passageiro` o reserva.
1. **Processo de Empréstimo:** Um `Cliente` solicita um empréstimo. O `Analista de Crédito` verifica a documentação. Se tudo estiver correto, o `Gerente do Banco` aprova o empréstimo.
1. **Processo de Suporte ao Cliente:** Um `Cliente` envia um problema. O `Atendente` o recebe. Se a solução for simples, o `Atendente` resolve. Se for complexa, ele encaminha para um `Técnico Especializado`.
1. **Processo de Envio de Mercadoria:** A `Equipe de Vendas` prepara um pedido. O `Armazém` embala o produto. A `Transportadora` coleta e entrega a mercadoria.
1. **Processo de Relatório de Despesa:** Um `Funcionário` preenche um relatório. O `Supervisor` o aprova. O `Departamento Financeiro` processa o reembolso.
1. **Processo de Publicação de Artigo:** Um `Autor` envia um artigo. O `Editor` o revisa. Se for aprovado, o `Designer` formata o artigo antes da publicação.
1. **Processo de Reclamação:** Um `Cliente` registra uma reclamação. A `Equipe de Atendimento` a recebe e a investiga. Uma resposta é enviada ao `Cliente`.
1. **Processo de Devolução:** Um `Cliente` solicita uma devolução. A `Loja` recebe o produto. O `Gerente` inspeciona o produto e autoriza o reembolso.

**Crie modelos com Gateways mais complexos:**

1. Após um pedido, o `Sistema de Pagamento` e o `Sistema de Entrega` são notificados **simultaneamente**.
1. Um ticket de suporte precisa ser revisado pelo `Técnico 1` **e/ou** pelo `Técnico 2`, dependendo da sua carga de trabalho.
1. Um novo usuário é registrado. O `Sistema` envia um e-mail de boas-vindas e, **ao mesmo tempo**, inicia o processo de validação da conta.
1. Um cliente faz um pedido. Ele é pago com cartão de crédito **ou** boleto. Após o pagamento ser confirmado, o pedido é processado.
1. Um relatório de projeto precisa ser aprovado pelo `Gerente` e pelo `Coordenador` antes de ser arquivado.
1. Após um evento de treinamento, o feedback dos participantes é coletado. Ele é enviado ao `Instrutor` e ao `Gerente do Departamento` **ao mesmo tempo**.
1. Um pedido de reserva online só pode ser confirmado após o `Sistema de Pagamento` e o `Sistema de Disponibilidade` retornarem uma resposta positiva.
1. A `Equipe de Suporte` recebe uma solicitação. O problema é resolvido **ou** a solicitação é encaminhada. Após uma dessas ações, o processo é encerrado.
1. Para se qualificar para um desconto, um cliente precisa estar inscrito na newsletter e ter feito pelo menos 3 compras anteriores.
1. Um processo de aprovação de orçamento: ele pode ser aprovado pelo `Gerente`, pelo `Diretor` **ou** pelo `Presidente`.

---

### Modelagem Avançada (51-75)

**Modele os seguintes processos usando eventos, sub-processos e exceções:**

1. Um processo de compra de passagens. O `Pagamento` deve ser concluído em até 10 minutos após a reserva. Se o tempo expirar, a reserva é cancelada.
1. O processo de registro de um novo usuário. Se ocorrer um **erro** de validação, uma mensagem de erro é exibida.
1. O processo de aprovação de um pedido de férias. O `Gestor` tem 3 dias para aprovar. Se o prazo for excedido, o pedido é **automaticamente aprovado**.
1. Modele um processo de login onde o usuário tem 3 tentativas. Se as 3 tentativas falharem, a conta é bloqueada.
1. O processo de suporte ao cliente. O cliente pode cancelar a solicitação a qualquer momento com um evento de mensagem.
1. Crie um sub-processo para o "Processo de Aprovação", que inclui as atividades de "Revisar Documentos" e "Aprovar ou Negar".
1. Modele um processo de venda de um carro, onde o sub-processo "Negociação de Preço" pode ser repetido até que um acordo seja alcançado.
1. O processo de um leilão online. O leilão dura 5 minutos. Se um lance for feito no último minuto, o temporizador é reiniciado.
1. Modele um processo onde o `Líder da Equipe` aprova uma tarefa, mas o `Gerente` pode **cancelar** a aprovação a qualquer momento.
1. Uma ordem de serviço é aberta. Se a ordem não for concluída em 7 dias, um lembrete é enviado ao técnico. Este lembrete **não interrompe** o processo.
1. Modele um processo de verificação de segurança. Se o sistema detectar uma atividade suspeita, um evento de erro é acionado.
1. Um processo de pedido de comida em um restaurante. O `Cozinheiro` pode sinalizar que um ingrediente está em falta, o que aciona um evento de erro.
1. Modele um processo de recrutamento que pode ser interrompido se o candidato recusar a oferta.
1. Modele o processo de compra de um produto, onde o cliente pode cancelar o pedido a qualquer momento antes do envio.
1. Um processo de publicação de conteúdo online. A publicação é agendada para uma data específica, mas pode ser publicada manualmente a qualquer momento antes.
1. Modele um processo que se inicia quando um arquivo é recebido e também pode ser iniciado manualmente.
1. O processo de renovação de contrato. Se a renovação não for assinada em 30 dias, um evento de compensação é acionado.
1. Modele um processo que lida com uma fatura. Se a fatura for inválida, um evento de erro é lançado e um sub-processo de "Correção de Fatura" é iniciado.
1. O processo de empréstimo bancário. Após a aprovação inicial, se a documentação do cliente não for recebida em 15 dias, o processo é cancelado.
1. Modele um processo de licitação pública, onde o processo é interrompido se todas as propostas forem consideradas inválidas.

---

### Dados e Artefatos (76-85)

1. Adicione ao exercício 11 (pedido de compra) um **Objeto de Dados** para "Pedido".
1. No exercício 15 (pagamento), adicione um **Grupo** chamado "Opções de Pagamento".
1. Adicione uma **Anotação de Texto** ao exercício 20 (controle de qualidade) para explicar o critério de rejeição.
1. Modele o processo de preenchimento de um formulário de cadastro, mostrando os **Objetos de Dados** "Formulário", "Dados do Usuário" e "Confirmação de Cadastro".
1. Adicione uma **Anotação de Texto** ao exercício 30 (suporte ao cliente) para explicar o que significa um problema "simples" ou "complexo".
1. Modele um processo onde um relatório é gerado e arquivado em um sistema. Represente o "Relatório" como um Objeto de Dados com os estados "Gerado" e "Arquivado".
1. No exercício 56, adicione um **Grupo** ao sub-processo para destacar as atividades de revisão.
1. Adicione um **Grupo** no exercício 62 (restaurante) para as atividades de cozinha.
1. Adicione **Anotações de Texto** no exercício 68 (fatura) para explicar os motivos da invalidez.
1. Modele um processo de pesquisa acadêmica, mostrando os Objetos de Dados "Dados Brutos", "Análise de Dados" e "Relatório Final".

---

### Casos de Estudo (86-100)

**Modele os seguintes processos completos e complexos:**

1. **Processo de Atendimento de Pedido Online:** Um cliente faz um pedido. O sistema de e-commerce o recebe, verifica o estoque e o pagamento (em paralelo). Se ambos estiverem ok, a ordem é enviada para o armazém. Caso contrário, o pedido é cancelado e o cliente é notificado.
1. **Processo de Lançamento de Software:** O processo se inicia quando a codificação é concluída. Um **Sub-processo de Teste** é iniciado. Se o teste falhar, um evento de erro é lançado para a equipe de desenvolvimento. Se o teste for bem-sucedido, o software é enviado para a produção e uma notificação de sucesso é enviada ao gerente.
1. **Processo de Resolução de Erro de Software:** Um **Analista de Suporte** recebe um relatório de erro. Se o erro for conhecido, o analista busca a solução. Se o erro for desconhecido, um **Sub-processo de Investigação** é iniciado, que pode levar a uma correção ou à abertura de um novo relatório de erro.
1. **Processo de Reembolso de Voo Cancelado:** O **Cliente** solicita um reembolso. A **Companhia Aérea** recebe a solicitação. Se o motivo for válido, um evento de reembolso é acionado. Se o motivo for inválido, uma notificação é enviada ao cliente. O cliente pode apelar da decisão.
1. **Processo de Onboarding de Novo Cliente:** O **Cliente** preenche um formulário. O **Representante de Vendas** o revisa. Se as informações estiverem completas, um **Sub-processo de Verificação de Crédito** é iniciado. Se a verificação for aprovada, o contrato é gerado. Se não, o processo é cancelado.
1. **Processo de Aprovação de Orçamento:** Um `Gestor de Projeto` submete um orçamento. O `Departamento Financeiro` o revisa. Se o valor for abaixo de 10k, ele é aprovado. Se for acima de 10k, a aprovação do `Diretor` é necessária.
1. **Processo de Manutenção de Equipamento:** Um **Técnico** recebe uma ordem de serviço. Ele inspeciona o equipamento. Se o problema for simples, o técnico o repara. Se for complexo, ele solicita peças de reposição.
1. **Processo de Cadastro de Fornecedor:** O processo se inicia com o recebimento de uma proposta. O **Analista de Compras** verifica a documentação. Se estiver completa, um **Sub-processo de Avaliação** é iniciado. Se o fornecedor for aprovado, ele é cadastrado no sistema.
1. **Processo de Publicação em Rede Social:** A **Equipe de Marketing** cria um post. O **Gerente** o aprova. O post é agendado para publicação. Se o gerente não aprovar em 24h, a tarefa é escalada para o `Diretor`.
1. **Processo de Compra de Imóvel:** O **Cliente** encontra um imóvel. Ele preenche uma proposta. O **Agente Imobiliário** a envia ao **Proprietário**, que pode aceitar, negar ou fazer uma contraproposta.
1. **Processo de Tratamento de Incidente de TI:** Um **Usuário** relata um incidente. O **Suporte de Nível 1** o registra e tenta resolver. Se não conseguir, ele escala para o **Suporte de Nível 2**.
1. **Processo de Entrega de Refeição:** O **Restaurante** recebe um pedido. A `Cozinha` o prepara. Um **Motoboy** é acionado e pega o pedido. Ele entrega a refeição.
1. **Processo de Ativação de Chip de Celular:** Um **Cliente** solicita um chip. O **Vendedor** o ativa no sistema. Se a ativação falhar, o processo retorna para o vendedor.
1. **Processo de Recrutamento (com múltiplos candidatos):** Modele o processo de entrevista, onde a **Equipe de RH** pode entrevistar vários candidatos simultaneamente, e a decisão final só é tomada após todas as entrevistas.
1. **Processo de Avaliação de Desempenho:** O **Funcionário** preenche um formulário de autoavaliação. Em paralelo, o **Gestor** preenche sua avaliação. O **Gestor** e o **Funcionário** se reúnem para discutir e assinar a avaliação final.
