<!-- README - AraBet | Projeto de Software -->

<a href="https://classroom.github.com/online_ide?assignment_repo_id=99999999&assignment_repo_type=AssignmentRepo"><img src="https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg" width="200"/></a> <a href="https://classroom.github.com/open-in-codespaces?assignment_repo_id=99999999"><img src="https://classroom.github.com/assets/launch-codespace-2972f46106e565e64193e422d61a12cf1da4916b45550586e14ef0a7c637dd04.svg" width="250"/></a>

---

# 🎰 AraBet — Plataforma de Apostas Esportivas 🏆

> [!NOTE]
> **AraBet** é uma plataforma online de apostas esportivas que permite a usuários cadastrados apostar em eventos ao vivo e pré-jogo, gerenciar sua carteira digital e acompanhar resultados em tempo real.

<table>
  <tr>
    <td width="800px">
      <div align="justify">
        O <b>AraBet</b> é um sistema completo de apostas esportivas desenvolvido como projeto acadêmico da disciplina <i>Projeto de Software</i>. A plataforma oferece um ecossistema integrado que cobre o ciclo completo do apostador: desde o cadastro com verificação de identidade (KYC), passando pelo gerenciamento de carteira (depósitos via Pix, cartão e transferência), até a realização de apostas em mercados esportivos ao vivo ou pré-jogo — com suporte a <b>Cash Out</b> antecipado. A documentação e arquitetura do projeto seguem as melhores práticas de <i>Engenharia de Software</i>, com modelos UML completos (Casos de Uso, Sequência, Classes, Componentes, Implantação, Comunicação, Estados e Entidade-Relacionamento), arquitetura em três camadas (SPA React, API REST Node.js, PostgreSQL + Redis) e deploy em infraestrutura AWS.
      </div>
    </td>
    <td>
      <div align="center">
        <!-- Substitua pela logo do AraBet quando disponível -->
        <img src="https://joaopauloaramuni.github.io/image/logo_ES_vertical.png" alt="Logo AraBet" width="120px"/>
      </div>
    </td>
  </tr>
</table>

---

## 🚧 Status do Projeto

