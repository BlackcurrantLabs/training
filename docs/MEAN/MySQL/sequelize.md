# Sequelize JS

Sequelize is an ORM that helps your write queries for relational Databases. It supports Postgres, MySQL, SQLite, etc. Other popular ORMs are Prisma, TypeORM, etc.

Defining models and validations and querying via them avoids smaller errors in development time. While it's possible to fire native queries also, it's highly recommended not to.

Sequelize is particularly useful to join tables and return the result in nested JSON objects. This makes writing API logic very easy.

!!! tldr "Project Homepage"
    [https://sequelize.org/](https://sequelize.org/)

!!! tldr "Sequelize CLI"
    This small utility can help with getting started with sequelize in your express project very easily.
    It will lay out the scaffolds and create some primitive models to help you get started.

    [https://www.npmjs.com/package/sequelize-cli](https://www.npmjs.com/package/sequelize-cli)

!!! tldr "Sequelize Guides"
    This small utility can help with getting started with sequelize in your express project very easily.
    It will layout the scaffolds and create some primitive models to help you get started.
    
    [https://sequelize.org/docs/v6/](https://sequelize.org/docs/v6/)

## Important Concepts to learn
Ideally you should read the full guides section of the Sequelize project. But the concepts mentioned below are bare minimum that you should know.

### Defining Models
This is where you define individual tables and the columns they should have

[https://sequelize.org/docs/v6/core-concepts/model-basics/](https://sequelize.org/docs/v6/core-concepts/model-basics/)

### Querying 
Basic Queries based on model definitions

[https://sequelize.org/docs/v6/core-concepts/model-querying-basics/](https://sequelize.org/docs/v6/core-concepts/model-querying-basics/)

### Validations 
Making models bullet-proof for production applications

[https://sequelize.org/docs/v6/core-concepts/validations-and-constraints/](https://sequelize.org/docs/v6/core-concepts/validations-and-constraints/)

### Associations
Linking models to each other via one to one, one to many or many to one relationships.

[https://sequelize.org/docs/v6/core-concepts/validations-and-constraints/](https://sequelize.org/docs/v6/core-concepts/assocs/)

### Eager Loading
Using linking defined in models to query across multiple tables for nested outputs.

[https://sequelize.org/docs/v6/advanced-association-concepts/eager-loading/](https://sequelize.org/docs/v6/advanced-association-concepts/eager-loading/)
