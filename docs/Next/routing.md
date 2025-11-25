# Routing

Next.js uses a **file-system based router**.

## App Router

The `app` directory is the root of your routes. Folders define routes, and files define the UI.

### Special Files

- `page.tsx`: The UI for a route.
- `layout.tsx`: Shared UI for a segment and its children (e.g., navigation).
- `loading.tsx`: Loading UI for a segment (Suspense fallback).
- `error.tsx`: Error UI for a segment.
- `not-found.tsx`: UI for 404 errors.

### Dynamic Routes

You can create dynamic segments by wrapping a folder name in square brackets: `[folderName]`.
For example, `app/blog/[slug]/page.tsx` matches `/blog/hello-world`.

- **Docs**: [https://nextjs.org/docs/app/building-your-application/routing](https://nextjs.org/docs/app/building-your-application/routing)
