# Prisma ORM

**Prisma** is our standard ORM for Node.js and TypeScript.

## Why Prisma?

We have chosen Prisma as our primary ORM for the following reasons:

- **Type Safety**: Auto-generated types based on your schema.
- **Syntax**: The query syntax is intuitive and readable, similar to Sequelize.
- **Ecosystem**: Robust migration tools (`prisma migrate`) and a great visual editor (`prisma studio`).

- **Docs**: [https://www.prisma.io/docs](https://www.prisma.io/docs)

## Prisma vs Drizzle

| Feature         | Prisma                           | Drizzle                         |
| :-------------- | :------------------------------- | :------------------------------ |
| **Philosophy**  | Schema-first (schema.prisma)     | Code-first (TypeScript schema)  |
| **Query Style** | Object-based, abstracted         | SQL-like, closer to raw SQL     |
| **Performance** | Good (Rust engine)               | Excellent (Lightweight wrapper) |
| **Our Choice**  | **Preferred** (Better DX/Syntax) | Alternative                     |

We switched back to Prisma primarily because its syntax feels more natural for our team's workflow, resembling established patterns like Sequelize.
