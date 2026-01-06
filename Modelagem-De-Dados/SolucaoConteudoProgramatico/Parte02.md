# 🔗 O que é **Cardinalidade**?

👉 **Cardinalidade define “quantos” registros de uma entidade podem se relacionar com outra.**

Ela responde perguntas como:

* Quantos A se relacionam com B?
* É obrigatório ou opcional?
* Existe limite?

---

## 📐 Tipos de Cardinalidade

Vamos ver **1:1**, **1:N** e **N:N**, sempre com:

* Definição
* Exemplo real
* Quando usar
* Erro comum

---

## 1️⃣ Cardinalidade **1 : 1** (Um para Um)

### 🔹 O que significa? 1

👉 Um registro de A se relaciona com **apenas um** de B
👉 E um registro de B se relaciona com **apenas um** de A

```md
A 1 ─── 1 B
```

---

### 📌 Exemplo clássico 1

* Pessoa ↔ CPF
* Usuário ↔ PerfilDetalhado

📌 Um CPF pertence a uma pessoa
📌 Uma pessoa tem um CPF

---

### ⚠️ Quando usar? 1

* Quando faz sentido **separar dados**
* Geralmente por:
  * Organização
  * Segurança
  * Performance
  * Responsabilidade diferente

---

### ❌ Erro comum 1

Criar 1:1 sem necessidade.

Se os dados:

* Sempre andam juntos
* Sempre são usados juntos

➡️ Podem ser **a mesma entidade**.

---

## 2️⃣ Cardinalidade **1 : N** (Um para Muitos)

### 🔹 O que significa? 2

👉 Um registro de A se relaciona com **vários** de B
👉 Um registro de B se relaciona com **apenas um** de A

```md
A 1 ─── N B
```

---

### 📌 Exemplo clássico 2

* Paciente → Consulta
* Cliente → Pedido
* Pedido → ItemPedido

📌 Esse é o **relacionamento mais comum** em sistemas.

---

### 🧠 Como identificar?

Pergunta simples:

> “Um X pode ter vários Y?”

Se sim, provavelmente é 1:N.

---

### ❌ Erro comum

Inverter o lado errado:

* Achar que Consulta → Paciente é N:1 e modelar errado

📌 Cardinalidade é **sempre pensada dos dois lados**.

---

## 3️⃣ Cardinalidade **N : N** (Muitos para Muitos)

### 🔹 O que significa?

👉 Um registro de A pode se relacionar com **vários** de B
👉 E vice-versa

```md
A N ─── N B
```

---

### 📌 Exemplo conceitual

* Aluno ↔ Disciplina
* Pedido ↔ Produto
* Médico ↔ Paciente *(conceitualmente)*

---

### 🚨 Regra de ouro

> **Relacionamento N:N NÃO existe no banco relacional.**

Ele **sempre vira uma entidade intermediária**.

---

### 🧱 Exemplo correto

```md
Pedido 1:N ItemPedido
Produto 1:N ItemPedido
```

📌 `ItemPedido` resolve o N:N.

---

## 🧠 Cardinalidade vs Obrigatoriedade (extra importante)

Além de 1, N, existe:

* **Obrigatório**
* **Opcional**

Exemplo:

* Um paciente **pode** não ter consulta ainda
* Uma consulta **deve** ter um paciente

Isso refina o modelo, mas por enquanto:
👉 Foque só em **1, N e N:N**

---

## 🧪 Exercício rápido (faça agora)

Responda **sem pensar muito**:

1️⃣ Um **médico** pode atender várias **consultas**? Sim
→ Cardinalidade? Medicos 1 : N Consulta

2️⃣ Uma **consulta** pode ter vários **pacientes**? Não
→ Cardinalidade? Pacientes 1 : 1 Consulta

3️⃣ Um **paciente** pode consultar vários **médicos ao longo do tempo**? Sim
→ Cardinalidade conceitual? Paciente N : N Medicos

---

### 1️⃣ Um **médico** pode atender várias **consultas**?

👉 **Resposta:** Sim ✅

#### ❌ Como você escreveu

```md
Consulta 1 : N Medicos
```

#### ✅ Forma correta

```md
Médico 1 : N Consulta
```

📌 Regra importante:

> A leitura da cardinalidade começa **da entidade que “possui” várias**.

* Um médico → várias consultas ✔
* Uma consulta → um médico ✔

---

### 2️⃣ Uma **consulta** pode ter vários **pacientes**?

👉 **Resposta:** Não ✅

#### ❌ Como você escreveu 2

```md
Pacientes 1 : 1 Consulta
```

#### ✅ Forma correta 2

```md
Paciente 1 : N Consulta
```

Por quê?

* Um paciente → várias consultas ✔
* Uma consulta → um paciente ✔

📌 Não é 1:1, porque o paciente pode voltar várias vezes.

---

### 3️⃣ Um **paciente** pode consultar vários **médicos ao longo do tempo**?

👉 **Resposta:** Sim ✅

#### ✔ Sua resposta conceitual

```md
Paciente N : N Médicos
```

👉 **Conceitualmente correta**, mas com um detalhe importante 👇

#### ⚠️ Ajuste profissional

Esse N:N **não aparece diretamente no modelo**.

Ele é resolvido por:

```md
Paciente 1 : N Consulta
Médico   1 : N Consulta
```

📌 **Consulta é a entidade associativa**.

---

## 🧠 Regra de ouro (anote isso)

> **Cardinalidade sempre deve ser lida como uma frase completa.**

Exemplo:

> *Um médico pode ter várias consultas.*

Se a frase fizer sentido, a cardinalidade está correta.

---

### ✅ Resumo corrigido

| Situação                       | Cardinalidade correta |
| ------------------------------ | --------------------- |
| Médico → Consulta              | Médico 1:N Consulta   |
| Paciente → Consulta            | Paciente 1:N Consulta |
| Paciente ↔ Médico (conceitual) | N:N (via Consulta)    |

---

## 📌 Resumo final (guarde isso)

> **1:1 → exclusividade**
> **1:N → hierarquia**
> **N:N → sempre vira outra entidade**

---
