# 🧠 NLW Agents

Projeto full stack desenvolvido durante o evento **Next Level Week (NLW)** da Rocketseat.  
O sistema permite interagir com uma **IA de sugestão de mensagens**, com um backend rápido usando **Fastify** e **PostgreSQL + pgvector**, e um frontend moderno feito em **React + Vite + Tailwind**.

---

## 📦 Repositórios

- 🔗 Backend: [NLW-Agents-Server](https://github.com/IgorBern02/NLW-Agents-Server)
- 🌐 Frontend: [NLW-Agents-Web](https://github.com/IgorBern02/NLW-Agents-Web)

---

## 📷 Preview

![Preview NLW Agents](https://via.placeholder.com/1000x500?text=Insira+um+print+do+projeto+rodando+aqui)

> Você pode substituir essa imagem por um print real da aplicação.

---

## 🚀 Tecnologias usadas

### Backend

- Node.js + Fastify
- Zod para validação
- Drizzle ORM
- PostgreSQL com pgvector
- Docker (para banco)
- TypeScript

### Frontend

- React com Vite
- Tailwind CSS
- ShadCN UI
- Lucide Icons
- Axios
- Zustand
- Zod

---

## 🛠️ Como rodar o projeto localmente

### 🔧 1. Clone os repositórios

```bash
git clone https://github.com/IgorBern02/NLW-Agents-Server.git
git clone https://github.com/IgorBern02/NLW-Agents-Web.git
```

🧠 Backend (NLW-Agents-Server)

Acesse a pasta do backend:

```bash
cd NLW-Agents-Server
```

Instale as dependências:

```bash
npm install
```

Crie o arquivo .env:

```bash
# .env
PORT=3333
DATABASE_URL=postgres://docker:docker@localhost:5432/agents
```

Inicie o banco com Docker:

```bash
docker compose up -d
```

Rode as migrations:

```bash
npx drizzle-kit migrate
```

Inicie o servidor:

```bash
npm run dev
```

Servidor disponível em: http://localhost:3333

🌐 Frontend (NLW-Agents-Web)

Acesse a pasta do frontend:

```bash
cd ../NLW-Agents-Web
```

Instale as dependências:

```bash
npm install
```

Crie o .env apontando para o backend:

```bash
# .env
VITE_API_URL=http://localhost:3333
```

Inicie o projeto:

```bash
npm run dev
```

Aplicação acessível em: http://localhost:5173

🗂 Estrutura das pastas

### Backend

NLW-Agents-Server/
├── src/
│ ├── http/routes/
│ ├── lib/
│ └── env.ts
├── docker/
├── drizzle/
└── .env, package.json, tsconfig.json

### Frontend

NLW-Agents-Web/
├── src/
│ ├── components/
│ ├── lib/
│ ├── pages/
│ ├── stores/
│ └── main.tsx
├── public/
└── .env, vite.config.ts, package.json

✍️ Autor
Feito por @IgorBern02 no evento NLW da Rocketseat.
