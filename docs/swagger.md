# Swagger

Also known as <a target="_blank" href="https://swagger.io/specification/">open api spec</a>, is a structured way of documenting APIs.
A swagger docs contains all the different routes exposed by the backend, ways to authenticate them, and the inputs and outpus that that particular API provides.

Swagger doc can be thought of as a contract between the frontend and the backend.

We use swagger 2.0 internally as it has the largest ecosystem and support across the board.

As a backend developer, you're expected to document all the APIs you develop. Moreover, we recommened that you write the swagger doc for the api first and then write the API logic while making sure the actual API conforms exactly to what was documented in Swagger.

We use generated client libraries extensively which reduces the effort of writing API specific login in the frontend.

## Why this is critical

- Frontend and backend teams can develop in parallel.
- API changes are easier to track and review.
- Breaking changes can be detected early in CI.

## Minimum documentation checklist

- Endpoint purpose and ownership
- Auth requirements
- Request and response schema examples
- Error response structure
- Pagination/filter/sort semantics
- Versioning strategy

!!! tldr "Best practices"

    - Keep your OpenAPI spec in source control with code reviews.
    - Generate API clients from spec to avoid manual drift.
    - Validate API responses against schema during testing.

!!! tldr "Interative explorer"

    <a target="_blank" href="https://openapi-map.apihandyman.io/">https://openapi-map.apihandyman.io/</a> is an interactive explorer for the fields available in a swagger doc

!!! tldr "Online Editor"

    <a target="_blank" href="https://editor.swagger.io/">https://editor.swagger.io/</a> is an online editor to get started with swagger quickly. Although in real-world projects the swagger file is included in source control.

!!! tldr "Additional resources"

    - <a target="_blank" href="https://swagger.io/docs/specification/about/">https://swagger.io/docs/specification/about/</a>
    - <a target="_blank" href="https://www.openapis.org/">https://www.openapis.org/</a>
