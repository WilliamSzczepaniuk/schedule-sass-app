
# Contexto do Projeto: SaaS de Agendamento e Gestão

## Stack Tecnológica
- **Framework:** Next.js (App Router) + React 19 + TypeScript
- **Estilização:** Tailwind CSS
- **ORM / Banco de Dados:** Prisma ORM com PostgreSQL (Relacional) e MongoDB (Não Relacional)
- **Validação / Autenticação:** Zod, NextAuth / JWT
- **Microserviço:** PHP para geração de relatórios em PDF/Email

## Padrões de Código e Convenções
1. Usar **Server Components** no Next.js por padrão; usar `'use client'` apenas onde houver interatividade/hooks.
2. Nomenclatura em **camelCase** para variáveis e funções; **PascalCase** para componentes React e tipos TypeScript.
3. Todas as rotas de API em `/app/api` devem ter validação de entrada usando **Zod**.
4. Não utilizar `any` no TypeScript. Tipar explicitamente retornos e props.
5. Commits no padrão **Conventional Commits** (`feat:`, `fix:`, `docs:`, `refactor:`).

## Comandos Úteis
- `npm run dev` - Roda o servidor de desenvolvimento.
- `npx prisma db push` - Sincroniza o schema do Prisma com o banco.
- `npx prisma studio` - Interface visual para inspecionar o banco de dados.