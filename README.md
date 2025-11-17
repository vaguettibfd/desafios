# 🚀 Coleção de 10 Desafios FrontEnd (podendo ser FullStack)

**ReactJS + Ant Design + LocalStorage ou Backend + DAOs**

Este repositório reúne **10 desafios práticos completos**, projetados para reforçar habilidades em desenvolvimento front-end (e fullstack) utilizando tecnologias modernas e amplamente utilizadas no mercado.

Todos os desafios seguem um padrão comum e incluem:

- **3 CRUDs completos**, com relacionamentos entre entidades
- **1 Relatório** que combina informações de pelo menos 2 CRUDs
- **Requisitos funcionais e não funcionais padronizados**
- **Flexibilidade de armazenamento**: LocalStorage **ou** Backend (Node.js + MongoDB)
- **Uso obrigatório de DAOs**, independentemente da persistência escolhida

---

# 🧰 Tecnologias Utilizáveis

## **Frontend (obrigatório)**

- ReactJS  
- Ant Design (AntD)  
- Fetch API  
- React Router (opcional)

## **Persistência (flexível)**

### ✔ Usando LocalStorage  
- DAOs encapsulando todas as operações

### ✔ Usando Backend + MongoDB  
- Node.js, Express, Mongoose  
- DAOs integrados ao Model

---

# 📌 Requisitos Não Funcionais (Comuns)

- ReactJS + AntD obrigatórios  
- Persistência via LocalStorage **ou** backend, mas sempre com **DAOs**
- Interface **responsiva**  
- Formulários validados  
- Feedback visual (loaders, mensagens, erros)  
- Código limpo, modular e bem documentado  

---

# 🎯 Lista Completa dos 10 Desafios (com CRUDs detalhados)

## **1 — Sistema de Biblioteca Universitária**

### 📚 CRUD Livros  
- título, ano, ISBN, categoria, autorId  

### 🖋 CRUD Autores  
- nome, nacionalidade, dataNascimento  

### 🎓 CRUD Alunos  
- nome, matrícula, curso  

### 📊 Relatório  
Livros emprestados por aluno

---

## **2 — Plataforma de Cursos Online**

### 🎓 CRUD Cursos  
- título, descrição, cargaHoraria, instrutorId  

### 👨‍🏫 CRUD Instrutores  
- nome, especialidade, email  

### 🧑‍🎓 CRUD Alunos  
- nome, email, dataCadastro  

### 📊 Relatório  
Inscrições por curso e instrutor

---

## **3 — Gerenciador de Projetos e Tarefas**

### 📁 CRUD Projetos  
- nome, dataInicio, dataFim, gerenteId  

### 📝 CRUD Tarefas  
- título, status, prioridade, projetoId, colaboradorId  

### 🧑‍💼 CRUD Colaboradores  
- nome, cargo, email  

### 📊 Relatório  
Tarefas por projeto

---

## **4 — Sistema de Restaurante e Pedidos**

### 🍽 CRUD Pratos  
- nome, preço, categoria, ingredientes  

### 🧑 CRUD Clientes  
- nome, telefone, endereço  

### 🧾 CRUD Pedidos  
- clienteId, itens, data, valorTotal  

### 📊 Relatório  
Pedidos por cliente

---

## **5 — Sistema de Academia**

### 🧍 CRUD Alunos  
- nome, idade, objetivo, plano  

### 🏋 CRUD Treinos  
- alunoId, exercícios, frequência, professorId  

### 🧑‍🏫 CRUD Professores  
- nome, especialidade, registroProfissional  

### 📊 Relatório  
Treinos por professor

---

## **6 — Clínica Médica**

### 🧑 CRUD Pacientes  
- nome, cpf, dataNascimento  

### 👨‍⚕ CRUD Médicos  
- nome, especialidade, crm  

### 🩺 CRUD Consultas  
- pacienteId, medicoId, data, diagnóstico  

### 📊 Relatório  
Consultas por médico / paciente

---

## **7 — Controle de Estoque**

### 📦 CRUD Produtos  
- nome, quantidade, unidade, fornecedorId  

### 🚚 CRUD Fornecedores  
- nome, cnpj, telefone  

### 🔄 CRUD Movimentações  
- produtoId, tipo, quantidade, data  

### 📊 Relatório  
Saldo atualizado por produto

---

## **8 — Sistema de Viagens e Turismo**

### 🧳 CRUD Pacotes  
- destino, preço, dataIda, dataVolta  

### 🧑 CRUD Clientes  
- nome, email, telefone  

### 📄 CRUD Reservas  
- clienteId, pacoteId, dataReserva, valorPago  

### 📊 Relatório  
Reservas por destino

---

## **9 — Plataforma de Eventos**

### 🎤 CRUD Eventos  
- nome, local, capacidade, data  

### 🧑 CRUD Participantes  
- nome, email, telefone  

### 🎫 CRUD Ingressos  
- eventoId, participanteId, tipo, valor  

### 📊 Relatório  
Ocupação por evento

---

## **10 — Gestão Escolar**

### 🏫 CRUD Turmas  
- nome, ano, professorId  

### 👨‍🏫 CRUD Professores  
- nome, disciplina, email  

### 🧑‍🎓 CRUD Alunos  
- nome, idade, turmaId  

### 📊 Relatório  
Alunos por professor / turma

---

# 📁 Estrutura Recomendada de Pastas

``` bash
📦 projeto
 ┣ 📂 frontend
 │ ┣ 📂 src
 │ │ ┣ 📂 components
 │ │ ┣ 📂 pages
 │ │ ┣ 📂 daos        # DAOs usando LocalStorage ou fetch()
 │ │ ┣ 📂 models      # Interfaces/Classes
 │ │ ┗ App.jsx
 ┗ 📂 backend (opcional)
   ┣ 📂 models
   ┣ 📂 daos          # DAOs usando Mongoose
   ┣ 📂 controllers
   ┣ 📂 routes
   ┗ server.js
```

---

# ⚙️ Instalação e Execução

## ✔ Apenas Frontend (LocalStorage)

``` bash
cd frontend
npm install
npm run dev
```

## ✔ Com Backend (opcional)

### Backend

``` bash
cd backend
npm install
npm start
```

### Frontend

``` bash
cd frontend
npm install
npm run dev
```

------------------------------------------------------------------------

# 📄 Licença

MIT License.

------------------------------------------------------------------------

# ⭐ Observações

-   O uso de **DAOs é obrigatório**, independentemente da escolha de
    persistência.\
-   O backend é **opcional** --- mas, se usar, deve seguir o padrão
    DAO + Mongoose.

