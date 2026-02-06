# Data Modeling and Migrations

Bad schema decisions are expensive to fix later. Plan for change from the start.

## Data modeling essentials

- Normalize where needed, denormalize where useful
- Define clear ownership of data entities
- Use indexes intentionally
- Track constraints and invariants in schema

## Migration safety

- Make migrations forward-compatible
- Avoid long locks on large tables
- Backfill data in batches
- Validate before and after migration
- Keep rollback strategy ready

## Resources

- [Database Normalization](https://www.geeksforgeeks.org/dbms/normalization-in-dbms/)
- [PostgreSQL ALTER TABLE](https://www.postgresql.org/docs/current/sql-altertable.html)
- [Prisma Migrate](https://www.prisma.io/docs/orm/prisma-migrate)
- [Liquibase Docs](https://www.liquibase.com/documentation)
