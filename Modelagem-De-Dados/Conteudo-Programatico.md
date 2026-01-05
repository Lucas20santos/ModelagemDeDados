# 🧭 Roadmap de Modelagem de Dados

## 🔰 FASE 1 — Fundamentos Sólidos (Sem Pular Etapas)

⏱️ **2 a 3 semanas**

### 🎯 Objetivo 1

Pensar como **modelador**, não como programador.

### 📚 O que estudar 1

* O que é **entidade**, **atributo** e **relacionamento**
* Cardinalidade (1:1, 1:N, N:N)
* Chave primária e estrangeira
* Normalização:

  * 1FN
  * 2FN
  * 3FN
* Diferença clara entre:

  * **Regra de negócio**
  * **Regra de sistema**

### ✍️ Prática obrigatória 1

* Modelar **no papel ou draw.io**
* Criar **DER sem banco**
* Modelar sistemas simples:

  * Escola
  * Biblioteca
  * Controle de estoque

📌 **Regra de ouro**:

> *Modelo vem antes do código.*

---

## 🔹 FASE 2 — Modelagem OLTP na Prática (Aqui você brilha)

⏱️ **3 a 4 semanas**

### 🎯 Objetivo 2

Modelar dados para **APIs e sistemas reais**.

### 📚 O que estudar 2

* Modelagem para sistemas transacionais
* Impacto da modelagem na API
* Integridade referencial
* Campos obrigatórios vs opcionais
* Soft delete vs hard delete

### 🛠️ Projetos práticos (GitHub) 2

1️⃣ **API de Vendas**

* Cliente
* Produto
* Pedido
* ItemPedido

2️⃣ **Sistema de Usuários**

* Usuário
* Perfil
* Permissões

📌 Entregáveis:

* DER
* Script SQL
* README explicando decisões de modelagem

---

## 🔸 FASE 3 — SQL para Modelagem (Não é só SELECT *)

⏱️ **2 a 3 semanas**

### 🎯 Objetivo 3

Pensar **em dados**, não em telas.

### 📚 O que estudar 3

* Joins (INNER, LEFT)
* Constraints
* Índices
* Views
* Transações
* Integridade e consistência

### 🧪 Prática 3

* Criar banco a partir do DER
* Popular dados fictícios
* Consultas respondendo perguntas do negócio

📌 Exemplo:

> “Total de vendas por mês”
> “Clientes mais ativos”

---

## ⭐ FASE 4 — Introdução ao OLAP (Noções fortes, não superficial)

⏱️ **2 semanas**

### 🎯 Objetivo 4

Entender **como dados operacionais viram análise**.

### 📚 O que estudar 4

* Diferença OLTP x OLAP
* Fato e Dimensão
* Modelo Estrela
* Granularidade
* Métricas x Dimensões

### 🛠️ Prática 4

* Transformar o banco da API em:

  * Fato_Vendas
  * Dim_Cliente
  * Dim_Produto
  * Dim_Tempo

📌 Não precisa BI agora — **só modelagem**.

---

## 🚀 FASE 5 — Portfólio Estratégico (Onde você se vende)

⏱️ **1 a 2 semanas**

### 🎯 Objetivo 5

Mostrar que você **sabe pensar dados**.

### 📁 Repositórios ideais 5

* `modelagem-api-vendas`
* `modelagem-usuarios-permissoes`
* `oltp-to-olap-modeling`

### 📄 Cada projeto deve ter

* Contexto do problema
* DER (imagem)
* Script SQL
* Explicação das decisões
* OLTP x OLAP (quando aplicável)

📌 Isso impressiona mais que código.

---

## 🧠 Como estudar (do jeito certo pra você)

Você **não precisa**:
❌ decorar teoria
❌ virar DBA
❌ estudar tudo de uma vez

Você precisa:
✅ modelar
✅ errar
✅ justificar decisões
✅ repetir

---

## 🎯 Em entrevistas, você será capaz de dizer

> “Começo entendendo o negócio, depois modelo conceitualmente, normalizo o banco para OLTP e só depois penso em código ou API.”

Isso é **nível profissional**.

---
