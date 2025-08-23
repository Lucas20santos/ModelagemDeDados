# Exercicios de Modelagem de Dados

## Perguntas Essenciais sobre Modelagem de Dados

### Conceitos Fundamentais

1. Qual a diferença entre dados e informação?
1. O que é um modelo de dados e qual sua importância?
1. Explique os três níveis de abstração em um modelo de dados (conceitual, lógico e físico).
1. O que é um esquema de banco de dados?
1. Qual a diferença entre um SGBD e um banco de dados?

### Modelo Entidade-Relacionamento (MER)

1. O que é uma entidade e quais suas características?
1. Defina atributo. Qual a diferença entre atributo simples, composto, multivalorado e derivado?
1. O que é uma chave primária e qual sua função?
1. O que é uma chave candidata?
1. O que é uma chave estrangeira e por que ela é importante?
1. Explique os diferentes tipos de cardinalidade (1:1, 1:N, N:N).
1. O que é uma entidade fraca? Dê um exemplo.
1. Como um relacionamento N:N é representado no modelo lógico?
1. O que é uma generalização/especialização no MER?
1. O que é uma agregação?
1. Como a herança é representada em um modelo de dados relacional?
1. O que é um auto-relacionamento?
1. Qual a diferença entre a modelagem de dados e a engenharia de requisitos?
1. O que é um modelo de dados conceitual e quais são suas principais notações?
1. O que é uma supertipo e um subtipo?

---

### Normalização

1. O que é normalização e por que ela é importante?
1. Explique o conceito de redundância de dados.
1. O que é dependência funcional?
1. Explique a Primeira Forma Normal (1FN).
1. Explique a Segunda Forma Normal (2FN).
1. Explique a Terceira Forma Normal (3FN).
1. O que é a Forma Normal de Boyce-Codd (BCNF)? Quando ela deve ser usada?
1. Qual a diferença entre 3FN e BCNF?
1. O que é a Quarta Forma Normal (4FN)?
1. O que é a Quinta Forma Normal (5FN)?
1. A desnormalização é sempre uma má prática? Explique.
1. Quando a desnormalização é uma estratégia aceitável?
1. Como a normalização afeta o desempenho de consultas?
1. Qual a relação entre a normalização e a integridade dos dados?
1. Como você decide o nível de normalização adequado para um banco de dados?

---

### Modelagem Dimensional e de Data Warehouse

1. O que é um Data Warehouse?
1. Qual a diferença entre um banco de dados transacional (OLTP) e um banco de dados analítico (OLAP)?
1. Explique a diferença entre modelagem relacional e dimensional.
1. O que é uma tabela de fatos? Dê um exemplo.
1. O que é uma tabela de dimensão? Dê um exemplo.
1. O que é o modelo estrela (star schema)?
1. O que é o modelo floco de neve (snowflake schema)?
1. Qual a principal vantagem do modelo estrela sobre o floco de neve?
1. Quando você escolheria o modelo floco de neve em vez do modelo estrela?
1. O que é um atributo de dimensão degenerada?
1. O que é uma dimensão de alteração lenta (SCD)?
1. Explique os diferentes tipos de SCD (Tipo 1, Tipo 2 e Tipo 3).
1. O que é uma hierarquia em uma dimensão?
1. O que é uma medida aditiva, semi-aditiva e não-aditiva?
1. O que é um Data Mart?

---

### Tipos de Modelagem de Dados

1. O que é um modelo hierárquico?
1. O que é um modelo de rede?
1. O que é um modelo orientado a objetos?
1. Qual a diferença entre um banco de dados relacional e um NoSQL?
1. Quando a modelagem NoSQL é mais adequada?
1. Quais são os principais tipos de bancos de dados NoSQL (chave-valor, documento, coluna, grafo)?
1. O que é um banco de dados de grafo? Para que ele serve?
1. O que é um banco de dados de documentos?
1. O que é um modelo de dados temporal?
1. O que é um modelo de dados geoespacial?

---

### Integridade e Restrições

1. O que é integridade de dados?
1. Explique a integridade de entidade.
1. Explique a integridade referencial.
1. Como a integridade referencial é garantida em um banco de dados relacional?
1. O que são as restrições `ON DELETE CASCADE` e `ON DELETE RESTRICT`?
1. O que é uma restrição `CHECK`?
1. O que é uma restrição de unicidade (`UNIQUE`)?
1. Qual a diferença entre uma chave primária e uma restrição de unicidade?
1. O que é uma regra de negócio?
1. Como as regras de negócio são representadas em um modelo de dados?

---

### Ferramentas e Processo

1. Quais são as principais etapas do processo de modelagem de dados?
1. Qual o papel de um modelador de dados em uma equipe de desenvolvimento?
1. Cite três ferramentas populares de modelagem de dados.
1. O que é o Diagrama de Classes UML e como ele se relaciona com a modelagem de dados?
1. Como a modelagem de dados evolui em projetos ágeis?
1. Qual a importância da comunicação com os *stakeholders* na modelagem de dados?
1. O que é a modelagem de dados *top-down* e *bottom-up*?
1. O que é um dicionário de dados?
1. O que é um catálogo de dados?
1. Como você garante a qualidade de um modelo de dados?

---

### Cenários e Desafios

1. Como você modelaria um sistema de e-commerce? Quais entidades seriam essenciais?
1. Como você modelaria um sistema de reservas de passagens aéreas?
1. Qual a melhor abordagem para modelar dados não estruturados, como postagens em redes sociais?
1. Como a modelagem de dados lida com o conceito de "histórico"?
1. Qual o desafio de modelar dados para um sistema com alto volume de transações (ex: IoT)?
1. Como você modelaria um banco de dados para suportar múltiplas línguas?
1. O que é um antipadrão de modelagem de dados? Dê um exemplo.
1. Qual o desafio de modelar dados para um sistema que precisa de alta disponibilidade e escalabilidade?
1. Como você modelaria dados para suportar a LGPD ou outras regulamentações de privacidade?
1. Qual a diferença entre modelagem para relatórios e para transações?

---

### Modelos Avançados e Tendências

1. O que é a modelagem de dados semânticos?
1. O que é um *Knowledge Graph*?
1. Como a inteligência artificial impacta a modelagem de dados?
1. O que é *Data Mesh*? Como ele afeta a modelagem de dados?
1. Qual a diferença entre um modelo de dados lógico e um modelo conceitual?
1. O que é um metadado?
1. Como o JSON afeta a modelagem de dados em bancos de dados relacionais e NoSQL?
1. O que é a modelagem de dados *polyglot*?
1. Como a segurança dos dados é considerada na modelagem?
1. Qual o futuro da modelagem de dados na era do Big Data?
