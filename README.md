# 🚀 NLW Agents - Rocketseat

Projeto desenvolvido durante a **20ª edição do NLW** da [Rocketseat](https://rocketseat.com.br/), com foco em **Inteligência Artificial com Agentes Autônomos**, aplicando conceitos modernos para construir sistemas que **pensam, planejam e agem** para resolver problemas reais.

## 🧠 Sobre o Projeto

> **Let Me Ask IA**

Aplicação inteligente com capacidade de tomada de decisões em tempo real, integração com IA e arquitetura escalável.

### Principais funcionalidades:

* Agente autônomo com tomada de decisão em tempo real
* Integração com API do **Gemini AI**
* Interface moderna e interativa
* Backend robusto com validação e controle de fluxo
* API performática e segura com Fastify

---

## 🚀 Tecnologias Utilizadas

### 🧩 Backend

* **Node.js** com **TypeScript** (`--experimental-strip-types`)
* **Fastify** – Web framework rápido e eficiente
* **PostgreSQL** com extensão **pgvector** (para vetores IA)
* **Drizzle ORM** – Operações seguras e tipadas no banco
* **Zod** – Validação de schemas
* **Docker** – Containerização do banco de dados
* **Biome** – Lint e formatação de código

### 🎨 Frontend

* **React**
* **Vite**
* **TailwindCSS**
* **TypeScript**

---

## 🏗️ Arquitetura

* Separação clara entre rotas, serviços, schemas e banco
* Schema validation com **Zod**
* ORM type-safe com **Drizzle**
* Variáveis de ambiente validadas de forma centralizada
* Projeto escalável e modularizado

---

## 🧪 Aprendizados e Desafios

* Integração com LLMs (Modelos de Linguagem)
* Arquitetura de agentes autônomos
* Práticas modernas com React + Node.js
* Foco em performance e usabilidade

---

## ⚙️ Como rodar o projeto localmente

### Pré-requisitos

* Node.js (versão compatível com `--experimental-strip-types`)
* Docker + Docker Compose

### Passo a passo

```bash
# Clone o repositório
git clone https://github.com/Hebert324/nlw-agents

# Acesse a pasta do projeto
cd nlw-agents
```

#### Backend

```bash
# Suba o banco de dados com Docker
docker-compose up -d

# Configure as variáveis de ambiente
touch .env
```

Exemplo de `.env`:

```env
PORT=3333
DATABASE_URL=postgresql://docker:docker@localhost:5432/agents
```

```bash
# Instale as dependências
npm install

# Execute as migrações
npx drizzle-kit migrate

# (Opcional) Popule o banco com dados de exemplo
npm run db:seed

# Inicie o servidor de desenvolvimento
npm run dev
```

#### Produção:

```bash
npm start
```

---

## 📚 Scripts Disponíveis

* `npm run dev` – Inicia o servidor em modo desenvolvimento com hot reload
* `npm start` – Executa o projeto em modo produção
* `npm run db:seed` – Popula o banco com dados de exemplo

---

## 🌐 Endpoints da API

A API ficará disponível em: `http://localhost:3333`

* `GET /health` – Health check da aplicação
* `GET /rooms` – Lista as salas disponíveis

---

## 💡 Créditos

Desenvolvido com ❤️ durante o **NLW da Rocketseat**
Por [Hebert](https://github.com/Hebert324)

---
