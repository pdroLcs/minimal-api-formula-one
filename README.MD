# F1 API

Uma API REST simples para dados de Fórmula 1, construída com Fastify.

## O que é isso?

Este projeto fornece endpoints para acessar informações sobre times e pilotos da Fórmula 1. Perfeito para aprender sobre APIs, ou como base para algo maior.

## Requisitos

- Node.js 16+
- npm ou yarn

## Instalação

```bash
npm install
```

## Rodando

```bash
npm run dev
```

O servidor vai ficar disponível em `http://localhost:3333`

## Endpoints

### Times

**GET** `/teams` - Lista todos os times

```json
[
  {
    "id": 1,
    "name": "Ferrari",
    "base": "Maranello, Italy"
  }
]
```

### Pilotos

**GET** `/drivers` - Lista todos os pilotos

**GET** `/drivers/:id` - Retorna um piloto específico

```json
{
  "id": 1,
  "name": "Lewis Hamilton",
  "team": "Ferrari"
}
```

## Tecnologias

- [Fastify](https://www.fastify.io/) - Framework web rápido e eficiente
- [TypeScript](https://www.typescriptlang.org/) - JavaScript com tipagem estática
- [CORS](https://github.com/fastify/fastify-cors) - Suporte a requisições cross-origin
