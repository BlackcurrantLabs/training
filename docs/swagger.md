# Swagger

Also known as <a href="https://swagger.io/specification/">open api spec</a>, is a structured way of documenting APIs.
A swagger docs contains all the different routes exposed by the backend, ways to authenticate them, and the inputs and outpus that that particular API provides.

Swagger doc can be thought of as a contract between the frontend and the backend.

We use swagger 2.0 internally as it has the largest ecosystem and support across the board.

As a backend developer, you're expected to document all the APIs you develop. Moreover, we recommened that you write the swagger doc for the api first and then write the API logic while making sure the actual API conforms exactly to what was documented in Swagger.

We use generated client libraries extensively which reduces the effort of writing API specific login in the frontend.

!!! tldr "Interative explorer"

    <a href="https://openapi-map.apihandyman.io/">https://openapi-map.apihandyman.io/</a> is an interactive explorer for the fields available in a swagger doc

!!! tldr "Online Editor"

    <a href="https://editor.swagger.io/">https://editor.swagger.io/</a> is an online editor to get started with swagger quickly. Although in real-world projects the swagger file is included in source control.