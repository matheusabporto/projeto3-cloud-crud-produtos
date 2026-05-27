# Projeto 3 — CRUD de Produtos em Nuvem

Aplicação Full Stack desenvolvida para a disciplina de Desenvolvimento de Software em Nuvem (Unifor, 2026.1, Prof. Américo Sampaio).

## Arquitetura

- **Frontend:** HTML + CSS + JavaScript puro, servido em VM EC2 separada
- **Backend:** Node.js + Express, API REST rodando em VM EC2 separada
- **Banco de dados:** PostgreSQL gerenciado via Supabase

## Estrutura do repositório

- `/backend` — API REST com Express
- `/frontend` — Interface estática

## Status

🚧 Em desenvolvimento

## Autor

Matheus Porto — Análise e Desenvolvimento de Sistemas, Unifor

# Backend

## Banco de dados

Banco gerenciado via Supabase (PostgreSQL).

### Tabela `produtos`

| Coluna     | Tipo        | Descrição                    |
| ---------- | ----------- | ---------------------------- |
| id         | bigint      | Primary key, auto-increment  |
| nome       | text        | Nome do produto              |
| descricao  | text        | Descrição do produto         |
| preco      | numeric     | Preço (decimal)              |
| quantidade | integer     | Quantidade em estoque        |
| created_at | timestamptz | Data de criação (automática) |
