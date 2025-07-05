# 🧪 Controle de Estoque - Zoonoses

Bem-vindo ao repositório do Sistema de Controle de Estoque para Centros de Zoonoses. Este projeto foi desenvolvido para otimizar o gerenciamento de insumos, medicamentos e materiais, facilitando o controle de entradas, saídas e o inventário geral.

A aplicação é totalmente containerizada usando Docker, o que garante um ambiente de desenvolvimento e produção consistente e fácil de configurar.

---

## ✨ Tecnologias Utilizadas

Este projeto é uma aplicação full-stack que utiliza um conjunto de tecnologias modernas para garantir performance e escalabilidade:

-   **Frontend:** [React](https://reactjs.org/)
-   **Backend:** [Node.js](https://nodejs.org/) com [Express](https://expressjs.com/)
-   **Banco de Dados:** [PostgreSQL](https://www.postgresql.org/)
-   **ORM:** [Sequelize](https://sequelize.org/) para a comunicação com o banco de dados.
-   **Containerização:** [Docker](https://www.docker.com/) e [Docker Compose](https://docs.docker.com/compose/)
-   **Testes:** [Jest](https://jestjs.io/)
-   **CI/CD:** [GitHub Actions](https://github.com/features/actions)

---

## 🚀 Guia de Instalação e Execução Local

Siga estes passos para configurar e rodar o projeto completo no seu notebook.

### Pré-requisitos

Antes de começar, certifique-se de que você tem as seguintes ferramentas instaladas na sua máquina:

-   [Git](https://git-scm.com/)
-   [Docker](https://www.docker.com/products/docker-desktop/)
-   [Docker Compose](https://docs.docker.com/compose/install/) (geralmente já vem com o Docker Desktop)

### Passo a Passo

**1. Clonar o Repositório**

Primeiro, clone o projeto do GitHub para a sua máquina local.

```bash
git clone https://github.com/LeonardoPCavalcanti/controle-estoque-zoonoses.git
cd controle-estoque-zoonoses
```

**2. Subir os Contêineres com Docker Compose**

Use o Docker Compose para construir as imagens e iniciar todos os serviços.

```bash
docker compose up --build
```

-   O comando `--build` força o Docker a reconstruir as imagens caso haja alguma alteração nos `Dockerfiles`.
-   Este processo pode demorar alguns minutos na primeira vez.

**3. Acessar a Aplicação**

Após o comando terminar e os logs se estabilizarem, a aplicação estará no ar!

-   🔗 **Frontend (Interface do Usuário):** Acesse [http://localhost:3000](http://localhost:3000)
-   🔗 **Backend (API):** A API estará disponível em [http://localhost:3001](http://localhost:3001)

Para parar todos os serviços, basta pressionar `Ctrl + C` no terminal onde o `docker compose` está rodando.

💡 Dica

Para abrir o projeto diretamente no Visual Studio Code e visualizar todos os arquivos no explorador, navegue até a pasta raiz do projeto (controle-estoque-zoonoses) no seu terminal e execute o seguinte comando:

```bash
code .
```

---

## 🧪 Rodando os Testes

A API possui uma suíte de testes de integração e unidade. Para executá-los, você precisará do [Node.js](https://nodejs.org/) instalado na sua máquina.

1.  Navegue para a pasta da API:
    ```bash
    cd controle-estoque-zoonoses-api
    ```

2.  Instale as dependências de desenvolvimento:
    ```bash
    npm install
    ```

3.  Execute os testes:
    ```bash
    npm test
    ```

---