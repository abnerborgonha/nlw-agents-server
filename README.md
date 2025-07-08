# Let Me Ask Server

![Let Me Ask Server Cover](https://github.com/user-attachments/assets/54ef9379-e0f9-4d7f-8910-735c41da6084)

Let Me Ask Server é a API backend de uma aplicação inovadora para responder, em tempo real, perguntas de pessoas que estão assistindo a uma live — mesmo que tenham chegado atrasadas. O objetivo é utilizar inteligência artificial e um banco vetorial para buscar respostas baseadas no que foi falado durante a transmissão, permitindo que qualquer espectador recupere informações relevantes do momento exato da live. O projeto está em desenvolvimento inicial.

## Principais Tecnologias

- **Node.js** & **Fasify** para o servidor
- **TypeScript** para segurança de tipos
- **Drizzle** como ORM para banco de dados
- **pgvector** para busca semântica de respostas


## Rotas Disponíveis

- `GET /health` — Health check da API
- `GET /rooms` — Listagem das salas disponíveis

## Como Rodar o Projeto

### Pré-requisitos

- Node.js ≥ 18.x
- npm ou yarn
- PostgreSQL com PG Vector

### Instalação

```bash
git clone https://github.com/your-username/let-me-ask-server.git
cd let-me-ask-server
npm install
```

### Configuração do Ambiente

Copie o arquivo de exemplo e ajuste as variáveis necessárias:

```bash
cp .env.example .env
```

Atualize as credenciais do banco de dados conforme necessário.

### Migração do Banco de Dados

Após configurar o ambiente, execute a migração do banco de dados para criar as tabelas necessárias:

```bash
npx drizzle-kit push
```

Esse comando aplica as migrations definidas no projeto usando o Drizzle ORM. Certifique-se de que o banco de dados esteja acessível e as variáveis de ambiente estejam corretamente configuradas antes de rodar o comando.

### Executando o Servidor

```bash
npm run dev
```

O servidor estará disponível em `http://localhost:3333`.

---

Projeto em desenvolvimento — feito com dedicação pelo time Let Me Ask.
