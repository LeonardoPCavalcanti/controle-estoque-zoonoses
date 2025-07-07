# 🧪 Controle de Estoque - Zoonoses

Bem-vindo ao repositório do Sistema de Controle de Estoque para Centros de Zoonoses. Este projeto foi desenvolvido para otimizar o gerenciamento de insumos, medicamentos e materiais, facilitando o controle de entradas, saídas e o inventário geral.

A aplicação é totalmente containerizada usando Docker, o que garante um ambiente de desenvolvimento e produção consistente e fácil de configurar.

---

## ✨ Tecnologias Utilizadas

Este projeto é uma aplicação full-stack que utiliza um conjunto de tecnologias modernas para garantir performance e escalabilidade:

- **Frontend:** [React](https://reactjs.org/)
- **Backend:** [Node.js](https://nodejs.org/) com [Express](https://expressjs.com/)
- **Banco de Dados:** [PostgreSQL](https://www.postgresql.org/)
- **ORM:** [Sequelize](https://sequelize.org/) para a comunicação com o banco de dados.
- **Containerização:** [Docker](https://www.docker.com/) e [Docker Compose](https://docs.docker.com/compose/)
- **Testes:** [Jest](https://jestjs.io/)
- **CI/CD:** [GitHub Actions](https://github.com/features/actions)

---

## 🚀 Guia de Instalação e Execução Local

Siga estes passos para configurar e rodar o projeto completo no seu notebook.

### Pré-requisitos

Antes de começar, certifique-se de que você tem as seguintes ferramentas instaladas na sua máquina:

- [Git](https://git-scm.com/)
- [Docker](https://www.docker.com/products/docker-desktop/)
- [Docker Compose](https://docs.docker.com/compose/install/) (geralmente já vem com o Docker Desktop)

### Passo a Passo

**1. Clonar o Repositório**

```bash
git clone https://github.com/LeonardoPCavalcanti/controle-estoque-zoonoses.git

cd controle-estoque-zoonoses

git clone https://github.com/LeonardoPCavalcanti/controle-estoque-zoonoses-api controle-estoque-zoonoses-api

git clone https://github.com/LeonardoPCavalcanti/controle-estoque-zoonoses-frontend controle-estoque-zoonoses-frontend
```

**2. Criar banco de testes (necessário para execução dos testes)**

Abra o **PgAdmin** ou utilize outro gerenciador de banco PostgreSQL e crie um banco com o seguinte nome:

```text
zoonoses_test_db
```

Esse banco será utilizado especificamente para os testes automatizados.

**3. Subir os Contêineres com Docker Compose**

```bash
docker compose up --build
```

Esse comando inicializa:

- PostgreSQL na porta 5432.
- Backend na porta 3001.
- Frontend na porta 3000.

**4. Acessar a Aplicação**

- 🔗 **Frontend:** [http://localhost:3000](http://localhost:3000)
- 🔗 **Backend:** [http://localhost:3001](http://localhost:3001)

Para parar todos os serviços:

```bash
Ctrl + C
```

💡 **Dica:**  
Para abrir o projeto no VS Code:

```bash
code .
```

---

## 🧪 Rodando os Testes

1. Acesse a pasta da API:

```bash
cd controle-estoque-zoonoses-api
```

2. Instale as dependências:

```bash
npm install
```

3. Execute os testes:

```bash
npm test
```

---

## 💻 Rodando o Frontend isoladamente

Se quiser rodar o frontend separadamente do Docker:

1. Vá até a pasta:

```bash
cd controle-estoque-zoonoses-frontend
```

2. Instale as dependências:

```bash
npm install
```

3. Execute a aplicação:

```bash
npm run dev
```
