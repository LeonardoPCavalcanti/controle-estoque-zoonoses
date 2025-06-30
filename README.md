# 🦠 Sistema de Controle de Estoque para Zoonoses

Este repositório centraliza os subprojetos do sistema de controle de estoque para zoonoses, facilitando a configuração e execução com Docker.

## 📦 Subprojetos

- 🔙 **Backend (API)**  
  Repositório: [controle-estoque-zoonoses-api](https://github.com/SEU_USUARIO/controle-estoque-zoonoses-api)

- 🎨 **Frontend (Interface Web)**  
  Repositório: [controle-estoque-zoonoses-frontend](https://github.com/SEU_USUARIO/controle-estoque-zoonoses-frontend)

> ⚠️ Substitua `SEU_USUARIO` acima pelo seu nome de usuário do GitHub.

---

## 🚀 Executando com Docker Compose

### 1. Clone os repositórios

```bash
git clone https://github.com/SEU_USUARIO/controle-estoque-zoonoses-api.git
git clone https://github.com/SEU_USUARIO/controle-estoque-zoonoses-frontend.git
```

> Coloque ambos os diretórios clonados na **mesma pasta deste repositório**, para que o Docker Compose funcione corretamente.

### 2. Execute o sistema

```bash
docker-compose up --build
```

---

## ⚙️ Serviços

- `backend` → Porta 3001
- `frontend` → Porta 3000
- `db` (PostgreSQL) → Porta 5432

---

## 🧪 Tecnologias

- TypeScript
- Node.js / Express
- React / Vite
- PostgreSQL
- Docker e Docker Compose

---

## 📂 Estrutura esperada

```
controle-estoque-zoonoses/
├── docker-compose.yml
├── controle-estoque-zoonoses-api/
└── controle-estoque-zoonoses-frontend/
```

---
