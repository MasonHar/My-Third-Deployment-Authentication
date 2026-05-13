# transactions-api

Minimal REST API for transactions (in-memory store). Useful for local development and Docker.

## Prerequisites

- Node.js 20+
- Docker (optional)

## Setup

```bash
npm install
```

Optional: add `.env.local` for machine-specific overrides (loaded after `.env`).

## Run

```bash
npm start
```

- Health: `GET /health`
- List: `GET /transactions`
- Create: `POST /transactions` with JSON `{ "amount": number, "description": string }`
- Get one: `GET /transactions/:id`
- Delete: `DELETE /transactions/:id`

## Seed

With the server running:

```bash
npm run seed
```

## Docker

```bash
docker compose up --build
```

## Dev container

Open the repo in VS Code / Cursor and choose “Reopen in Container” when prompted.
