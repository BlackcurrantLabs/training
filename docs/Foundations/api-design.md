# API Design Fundamentals

Good API design reduces integration bugs and speeds up delivery.

## Basic design rules

- Keep naming consistent and predictable.
- Model resources clearly.
- Return meaningful status codes and error messages.
- Version breaking changes.
- Validate inputs at the boundary.
- Document with OpenAPI/Swagger.

## Common pitfalls

- Overloading one endpoint for unrelated operations
- Returning different shapes for similar resources
- Missing pagination and filtering strategy
- Silent failures without error contracts

## Resources

- [Microsoft REST API Guidelines](https://github.com/microsoft/api-guidelines)
- [Zalando RESTful API Guidelines](https://opensource.zalando.com/restful-api-guidelines/)
- [OpenAPI Specification](https://swagger.io/specification/)
