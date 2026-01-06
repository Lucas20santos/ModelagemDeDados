# 🧠 Exercício Prático — Modelagem Básica

## 📌 Contexto (leia com atenção)

Você vai modelar um **sistema simples de uma clínica médica**.

A clínica precisa registrar:

* Pacientes
* Médicos
* Consultas

---

## ✍️ Tarefa 1 — Identificar as **Entidades**

👉 Responda:

> **Quais são as entidades principais do sistema?**

Dica:

* Pense em *“sobre o que o sistema precisa guardar dados”*
* Use **substantivos**
* Não pense em tela ou formulário

✏️ Escreva algo como:

* Entidade 1: Pacientes - Corretas e Essenciais
* Entidade 2: Médicos - Corretas e Essenciais
* Entidade 3: Consultas - Corretas e Essenciais

---

## ✍️ Tarefa 2 — Definir **Atributos** (sem exagerar)

Para **cada entidade**, defina **apenas atributos essenciais**.

### Exemplo de formato (não é a resposta)

```md
Entidade: Exemplo
- id_exemplo
- nome
```

⚠️ Regras:

* Não coloque outra entidade como atributo
* Pense no mínimo necessário

✏️ Escreva algo como:

* Entidade 1: Pacientes - Corretas e Essenciais
  * Atributo 1: id_paciente
  * Atributo 2: nome
  * Atributo 3: altura
  * Atributo 4: peso
* Entidade 2: Médicos - Corretas e Essenciais
  * Atributo 1: id_medico
  * Atributo 2: nome
  * Atributo 3: especialização
* Entidade 3: Consultas - Corretas e Essenciais
  * Atributo 1: id_consulta
  * Atributo 2: diagnostico
  * Atributo 3: historico_paciente
  * Atributo 3: plano_tratamento

---

## ✍️ Tarefa 3 — Identificar os **Relacionamentos**

Agora responda:

* Um **paciente** pode ter quantas **consultas**?
* Um **médico** pode atender quantas **consultas**?
* Uma **consulta** está ligada a quantos pacientes?
* Uma **consulta** está ligada a quantos médicos?

✏️ Escreva no formato:

```md
Paciente 1:N Consulta
Médico 1:N Consulta
Paciente N:N Medicos
```

---

## 🚨 O que **não** fazer (importante)

❌ Não criar SQL
❌ Não pensar em banco
❌ Não normalizar
❌ Não pensar em código

👉 Aqui o foco é **raciocínio**.

---

## ✅ Resultado esperado

Ao final, você deve ter:

✔ Uma lista de entidades
✔ Atributos básicos para cada uma
✔ Relacionamentos claros (1:1, 1:N, N:N)

---

## 🧪 Desafio extra (opcional)

Explique em **1 frase**:

> “Por que Consulta é uma entidade e não um atributo?”

---
