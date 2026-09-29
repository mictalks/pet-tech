# Pet-Tech

Pet-Tech é um projeto backend em Node.js com TypeScript e Fastify, pensado para servir como base para uma API de gestão de pets e serviços relacionados.

## Tecnologias

- Node.js
- TypeScript
- Fastify
- Zod
- dotenv

## Estrutura do projeto

```bash
pet-tech/
├── src/
│   ├── app.ts
│   ├── server.ts
│   └── env/
│       └── index.ts
├── package.json
├── tsconfig.json
└── README.md
```

## Requisitos

- Node.js 18+
- npm

## Instalação

No diretório do projeto, execute:

```bash
npm install
```

## Variáveis de ambiente

O projeto valida as variáveis de ambiente com Zod. Crie um arquivo `.env` na raiz do projeto com o seguinte conteúdo:

```env
NODE_ENV=development
PORT=3000
```

Observações:
- `NODE_ENV` deve ser `development`, `production` ou `test`
- `PORT` deve ser um número válido

## Executando a aplicação

Para iniciar o servidor em modo de desenvolvimento:

```bash
npx tsx src/server.ts
```

Se quiser observar alterações em tempo real:

```bash
npx tsx watch src/server.ts
```

O servidor ficará disponível em:

```text
http://localhost:3000
```

## Como o projeto funciona

- `src/app.ts`: cria a instância do Fastify
- `src/server.ts`: inicia o servidor na porta configurada
- `src/env/index.ts`: valida e exporta as variáveis de ambiente

## Observações

Este projeto ainda está em estrutura inicial. A aplicação já está configurada com Fastify, TypeScript e validação de ambiente, e pode servir de base para criação de rotas, controllers, banco de dados e autenticação.

## Próximos passos sugeridos

- adicionar rotas da API
- conectar com banco de dados
- criar estrutura de módulos e serviços
- adicionar scripts no `package.json` para dev/build/start
- incluir testes automatizados
