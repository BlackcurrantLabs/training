# State Management

Managing state effectively is key to a scalable React application. We follow a specific hierarchy of strategies.

## 1. URL State

**The URL is the ultimate source of truth.**

- Use for: Search filters, pagination, active tabs, modal open states.
- Why: Makes the state shareable and bookmarkable.

## 2. Server State

**Let the server handle the data.**

- Use: **React Query** (Client Components) or **RSC** (Server Components).
- Why: Keeps client state in sync with the DB without manual complexity.

## 3. Local State

**Component-level UI state.**

- Use: `useState`, `useReducer`.
- Why: Simple, isolated interactions (e.g., form input, toggle menu).

## 4. Client Global State

**Application-wide client state.**

- Use: **React Context API**.
- **Rule**: Do NOT use third-party libraries like Zustand or Redux unless absolutely necessary. The Context API is sufficient for most global state needs (e.g., theme, user session).
