# 🚀 User Management Application

Esta é uma pequena aplicação full-stack para gerenciamento de usuários, permitindo cadastrar, visualizar e deletar registros.

## 🛠️ Tecnologias Utilizadas

**Frontend:**

* **React:** Biblioteca JavaScript para construção da interface de usuário.
* **Vite:** Ferramenta de build rápida para o frontend.

**Backend:**

* **Node.js:** Ambiente de execução JavaScript no servidor.
* **Express:** Framework web para Node.js.
* **JavaScript:** Linguagem de programação.
* **CORS:** Middleware para habilitar o compartilhamento de recursos entre origens diferentes.

**Banco de Dados e ORM:**

* **MongoDB:** Banco de dados NoSQL.
* **Prisma:** ORM (Object-Relational Mapper) moderno para Node.js e TypeScript.

## ⚙️ Configuração e Inicialização

Para rodar esta aplicação localmente, siga os passos abaixo.

### Pré-requisitos

Certifique-se de ter o seguinte instalado em sua máquina:

* Node.js (versão LTS recomendada)
* MongoDB (rodando localmente ou configurado com uma URI de conexão remota)

### 1. Backend (API)

Entre na pasta do seu projeto backend (ex: `api` ou `server`).

1.  **Instalar dependências:**
    ```bash
    npm install
    ```

2.  **Configurar o Banco de Dados:**
    * Crie um arquivo `.env` na raiz do backend.
    * Adicione a URI de conexão do seu MongoDB. Exemplo:
        ```env
        DATABASE_URL="mongodb+srv://<user>:<password>@<cluster>/?retryWrites=true&w=majority"
        ```
        *Ou para uma instância local:*
        ```env
        DATABASE_URL="mongodb://localhost:27017/user-db"
        ```

3.  **Gerar o Cliente Prisma:**
    ```bash
    npx prisma generate
    ```

4.  **Iniciar o Servidor:**
    ```bash
    node index.js

    ```
    O servidor da API estará rodando, por padrão, em `http://localhost:3000` (ou na porta configurada).

### 2. Frontend (Aplicação React)

Entre na pasta do seu projeto frontend (ex: `client` ou `app`).

1.  **Instalar dependências:**
    ```bash
    npm install
    ```

2.  **Iniciar o Frontend (Vite):**
    ```bash
    npm run dev
    ```
    A aplicação estará acessível, por padrão, em `http://localhost:5173` (ou na porta indicada pelo Vite).

## 💡 Funcionalidades

* ✅ **Cadastrar:** Adicionar novos usuários.
* 👀 **Visualizar:** Listar todos os usuários cadastrados.
* ❌ **Deletar:** Remover um usuário existente.
