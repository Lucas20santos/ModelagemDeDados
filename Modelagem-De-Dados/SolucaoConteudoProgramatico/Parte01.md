# O que é **entidade**, **atributo** e **relacionamento**

## 🧱 1️⃣ O que é **Entidade**?

👉 **Entidade é algo do mundo real que você quer representar no sistema.**

Normalmente é:

* Um **substantivo**
* Algo que **existe por si só**
* Algo que guarda informações

### 📌 Exemplos de entidades

* Cliente
* Produto
* Pedido
* Usuário
* NotaFiscal
* Funcionário

📌 Regra prática:

> **Se você consegue dizer “um / uma” antes do nome, provavelmente é uma entidade.**

Ex:

* Um **cliente**
* Um **pedido**

---

### 🧠 Pensamento de modelador

Pergunta que você faz:

> *“Sobre o que o sistema precisa guardar dados?”*

Essas respostas viram **entidades**.

---

# 🧩 2️⃣ O que é **Atributo**?

👉 **Atributo é uma característica de uma entidade.**

É:

* Um **dado**
* Uma **propriedade**
* Uma **informação específica**

### 📌 Exemplos

#### Entidade: Cliente

Atributos:

* id_cliente
* nome
* cpf
* email
* data_nascimento

📌 Regra prática:

> **Atributo responde à pergunta: “o que eu preciso saber sobre isso?”**

---

### ⚠️ Erro comum

❌ Criar atributo que é outra entidade

Ex:

* Cliente com atributo `pedido`

➡️ **Pedido é outra entidade**, não atributo.

---

# 🔗 3️⃣ O que é **Relacionamento**?

👉 **Relacionamento é como duas entidades se conectam.**

Ele responde:

> *“Como uma entidade se relaciona com a outra?”*

### 📌 Exemplos

* Cliente **faz** Pedido
* Pedido **contém** Produto
* Usuário **possui** Perfil

---

## 📐 Tipos de relacionamento (cardinalidade)

### 🔹 1 : 1

* Uma pessoa → um CPF

### 🔹 1 : N

* Um cliente → vários pedidos
* Um pedido → vários itens

### 🔹 N : N

* Um pedido → vários produtos
* Um produto → vários pedidos

📌 N:N **sempre vira uma tabela intermediária**.

---

# 🧠 Juntando tudo (exemplo completo)

### Sistema de Vendas

#### Entidades

* Cliente
* Pedido
* Produto
* ItemPedido

#### Atributos

Cliente:

* id_cliente
* nome
* cpf

Pedido:

* id_pedido
* data
* id_cliente

Produto:

* id_produto
* nome
* preco

ItemPedido:

* id_item
* id_pedido
* id_produto
* quantidade

#### Relacionamentos

* Cliente 1:N Pedido
* Pedido 1:N ItemPedido
* Produto 1:N ItemPedido

📌 Isso é **modelagem OLTP clássica**.

---

# 🚨 Erros comuns de iniciantes (importante)

❌ Criar entidade para tudo
❌ Criar atributo que representa outra entidade
❌ Não pensar em cardinalidade
❌ Modelar pensando na tela, não no negócio

---

# 🧠 Regra de ouro da modelagem

> **Entidade = o que é**
> **Atributo = o que descreve**
> **Relacionamento = como se conecta**

Se você lembrar só disso, já está à frente de muita gente.

---
