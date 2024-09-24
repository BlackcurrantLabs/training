# Orval

Orval is similar to `swagger-codegen`, but it's much more tuned to react ecosystem.
Not only does it convert your swagger definition to usable apis, but it also wraps the call in `react-query`

Moreover, it can use your swagger definitions to create zod validators which are typesafe.

## orval.config.js

```javascript
module.exports = {
  api: {
    input: "./src/swagger/swagger.yaml",
    output: {
      target: "./src/swagger/lib/",
      mode: "tags-split",
      schemas: "./src/swagger/models/",
      client: "react-query",
      override: {
        mutator: {
          path: './src/swagger/axios-instance.ts',
          name: 'customInstance'
        }
      }
    },
  },
  validators: {
    input: "./src/swagger/swagger.yaml",
    output: {
      client: "zod",
      mode: "tags-split",
      target: "./src/zod",
    },
  },
};
```