# Client vs Server Components

Next.js App Router introduces a new paradigm with React Server Components (RSC). Understanding the distinction is crucial for performance and functionality.

## Server Components (RSC)

By default, all components in the `app` directory are **Server Components**.

- **What**: Rendered on the server. The HTML is sent to the client.
- **When to use**:
  - Fetching data.
  - Accessing backend resources (DB, API keys).
  - Keeping sensitive logic on the server.
  - Reducing client-side bundle size.

## Client Components

To use standard React features like state and effects, you must opt-in to Client Components.

- **How**: Add `'use client'` at the top of the file.
- **When to use**:

  - Interactivity (onClick, onChange).
  - State (`useState`, `useReducer`).
  - Lifecycle effects (`useEffect`).
  - Browser-only APIs (localStorage, window).

- **Docs**: [https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns](https://nextjs.org/docs/app/building-your-application/rendering/composition-patterns)
