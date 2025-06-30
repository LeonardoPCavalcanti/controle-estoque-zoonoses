# 🧪 Controle de Estoque - Zoonoses

Este repositório contém a infraestrutura principal do sistema de controle de estoque para instituições de zoonoses. Ele orquestra os serviços de frontend, backend e banco de dados utilizando Docker Compose.

## 📁 Estrutura do Projeto

- `controle-estoque-zoonoses-frontend/` → Aplicação React (interface do usuário)
- `controle-estoque-zoonoses-api/` → API Node.js com Express e Sequelize
- `docker-compose.yml` → Orquestração dos serviços

## 🚀 Executando o projeto

### Pré-requisitos

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

### Passos

1. Clone o repositório:
```bash
git clone https://github.com/LeonardoPCavalcanti/controle-estoque-zoonoses.git
cd controle-estoque-zoonoses
```

2. Suba os serviços:
```bash
docker compose up --build
```

3. Acesse os sistemas:

- Frontend: [http://localhost:3000](http://localhost:3000)
- Backend (API): [http://localhost:3001](http://localhost:3001)

## 🗃 Banco de Dados

O serviço `db` utiliza PostgreSQL com os seguintes dados:

- DB: `zoonoses_estoque`
- User: `postgres`
- Senha: `postgres`

> As configurações estão no arquivo `.env` e no `docker-compose.yml`.