[![Versão](https://img.shields.io/badge/Versão-v1.3-blue?style=for-the-badge)](https://github.com/viniciuszegarra/arabet/releases)
[![Status](https://img.shields.io/badge/Status-Documentação%20Concluída-success?style=for-the-badge)](https://github.com/viniciuszegarra/arabet)
[![Disciplina](https://img.shields.io/badge/Disciplina-Projeto%20de%20Software-orange?style=for-the-badge)](https://github.com/viniciuszegarra/arabet)
[![Node.js](https://img.shields.io/badge/Node.js-20.x-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-18.x-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Prisma](https://img.shields.io/badge/Prisma-ORM-2D3748?style=for-the-badge&logo=prisma&logoColor=white)](https://www.prisma.io/)
[![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![AWS](https://img.shields.io/badge/AWS-EC2%20%7C%20RDS%20%7C%20ElastiCache-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)](https://aws.amazon.com/)
[![Licença](https://img.shields.io/badge/Licença-MIT-green?style=for-the-badge&logo=opensourceinitiative)](./LICENSE)

---

## 📚 Índice

- [🔗 Links Úteis](#-links-úteis)
- [📝 Sobre o Projeto](#-sobre-o-projeto)
- [✨ Funcionalidades Principais](#-funcionalidades-principais)
- [🛠 Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [🏗 Arquitetura](#-arquitetura)
- [🔧 Instalação e Execução](#-instalação-e-execução)
  - [Pré-requisitos](#pré-requisitos)
  - [🔑 Variáveis de Ambiente](#-variáveis-de-ambiente)
  - [📦 Instalação de Dependências](#-instalação-de-dependências)
  - [💾 Inicialização do Banco de Dados](#-inicialização-do-banco-de-dados-postgresql)
  - [⚡ Como Executar a Aplicação](#-como-executar-a-aplicação)
  - [🐳 Execução com Docker Compose](#-execução-local-completa-com-docker-compose)
- [🚀 Deploy](#-deploy)
- [📂 Estrutura de Pastas](#-estrutura-de-pastas)
- [🎥 Demonstração](#-demonstração)
- [🧪 Testes](#-testes)
- [🔗 Documentações Utilizadas](#-documentações-utilizadas)
- [👥 Autores](#-autores)
- [🤝 Contribuição](#-contribuição)
- [🙏 Agradecimentos](#-agradecimentos)
- [📄 Licença](#-licença)

---

## 🔗 Links Úteis

* 🌐 **Demo Online:** [Acesse a Aplicação Web](https://arabet.vercel.app)
  > 💻 **Descrição:** Aplicação hospedada na Vercel (frontend) com backend na AWS EC2. Utilize credenciais de demonstração para explorar a plataforma.
* 📖 **Documentação Técnica:** [Swagger / OpenAPI](http://localhost:3333/api/docs)
  > 📚 **Descrição:** Acesso à documentação interativa de todos os endpoints REST do AraBet, gerada automaticamente via Swagger UI.
* 📄 **Documentação de Projeto:** [`/docs/AraBet_Documentacao_de_Projeto.pdf`](./docs/AraBet_Documentacao_de_Projeto.pdf)
  > 📑 **Descrição:** Documento completo de projeto com todos os diagramas UML (Casos de Uso, Sequência, Classes, Componentes, Implantação, Comunicação, Estados e DER).
* 🖼️ **Diagramas PlantUML:** [`/docs/AraBet_Diagramas.puml`](./docs/AraBet_Diagramas.puml)
  > 📐 **Descrição:** Código-fonte de todos os 13 diagramas UML do projeto, editáveis via [PlantUML Online](https://www.plantuml.com/plantuml/uml/).

---

## 📝 Sobre o Projeto

O **AraBet** nasceu da necessidade de modelar, de ponta a ponta, um sistema de software complexo com múltiplos atores, regras de negócio financeiras e integrações externas — como parte da disciplina de **Projeto de Software** do curso de Engenharia de Software.

**Por que ele existe?**
O mercado de apostas esportivas digitais é um dos segmentos de maior crescimento no Brasil pós-regulamentação. Modelar uma plataforma desse porte exige lidar com desafios reais de engenharia: consistência financeira em transações concorrentes, atualizações de dados em tempo real via WebSocket, fluxos de autenticação e autorização por perfis distintos (Apostador, Operador, Administrador) e integrações com sistemas externos críticos (gateway de pagamento, provedor de odds, serviço de e-mail).

**Qual problema ele resolve?**
Centraliza, em uma única plataforma web, todo o ciclo de vida da aposta esportiva: cadastro com KYC, gerenciamento de carteira (depósito/saque), seleção de eventos e mercados, emissão de bilhete, acompanhamento ao vivo com Cash Out e histórico completo de apostas.

**Contexto:**
Projeto acadêmico da disciplina Projeto de Software, desenvolvido com foco na produção de documentação técnica de qualidade profissional (modelos de domínio, modelos de projeto UML, modelos de dados) e na definição de uma arquitetura escalável.

> [!NOTE]
> Este projeto é uma documentação de arquitetura e modelagem — o código de produção não está incluído neste repositório. Todos os diagramas foram gerados com PlantUML e estão disponíveis no arquivo `.puml` no diretório `/docs`.

---

## ✨ Funcionalidades Principais

- 🔐 **Autenticação Segura por Perfil:** Login com JWT diferenciando Apostador, Operador e Administrador, cada um com permissões e visões distintas.
- 📝 **Cadastro com Verificação KYC:** Fluxo de registro com validação de CPF, e-mail único e verificação de identidade obrigatória para saques.
- 💳 **Gestão de Carteira Digital:** Depósitos via Pix, cartão de crédito e transferência bancária integrados ao PayGateway. Saques com aprovação administrativa.
- 🏟️ **Catálogo de Eventos e Mercados:** Painel com eventos esportivos (pré-jogo e ao vivo) e mercados de apostas com odds atualizadas em tempo real via OddsAPI.
- 🎯 **Realização de Apostas:** Seleção de evento → mercado → seleção → valor → confirmação de bilhete, com debito imediato de saldo e cálculo de ganhos potenciais.
- 📡 **Acompanhamento ao Vivo:** Stream de dados em tempo real (placar, odds dinâmicas) via WebSocket, com opção de **Cash Out** antecipado a qualquer momento.
- 🔄 **Cash Out:** Encerramento antecipado de apostas ativas com crédito parcial calculado pelo sistema conforme o momento do evento.
- 📜 **Histórico de Apostas:** Registro completo de bilhetes (ganhos, perdidos, cashout, cancelados) com filtros por status e período.
- 🛠️ **Painel Administrativo:** CRUD de eventos e mercados, moderação de usuários, aprovação de saques e verificação KYC.
- 📊 **Relatórios Financeiros:** Consolidação de depósitos, saques, volume de apostas e margem operacional da casa.
- 📨 **Notificações Automatizadas:** E-mails transacionais (confirmações de depósito, resultado de aposta, cashout) via SendGrid.
- 🔁 **Atualização de Odds em Tempo Real:** Integração automática com OddsAPI ou ajuste manual pelo Operador.

---

## 🛠 Tecnologias Utilizadas

### 💻 Front-end

* **Framework/Biblioteca:** [React 18](https://react.dev/)
* **Linguagem:** [TypeScript 5.x](https://www.typescriptlang.org/)
* **Estilização:** [Tailwind CSS](https://tailwindcss.com/)
* **Gerenciamento de Estado:** [Zustand](https://zustand-demo.pmnd.rs/)
* **Comunicação em Tempo Real:** [Socket.io Client](https://socket.io/)
* **Build Tool:** [Vite](https://vitejs.dev/)
* **Roteamento:** [React Router v6](https://reactrouter.com/)

### 🖥️ Back-end

* **Runtime:** [Node.js 20 LTS](https://nodejs.org/)
* **Framework:** [Express.js](https://expressjs.com/)
* **Linguagem:** [TypeScript 5.x](https://www.typescriptlang.org/)
* **Banco de Dados:** [PostgreSQL 16](https://www.postgresql.org/)
* **ORM:** [Prisma ORM](https://www.prisma.io/)
* **Cache / Sessões:** [Redis 7](https://redis.io/)
* **Mensageria:** [RabbitMQ](https://www.rabbitmq.com/) via AWS MQ
* **Autenticação:** JWT (JSON Web Tokens)
* **Comunicação em Tempo Real:** [Socket.io](https://socket.io/)
* **Envio de E-mails:** [SendGrid API](https://sendgrid.com/)

### ⚙️ Infraestrutura & DevOps

* **Containerização:** [Docker](https://www.docker.com/) + [Docker Compose](https://docs.docker.com/compose/)
* **Cloud:** AWS (EC2, RDS, ElastiCache, MQ, CloudFront)
* **CDN / Proxy:** AWS CloudFront + Nginx
* **CI/CD:** GitHub Actions
* **Deploy Front-end:** [Vercel](https://vercel.com/)

---

## 🏗 Arquitetura

O AraBet adota uma arquitetura em **três camadas** bem definidas, modelada com o **C4 Model** (nível de Contexto) e detalhada com diagramas UML de Componentes e Implantação:

- **Frontend (SPA - React):** Interface web responsiva com módulos de Apostas, Eventos Ao Vivo, Pagamentos e Perfil/Histórico. Comunica-se com o backend via HTTP/JSON (REST) e WebSocket.
- **Backend (API REST - Node.js/Express):** Centraliza a lógica de negócio em serviços especializados: `AuthService`, `BetService`, `EventService`, `WalletService`, `NotificationService` e `ReportService`. Utiliza **Prisma ORM** para acesso ao PostgreSQL e publica eventos em filas **RabbitMQ** para processamento assíncrono.
- **Infraestrutura de Dados:** PostgreSQL (dados relacionais), Redis (cache de odds ao vivo e sessões), RabbitMQ (fila de notificações e relatórios assíncronos).

**Padrões de Design adotados:** Repository Pattern, Service Layer, DTO, Adapter (para sistemas externos), Observer (via mensageria para notificações).

**Decisões arquiteturais importantes:**
- Uso de **UUID** como chave primária em todas as tabelas, evitando enumerações previsíveis na API pública.
- Tipos monetários declarados como `DECIMAL(15,2)` no Prisma para evitar erros de ponto flutuante IEEE 754 comuns em JavaScript.
- Cash Out e liquidação de apostas processados de forma **assíncrona** via RabbitMQ, garantindo consistência mesmo sob alta carga.

### Diagramas de Arquitetura

| Diagrama de Contexto (C4) | Diagrama de Componentes |
| :---: | :---: |
| **Visão Macro do Sistema** | **Camadas e Serviços Internos** |
| <img src="./docs/diagrams/C4_Contexto.png" alt="C4 Contexto AraBet" width="380px"> | <img src="/Diagrmas/Diagrama de componentes.png" alt="Diagrama de Componentes AraBet" width="380px"> |
| **Diagrama de Implantação (AWS)** | **Diagrama de Classes** |
| <img src="/Diagramas/Diagrama de implantacao.png" alt="Diagrama de Implantação AWS" width="380px"> | <img src="/Diagramas/Diagrama de classes.png" alt="Diagrama de Classes AraBet" width="380px"> |
| **Diagrama Entidade-Relacionamento** | **Diagrama de Casos de Uso** |
| <img src="Diagramas/DER.png" alt="DER AraBet" width="380px"> | <img src="/Diagramas/Diagrama de casos de usos.png" alt="Casos de Uso AraBet" width="380px"> |

> 📐 Todos os diagramas foram criados com **PlantUML**. O código-fonte completo está em [`/docs/AraBet_Diagramas.puml`](./docs/AraBet_Diagramas.puml).

---

## 🔧 Instalação e Execução

### Pré-requisitos

Certifique-se de ter o ambiente configurado antes de prosseguir:

* **Node.js:** Versão **20.x LTS** ou superior (necessário para backend e frontend)
* **npm:** Versão **9.x** ou superior (ou `yarn` como alternativa)
* **Docker:** Versão **24.x** ou superior (**altamente recomendado** para banco de dados e serviços)
* **Docker Compose:** Versão **2.x** (incluso no Docker Desktop)
* **Git:** Para clonar o repositório

---

### 🔑 Variáveis de Ambiente

Crie os arquivos `.env` a partir dos exemplos disponíveis em cada módulo do projeto.

#### Back-end (`/backend/.env`)

| Variável | Descrição | Exemplo |
| :--- | :--- | :--- |
| `PORT` | Porta onde a API REST será executada. | `3333` |
| `DATABASE_URL` | URL de conexão Prisma com o PostgreSQL. | `postgresql://postgres:senha@localhost:5432/arabet` |
| `REDIS_URL` | URL de conexão com o Redis. | `redis://localhost:6379` |
| `RABBITMQ_URL` | URL de conexão com o RabbitMQ. | `amqp://guest:guest@localhost:5672` |
| `JWT_SECRET` | Chave secreta para assinatura de tokens JWT. | `chave_super_segura_base64_256bits` |
| `JWT_EXPIRES_IN` | Tempo de expiração do token JWT. | `7d` |
| `PAYGATEWAY_API_KEY` | Chave de API do gateway de pagamento. | `pk_live_sua_chave_aqui` |
| `PAYGATEWAY_BASE_URL` | URL base do serviço de pagamento. | `https://api.paygateway.com/v1` |
| `ODDSAPI_API_KEY` | Chave de API do provedor de odds. | `sua_oddsapi_key_aqui` |
| `ODDSAPI_BASE_URL` | URL base da API de odds. | `https://api.the-odds-api.com/v4` |
| `SENDGRID_API_KEY` | Chave de API do SendGrid para e-mails. | `SG.sua_sendgrid_key_aqui` |
| `SENDGRID_FROM_EMAIL` | E-mail remetente das notificações. | `noreply@arabet.com.br` |

#### Front-end (`/frontend/.env`)

| Variável | Descrição | Exemplo |
| :--- | :--- | :--- |
| `VITE_API_URL` | URL base da API REST do backend. | `http://localhost:3333/api` |
| `VITE_WS_URL` | URL do servidor WebSocket. | `ws://localhost:3333` |

```bash
# Exemplo de /backend/.env
PORT=3333
DATABASE_URL="postgresql://postgres:arabet123@localhost:5432/arabet_db"
REDIS_URL="redis://localhost:6379"
RABBITMQ_URL="amqp://guest:guest@localhost:5672"
JWT_SECRET="arabet_jwt_super_secreto_256bits"
JWT_EXPIRES_IN="7d"
PAYGATEWAY_API_KEY="pk_test_sua_chave_aqui"
PAYGATEWAY_BASE_URL="https://api.paygateway.com/v1"
ODDSAPI_API_KEY="sua_oddsapi_key_aqui"
ODDSAPI_BASE_URL="https://api.the-odds-api.com/v4"
SENDGRID_API_KEY="SG.sua_sendgrid_key_aqui"
SENDGRID_FROM_EMAIL="noreply@arabet.com.br"
```

```bash
# Exemplo de /frontend/.env
VITE_API_URL=http://localhost:3333/api
VITE_WS_URL=ws://localhost:3333
```

---

### 📦 Instalação de Dependências

1. **Clone o Repositório:**

```bash
git clone https://github.com/viniciuszegarra/arabet.git
cd arabet
```

2. **Instale as dependências do Back-end:**

```bash
cd backend
npm install
cd ..
```

3. **Instale as dependências do Front-end:**

```bash
cd frontend
npm install
cd ..
```

---

### 💾 Inicialização do Banco de Dados (PostgreSQL)

O projeto utiliza **PostgreSQL 16** gerenciado via Docker e **Prisma** para migrações.

1. **Suba o banco de dados via Docker:**

```bash
docker run --name arabet_postgres \
  -e POSTGRES_USER=postgres \
  -e POSTGRES_PASSWORD=arabet123 \
  -e POSTGRES_DB=arabet_db \
  -p 5432:5432 \
  -d postgres:16
```

2. **Execute as migrações com Prisma:**

```bash
cd backend
npx prisma migrate dev --name init
```

3. **(Opcional) Rode o seed de dados de demonstração:**

```bash
cd backend
npx prisma db seed
```

---

### ⚡ Como Executar a Aplicação

Execute a aplicação em modo de desenvolvimento em **dois terminais separados**.

#### Terminal 1: Back-end (Node.js / Express)

```bash
cd backend
npm run dev
```

🚀 *A API estará disponível em **http://localhost:3333**.*
📖 *Swagger UI disponível em **http://localhost:3333/api/docs**.*

---

#### Terminal 2: Front-end (React + Vite)

```bash
cd frontend
npm run dev
```

🎨 *O Front-end estará disponível em **http://localhost:5173**.*

---

### 🐳 Execução Local Completa com Docker Compose

Para subir todo o ambiente (Backend, Frontend, PostgreSQL, Redis e RabbitMQ) de uma só vez:

1. Certifique-se de que o **Docker Desktop** (Mac/Windows) ou o serviço Docker (Linux) está em execução:

```bash
# Linux apenas
sudo systemctl start docker
```

2. Acesse a raiz do projeto e suba todos os serviços:

```bash
docker-compose up --build -d
```

> [!NOTE]
> O parâmetro `--build` garante que as imagens sejam reconstruídas com as últimas alterações. O `-d` executa em segundo plano.

3. Verifique se todos os containers estão rodando:

```bash
docker ps
```

4. Execute as migrações dentro do container do backend:

```bash
docker exec -it arabet_backend npx prisma migrate deploy
```

5. Acesse:
   - **Frontend:** http://localhost:5173
   - **API:** http://localhost:3333/api
   - **Swagger:** http://localhost:3333/api/docs
   - **RabbitMQ Management:** http://localhost:15672 (guest/guest)

6. Para parar todos os serviços:

```bash
docker-compose down
```

---

## 🚀 Deploy

### Build para Produção

```bash
# 1. Build do Front-end (React/Vite) → gera /frontend/dist
cd frontend
npm run build

# 2. Build do Back-end (TypeScript → JavaScript) → gera /backend/dist
cd ../backend
npm run build
```

### Configuração de Ambiente de Produção

> [!IMPORTANT]
> Configure as variáveis de ambiente no seu provedor de nuvem (Vercel para o frontend, AWS EC2 / Railway para o backend) antes do deploy. As variáveis críticas são: `DATABASE_URL`, `REDIS_URL`, `JWT_SECRET`, `PAYGATEWAY_API_KEY`, `ODDSAPI_API_KEY` e `SENDGRID_API_KEY`.

**Frontend (Vercel):**
```
VITE_API_URL=https://api.arabet.com.br/api
VITE_WS_URL=wss://api.arabet.com.br
```

**Backend (AWS EC2 / Docker):**
```bash
# Execução em produção via PM2 (recomendado)
npm install -g pm2
pm2 start dist/server.js --name arabet-api

# Ou via Docker
docker build -t arabet-backend .
docker run -p 3333:3333 --env-file .env.production arabet-backend
```

---

## 📂 Estrutura de Pastas

```
arabet/
├── .env.example                  # 🧩 Exemplo de variáveis de ambiente (raiz)
├── .gitignore                    # 🧹 Arquivos/pastas não versionados
├── .github/                      # 🤖 CI/CD (GitHub Actions) e templates
├── docker-compose.yml            # 🐳 Orquestração de todos os serviços
├── README.md                     # 📘 Documentação principal do projeto
├── LICENSE                       # ⚖️ Licença MIT
│
├── /docs                         # 📚 Documentação técnica completa
│   ├── AraBet_Documentacao_de_Projeto.pdf
│   ├── AraBet_Diagramas.puml     # 📐 Código-fonte dos 13 diagramas UML
│   └── /diagrams                 # 🖼️ Imagens PNG exportadas dos diagramas
│       ├── UC_AraBet.png
│       ├── Classes.png
│       ├── DER_AraBet.png
│       ├── C4_Contexto.png
│       ├── Componentes.png
│       ├── Implantacao.png
│       ├── DSS_RealizarAposta.png
│       ├── DSS_Depositar.png
│       ├── DSS_AoVivo.png
│       ├── DS_RealizarAposta.png
│       ├── DC_Depositar.png
│       ├── DE_Aposta.png
│       └── DE_Evento.png
│
├── /frontend                     # 📁 Aplicação React (SPA)
│   ├── .env.example
│   ├── Dockerfile
│   ├── vite.config.ts
│   ├── tailwind.config.ts
│   ├── /public
│   └── /src
│       ├── /components           # 🧱 Componentes reutilizáveis de UI
│       ├── /pages                # 📄 Páginas da aplicação
│       │   ├── Home/
│       │   ├── Login/
│       │   ├── Register/
│       │   ├── Events/
│       │   ├── BetSlip/
│       │   ├── LiveBetting/
│       │   ├── Wallet/
│       │   └── History/
│       ├── /services             # 🔌 Chamadas HTTP à API REST
│       ├── /hooks                # 🎣 Hooks personalizados (useAuth, useWallet, etc.)
│       ├── /store                # 🗂️ Estado global (Zustand)
│       ├── /styles               # 🎨 Estilos globais e tema
│       ├── /assets               # 🖼️ Imagens, ícones e fontes
│       └── /utils                # 🛠️ Funções utilitárias (formatação, validação)
│
├── /backend                      # 📁 API REST Node.js (Express + TypeScript)
│   ├── .env.example
│   ├── Dockerfile
│   ├── prisma/
│   │   ├── schema.prisma         # 📐 Definição do schema do banco de dados
│   │   ├── /migrations           # 📜 Histórico de migrações do banco
│   │   └── seed.ts               # 🌱 Dados iniciais de demonstração
│   └── /src
│       ├── server.ts             # 🚀 Ponto de entrada da aplicação
│       ├── /controllers          # 🎮 Endpoints REST (request/response)
│       │   ├── AuthController.ts
│       │   ├── BetController.ts
│       │   ├── EventController.ts
│       │   ├── WalletController.ts
│       │   └── ReportController.ts
│       ├── /services             # ⚙️ Regras e lógica de negócio
│       │   ├── AuthService.ts
│       │   ├── BetService.ts
│       │   ├── EventService.ts
│       │   ├── WalletService.ts
│       │   ├── NotificationService.ts
│       │   └── ReportService.ts
│       ├── /repositories         # 🗄️ Acesso a dados via Prisma
│       ├── /domain               # 🌐 Entidades e enums do domínio
│       ├── /dto                  # ✉️ Data Transfer Objects
│       ├── /adapters             # 🔌 Integrações externas (PayGateway, OddsAPI)
│       ├── /config               # 🔧 Configurações (DB, JWT, CORS, Swagger)
│       ├── /middleware           # 🛡️ Autenticação, autorização e validação
│       ├── /messaging            # 📨 Produtores e consumidores RabbitMQ
│       └── /websocket            # 📡 Servidor Socket.io para dados ao vivo
│
└── /scripts                      # 📜 Scripts utilitários
    ├── dev.sh                    # 🚀 Inicializa ambiente de desenvolvimento completo
    └── seed-events.ts            # 🏟️ Popula eventos esportivos de demonstração
```

---

### 💻 Exemplo de Saída no Terminal (API)

#### 1. Realizando uma Aposta via cURL

```bash
curl -X POST 'http://localhost:3333/api/apostas' \
     -H 'Authorization: Bearer <seu-jwt-token>' \
     -H 'Content-Type: application/json' \
     -d '{"selecaoId": "uuid-da-selecao", "valor": 100.00}'
```

**Saída Esperada:**
```json
{
  "apostaId": "a1b2c3d4-e5f6-7890-abcd-ef1234567890",
  "status": "PENDENTE",
  "selecao": "Vitória do Time A",
  "evento": "Flamengo x Palmeiras - Brasileirão",
  "oddNoMomento": 2.75,
  "valor": 100.00,
  "ganhosPotenciais": 275.00,
  "criadaEm": "2025-06-10T14:32:00.000Z"
}
```

#### 2. Verificando Saldo da Carteira

```bash
curl -X GET 'http://localhost:3333/api/carteira' \
     -H 'Authorization: Bearer <seu-jwt-token>'
```

**Saída Esperada:**
```json
{
  "saldo": 900.00,
  "moeda": "BRL",
  "atualizadoEm": "2025-06-10T14:32:05.000Z"
}
```

---

## 🧪 Testes

### Testes Unitários e de Integração

```bash
cd backend
npm run test
```
*Ferramenta: **Jest** + **Supertest** para testes de integração de endpoints REST.*

### Testes End-to-End (E2E)

```bash
cd frontend
npm run test:e2e
```
*Ferramenta: **Playwright** para testes E2E simulando fluxos completos do usuário (cadastro → depósito → aposta → cash out).*

### Cobertura de Testes

```bash
cd backend
npm run test:coverage
```

---

## 🔗 Documentações Utilizadas

* 📖 **Framework (Front-end):** [Documentação Oficial do React 18](https://react.dev/reference/react)
* 📖 **Build Tool (Front-end):** [Guia de Configuração do Vite](https://vitejs.dev/config/)
* 📖 **Estilização:** [Documentação do Tailwind CSS](https://tailwindcss.com/docs)
* 📖 **ORM (Back-end):** [Documentação Oficial do Prisma](https://www.prisma.io/docs)
* 📖 **Framework (Back-end):** [Documentação do Express.js](https://expressjs.com/)
* 📖 **Banco de Dados:** [Documentação do PostgreSQL 16](https://www.postgresql.org/docs/16/)
* 📖 **Mensageria:** [Documentação do RabbitMQ](https://www.rabbitmq.com/docs)
* 📖 **Tempo Real:** [Documentação do Socket.io](https://socket.io/docs/v4/)
* 📖 **Containerização:** [Documentação de Referência do Docker](https://docs.docker.com/)
* 📖 **Diagramas:** [PlantUML Language Reference](https://plantuml.com/sitemap-language-specification)
* 📖 **Arquitetura:** [C4 Model — Simon Brown](https://c4model.com/)
* 📖 **Padrão de Commits:** [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

---

## 👥 Autores

| 👤 Nome | :octocat: GitHub | 💼 LinkedIn | 📤 Gmail |
|---------|-----------------|-------------|-----------|
| Vinícius Zegarra Palhares | <div align="center"><a href="https://github.com/ZegarraV"><img src="https://joaopauloaramuni.github.io/image/github6.png" width="50px" height="50px"></a></div> | <div align="center"><a href="[https://www.linkedin.com/in/viniciuszegarra](https://www.linkedin.com/in/vinicius-zegarra-palhares/)"><img src="https://joaopauloaramuni.github.io/image/linkedin2.png" width="50px" height="50px"></a></div> | <div align="center"><a href="mailto:vinizegarra@gmail.com"><img src="https://joaopauloaramuni.github.io/image/gmail3.png" width="50px" height="50px"></a></div> |

---

## 🤝 Contribuição

Contribuições são bem-vindas! Para contribuir com o AraBet:

1. Faça um `fork` do projeto.
2. Crie uma branch para sua feature (`git checkout -b feature/minha-feature`).
3. Commit suas mudanças (`git commit -m 'feat: Adiciona nova funcionalidade X'`). **(Utilize [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/))**
4. Faça o `push` para a branch (`git push origin feature/minha-feature`).
5. Abra um **Pull Request (PR)** descrevendo suas alterações.

> [!IMPORTANT]
> 📝 **Regras:** Por favor, verifique o arquivo [`CONTRIBUTING.md`](./CONTRIBUTING.md) para detalhes sobre o guia de estilo de código e o processo de submissão de PRs. Certifique-se de que os testes unitários passem antes de abrir o PR.

---

## 🙏 Agradecimentos

Gostaria de agradecer às seguintes pessoas e recursos que foram fundamentais para o desenvolvimento deste projeto:

* [**Engenharia de Software PUC Minas**](https://www.instagram.com/engsoftwarepucminas/) — Pelo apoio institucional, estrutura acadêmica e fomento às boas práticas de engenharia de software.
* [**Prof. Dr. João Paulo Aramuni**](https://github.com/joaopauloaramuni) — Pelos ensinamentos sobre **Arquitetura de Software**, **Padrões de Projeto** e pela orientação na disciplina de Projeto de Software.
* [**Simon Brown — C4 Model**](https://c4model.com/) — Pela metodologia de documentação arquitetural clara e prática que norteou a modelagem deste projeto.
* [**Rodrigo Branas**](https://branas.io/) — Pela didática excepcional em **Clean Architecture** e **Clean Code**, essenciais para a organização do backend.
* [**Prisma Team**](https://www.prisma.io/) — Pela excelente documentação e pela ORM que simplificou o mapeamento objeto-relacional e as migrações de banco de dados.

---

## 📄 Licença

Este projeto é distribuído sob a **[Licença MIT](./LICENSE)**.

```
MIT License

Copyright (c) 2025 Vinícius Zegarra Palhares

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

<div align="center">
  <sub>Feito com ❤️ por <a href="https://github.com/viniciuszegarra">Vinícius Zegarra Palhares</a> — Disciplina de Projeto de Software • 2025</sub>
</div>
