# ecommerce-news-agent

Local n8n workflow for reading e-commerce news from RSS feeds, summarizing the updates, and sending the summaries to Telegram.

## Prerequisites

- Docker Desktop
- Docker Compose
- A browser
- Telegram bot token and target chat ID values

## Setup

```bash
cp .env.example .env
```

Edit `.env` and set safe local values. Keep secrets such as bot tokens out of Git.

```bash
docker compose up -d
docker compose logs -f n8n
```

Open n8n in your browser:

```text
http://localhost:5678
```

## Useful Commands

Start n8n:

```bash
docker compose up -d
```

Stop n8n:

```bash
docker compose down
```

Restart n8n:

```bash
docker compose restart n8n
```

View logs:

```bash
docker compose logs -f n8n
```

List containers:

```bash
docker compose ps
```

## Security

Never commit `.env`, Telegram bot tokens, chat IDs, or other secrets.
