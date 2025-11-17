# 🚀 Coleção de 10 Desafios FrontEnd (podendo ser FullStack)

**ReactJS + Ant Design + LocalStorage ou Backend + DAOs**

Este repositório reúne **10 desafios práticos completos**, projetados
para reforçar habilidades em desenvolvimento front-end (e fullstack)
utilizando tecnologias modernas e amplamente utilizadas no mercado.

Todos os desafios seguem um padrão comum e incluem:

-   **3 CRUDs completos**, com relacionamentos entre entidades.\
-   **1 Relatório** que combina informações de pelo menos 2 CRUDs.\
-   **Requisitos funcionais e não funcionais padronizados**.\
-   **Flexibilidade de armazenamento**: LocalStorage **ou** Backend
    (Node.js + MongoDB).\
-   **Uso obrigatório de DAOs**, independentemente do tipo de
    persistência.

Ideal para estudos, avaliações técnicas, desafios acadêmicos e
construção de portfólio.

------------------------------------------------------------------------

# 🧰 Tecnologias Utilizáveis

### **Frontend (obrigatório)**

-   ReactJS\
-   Ant Design (AntD)\
-   Fetch API (quando houver backend)\
-   React Router (opcional e recomendado)

### **Persistência (flexível)**

Você pode implementar o desafio de duas formas:

### ✔ **1. Usando LocalStorage (sem backend)**

-   Persistência feita no navegador\
-   DAOs implementados encapsulando operações de leitura/escrita no
    localStorage

### ✔ **2. Usando Backend + MongoDB (opcional)**

-   Node.js\
-   Express\
-   Mongoose\
-   Banco MongoDB local ou em nuvem\
-   DAOs implementados como classes responsáveis pela comunicação com o
    Model Mongoose

------------------------------------------------------------------------

# 📌 Requisitos Não Funcionais (Comuns a Todos os Desafios)

### **Tecnologias e Arquitetura**

-   Frontend em **ReactJS** com **Ant Design**.\
-   Persistência de dados via **LocalStorage** ou via **Backend**, mas
    **sempre** utilizando **DAOs** para separar regras de domínio da
    persistência.\
-   Comunicação com backend via **fetch()**, quando existir.\
-   Estrutura modular: componentes, páginas, serviços, DAOs, modelos.

### **Usabilidade**

-   Interface totalmente **responsiva** (desktop e mobile).\
-   Formulários validados.\
-   Feedback visual (mensagens, loaders, estados de erro).\
-   Boa organização e navegação intuitiva.

### **Qualidade e Organização**

-   DAOs obrigatórios (mesmo usando LocalStorage).\
-   Separação de responsabilidades:
    -   Componentes → interface\
    -   Serviços → lógica\
    -   DAOs → persistência\
-   Tratamento consistente de erros.\
-   Código limpo, reutilizável e bem documentado.

------------------------------------------------------------------------

# 🎯 Lista Resumida dos 10 Desafios

## 1 --- Sistema de Biblioteca Universitária

CRUDs: Livros, Autores, Alunos\
Relatório: Livros emprestados por aluno

## 2 --- Plataforma de Cursos Online

CRUDs: Cursos, Instrutores, Alunos\
Relatório: Inscrições por curso/instrutor

## 3 --- Gerenciador de Projetos e Tarefas

CRUDs: Projetos, Tarefas, Colaboradores\
Relatório: Tarefas por projeto

## 4 --- Sistema de Restaurante / Pedidos

CRUDs: Pratos, Clientes, Pedidos\
Relatório: Pedidos por cliente

## 5 --- Sistema de Academia

CRUDs: Alunos, Treinos, Professores\
Relatório: Treinos por professor

## 6 --- Clínica Médica

CRUDs: Pacientes, Médicos, Consultas\
Relatório: Consultas por médico/paciente

## 7 --- Controle de Estoque

CRUDs: Produtos, Fornecedores, Movimentações\
Relatório: Saldo atualizado por produto

## 8 --- Sistema de Viagens e Turismo

CRUDs: Pacotes, Clientes, Reservas\
Relatório: Reservas por destino

## 9 --- Plataforma de Eventos

CRUDs: Eventos, Participantes, Ingressos\
Relatório: Ocupação por evento

## 10 --- Gestão Escolar

CRUDs: Turmas, Professores, Alunos\
Relatório: Alunos por professor

------------------------------------------------------------------------

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

------------------------------------------------------------------------

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
