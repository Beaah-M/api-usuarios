# Cadastro de Usuário - API (Back-End)

Esta é a API do sistema de cadastro de usuários, desenvolvida com **Node.js**, **Express** e **Prisma ORM**. Ela é responsável por armazenar, buscar, atualizar e excluir dados de usuários em um banco de dados relacional.

## 🔧 Funcionalidades

- **GET /usuarios** – Retorna a lista de usuários cadastrados.
- **POST /usuarios** – Cadastra um novo usuário.
- **PUT /usuarios/:id** – Atualiza os dados de um usuário.
- **DELETE /usuarios/:id** – Remove um usuário do banco.
- **Timestamps** – Guarda data de criação e atualização automática via Prisma.

## 🛠️ Tecnologias Utilizadas

- **Node.js** – Ambiente de execução JavaScript.
- **Express** – Framework para criação da API.
- **Prisma ORM** – Acesso ao banco de dados com tipagem.
- **SQLite ou PostgreSQL** – Armazenamento dos dados.
- **Render** – Plataforma para deploy da API.

## 📁 Estrutura do Projeto

- `index.js` – Ponto de entrada da aplicação.
- `prisma/schema.prisma` – Modelo do banco de dados.
- `.env` – Variáveis de ambiente como `DATABASE_URL`.

## 🚀 Como rodar localmente

```bash
git clone https://github.com/seu-usuario/api-cadastro-usuarios.git
cd api-cadastro-usuarios
npm install
npx prisma generate
npx prisma migrate dev --name init
node index.js
