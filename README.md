Aqui está o README atualizado com a substituição do campo `password` pelo campo `age`:

---

# 📝 API de Cadastro de Usuários

Este repositório contém uma **API de cadastro de usuários** desenvolvida para praticar o uso de **Node.js** no backend e **React** no frontend. O projeto foi criado com o objetivo de consolidar conhecimentos em desenvolvimento fullstack, utilizando ferramentas modernas como **Express**, **Prisma**, **MongoDB**, **Axios** e **Vite**.

---

## 🛠️ Tecnologias Utilizadas

### Backend
- **Node.js** com **Express**
  - API RESTful para operações de cadastro e consulta de usuários.
- **Prisma**
  - ORM utilizado para conectar e gerenciar os dados no banco **MongoDB**.

### Banco de Dados
- **MongoDB**
  - Banco NoSQL para armazenar os dados dos usuários.

### Frontend
- **React** com **Vite**
  - Interface de usuário simples e funcional para cadastro e listagem de usuários.
- **Axios**
  - Biblioteca para realizar requisições HTTP do frontend para o backend.

---

## 🎯 Funcionalidades

1. **Cadastro de Usuários**
   - Permite criar um novo usuário com informações como nome, e-mail e idade.

2. **Listagem de Usuários**
   - Exibe uma lista de todos os usuários cadastrados.

3. **Validação Simples**
   - Validação básica de dados antes de enviar para o backend.

4. **Comunicação via API**
   - O frontend utiliza **Axios** para se comunicar com o backend.

---

## 🚀 Como Executar o Projeto

### Pré-requisitos

- **Node.js** (v16 ou superior).
- **npm** ou **yarn**.
- **MongoDB** instalado ou serviço na nuvem (ex.: MongoDB Atlas).

---

### Passos para Rodar o Backend

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/api-cadastro-usuarios.git
   cd api-cadastro-usuarios/backend
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Configure o acesso ao banco de dados:
   - No arquivo `.env`, configure a variável `DATABASE_URL` com a URL do seu banco MongoDB. Exemplo:
     ```
     DATABASE_URL=mongodb+srv://usuario:senha@cluster0.mongodb.net/banco
     ```

4. Gere os arquivos do Prisma:
   ```bash
   npx prisma generate
   ```

5. Inicie o servidor:
   ```bash
   npm start
   ```
6. O backend estará disponível em `http://localhost:3000`.

---

### Passos para Rodar o Frontend

1. Navegue para o diretório do frontend:
   ```bash
   cd ../frontend
   ```

2. Instale as dependências:
   ```bash
   npm install
   ```

3. Configure o arquivo `.env`:
   - No diretório do frontend, crie um arquivo `.env` e configure o endpoint do backend:
     ```
     VITE_API_URL=http://localhost:3000
     ```

4. Inicie o servidor de desenvolvimento:
   ```bash
   npm run dev
   ```
5. O frontend estará disponível em `http://localhost:5173`.

---

## 📚 Estrutura do Projeto

```
api-cadastro-usuarios/
├── backend/          # Código do backend em Node.js com Express
│   ├── prisma/       # Configuração e esquema do Prisma
│   ├── src/          # Código fonte da API
│   └── .env          # Variáveis de ambiente para conexão ao banco
├── frontend/         # Código do frontend em React com Vite
│   ├── src/          # Código fonte da interface
│   └── .env          # Variáveis de ambiente para configurar a API
├── README.md         # Este arquivo
└── .gitignore        # Arquivos ignorados pelo Git
```

---

## 📋 Rotas da API

### **Usuários**
- **`POST /users`**: Cadastrar um novo usuário.
  - Body:
    ```json
    {
      "name": "Exemplo",
      "email": "exemplo@email.com",
      "age": "25"
    }
    ```

- **`GET /users`**: Listar todos os usuários cadastrados.

---

## 🌟 Intuito do Projeto

Este projeto foi desenvolvido como uma forma de **praticar e consolidar conhecimentos em Node.js e React**. Além disso, buscou-se aplicar as seguintes habilidades:

- Configuração e uso de **Prisma** como ORM.
- Conexão com o banco **MongoDB**.
- Criação de uma interface simples com **React**.
- Comunicação eficiente entre frontend e backend com **Axios**.
- Configuração e uso do **Vite** para melhorar a experiência no desenvolvimento frontend.

---

## 🔧 Melhorias Futuras

- Implementar autenticação de usuários.
- Adicionar validação mais robusta no backend.
- Estilizar a interface com **TailwindCSS** ou **Material-UI**.
- Implementar testes automatizados.

---

## 👥 Contribuidores

- **[Lucas Bragança Gonçalves](https://github.com/lucasbg98)**  
  Desenvolvedor Fullstack.

Contribuições são sempre bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

---
