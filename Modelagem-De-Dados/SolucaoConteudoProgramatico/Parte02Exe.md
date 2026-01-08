# 🧠 Exercícios — Cardinalidade

## 🟢 Exercício 1 — Responda rapidamente (Sim / Não + Cardinalidade)

1️⃣ Um **cliente** pode fazer vários **pedidos**?
→ Cardinalidade? cliente 1 : N pedidos

2️⃣ Um **pedido** pode conter vários **produtos**?
→ Cardinalidade? pedido 1 : N produtos

3️⃣ Um **produto** pode aparecer em vários **pedidos**?
→ Cardinalidade? produto 1 : N pedidos

- pedidos é a entidade associativa entre cliente e produtos
- o cliente faz um pedido de vários produtos

---

### ✅ Exercício 1 — Correção Comentada

#### 1️⃣ Cliente → Pedidos

Você respondeu:

```yarm
cliente 1 : N pedidos
```

✔ **Correto.**
Um cliente pode fazer vários pedidos.

👉 Forma correta:

```yarm
Cliente 1 : N Pedido
```

---

#### 2️⃣ Pedido → Produtos

Você respondeu:

```yarm
pedido 1 : N produtos
```

⚠️ **Parcialmente correto**, mas incompleto.

Por quê?

Sim: Um pedido pode ter vários produtos.
Mas também é verdade que:

→ Um produto pode estar em vários pedidos.

Logo, a relação correta ENTRE PEDIDO e PRODUTO não é 1:N.

#### A relação é

```yarm
Pedido N : N Produto
```

Esse é exatamente o motivo de existir **ItemPedido**.

---

## 3️⃣ Produto → Pedidos

Você respondeu:

```yarm
produto 1 : N pedidos
```

⚠️ Essa resposta “espelha” a anterior, mas também incorreta.

Um produto não pertence a apenas 1 pedido — ele pode aparecer em muitos pedidos.

Logo:

```yarm
Produto N : N Pedido
```

---

### 🧱 Correção final do conjunto

#### ⭐ Relações verdadeiras

```yarm
Cliente 1:N Pedido
Pedido N:N Produto
```

#### ⭐ E sim, você acertou o raciocínio

> “Pedidos é a entidade associativa entre cliente e produtos.”

PERFEITO!
Isso mostra que você **entendeu o papel da entidade associativa**.

---

#### 🎯 Avaliação Geral

| Item                                  | Nota                                  |
| ------------------------------------- | --------------------------------      |
| Entendimento conceitual               | ⭐⭐⭐⭐⭐                            |
| Identificação de entidade associativa | ⭐⭐⭐⭐⭐                            |
| Expressão correta de cardinalidade    | ⭐⭐⭐☆☆ (precisa só ajustar forma)   |

Você está **muito no caminho certo** — agora só falta escrever a cardinalidade com a precisão técnica correta.

---

## 🟢 Exercício 2 — Leia e defina a cardinalidade

Considere um **sistema escolar**:

4️⃣ Um **aluno** pode estar matriculado em várias **disciplinas**?
→ Cardinalidade? Sim -> Aluno 1 : N Disciplinas

5️⃣ Uma **disciplina** pode ter vários **alunos**?
→ Cardinalidade? Sim Disciplinas 1 : N Alunos

6️⃣ Qual é a cardinalidade **entre Aluno e Disciplina**? Alunos N : N Diciplinas

- A sala de aula seria a entidade associativo entre alunos ou ItemDeEstudo

---
Vamos corrigir **com muito cuidado**, porque aqui você fez **quase tudo certo**, mas cometeu um pequeno erro importante no item sobre a sala de aula.

---

### ✅ Correção do Exercício 2

#### 4️⃣ Um **aluno** pode estar matriculado em várias **disciplinas**?

✔ **Sim**
→ **Aluno 1 : N Disciplinas**

#### 5️⃣ Uma **disciplina** pode ter vários **alunos**?

✔ **Sim**
→ **Disciplina 1 : N Alunos**

### 6️⃣ Qual é a cardinalidade **entre Aluno e Disciplina**?

✔ **N : N**
→ Porque cada aluno pode ter várias disciplinas
→ E cada disciplina pode ter vários alunos

Até aqui, tudo PERFEITO. 👏🔥

---

### ❗ Correção da sua conclusão sobre *entidade associativa*

Você escreveu:

> A sala de aula seria a entidade associativo entre alunos ou ItemDeEstudo

Isso **não está correto**, e aqui está a explicação clara:

---

### ✅ A entidade associativa entre Aluno e Disciplina é **Matrícula**

Por quê?

- “Sala de aula” **não resolve** o relacionamento N:N
- “ItemDeEstudo” não faz sentido no contexto

Para transformar **N:N → 1:N + 1:N**, criamos a entidade associativa:

#### ✔ Entidade Associativa: **Matrícula**

Ela representa o ato do aluno se matricular em uma disciplina.

#### Estrutura correta

**Aluno** 1:N **Matrícula** N:1 **Disciplina**

#### Atributos típicos da entidade associativa *Matrícula*

- data_matricula
- situação (ativa, trancada, cancelada)
- nota_final (em alguns sistemas)
- frequência

---

### 💡 Por que não é Sala de Aula?

Porque:

- Uma sala não representa a relação **Aluno–Disciplina**
- Uma sala pode ter aulas de várias disciplinas
- Um aluno não “se relaciona” com a sala, e sim com a disciplina e horário

Sala é apenas um **recurso físico**, não uma relação conceitual.

---

### 🎯 Conclusão Final

✓ Você acertou as cardinalidades
✓ Acertou que Aluno–Disciplina é N:N
✗ Só errou a entidade associativa
→ A correta é **Matrícula**, não Sala

## 🟢 Exercício 3 — Verdadeiro ou Falso (justifique mentalmente)

7️⃣ “Uma **consulta médica** sempre está ligada a exatamente **um médico**.”
→ Verdadeiro ou Falso? Sim
→ Cardinalidade? Medico 1 : N Consultas

8️⃣ “Um **médico** pode não ter nenhuma **consulta**.”
→ Verdadeiro ou Falso? Sim
→ Cardinalidade possível? Medico 0 : N Consulta

---

## 🟢 Exercício 4 — Identifique o erro

Analise a frase:

9️⃣

```md
Paciente 1 : 1 Consulta
```

Essa cardinalidade está correta?
Se não, qual seria a correta?

---

## 🟢 Exercício 5 — Desafio conceitual (importante)

10️⃣ Complete a frase corretamente:

> “Quando duas entidades têm relação **N:N**, geralmente existe uma terceira entidade que representa __________.”

---

## 📌 Regras do exercício

✔ Use frases para pensar
✔ Leia a relação dos dois lados
✔ Não crie tabelas
✔ Não pense em SQL

---
