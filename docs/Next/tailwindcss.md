# Tailwind CSS

**Tailwind CSS** is a utility-first CSS framework that allows you to build modern designs directly in your markup. It is the standard styling engine for all our Next.js projects.

## 1. Core Concepts

Instead of writing custom CSS classes like `.btn-primary`, you use utility classes like `bg-blue-500 text-white px-4 py-2 rounded`.

### Why?

- **Speed**: No context switching between HTML and CSS files.
- **Consistency**: Uses a predefined design system (spacing, colors, typography).
- **Bundle Size**: Unused CSS is automatically purged.

## 2. Essential Layout Classes

These are the bare minimum layout utilities you must master.

### Flexbox (`flex`)

The most common layout model.

| Class             | CSS Equivalent                    | Usage                                            |
| :---------------- | :-------------------------------- | :----------------------------------------------- |
| `flex`            | `display: flex;`                  | Enables flexbox context.                         |
| `flex-col`        | `flex-direction: column;`         | Stack items vertically.                          |
| `items-center`    | `align-items: center;`            | Center items on cross axis (vertically in row).  |
| `justify-center`  | `justify-content: center;`        | Center items on main axis (horizontally in row). |
| `justify-between` | `justify-content: space-between;` | Push items to edges.                             |
| `gap-4`           | `gap: 1rem;`                      | Space between items (16px).                      |
| `flex-1`          | `flex: 1 1 0%;`                   | Allow item to grow and fill space.               |

**Example:**

```tsx
<div className="flex items-center justify-between gap-4">
  <div>Left</div>
  <div>Right</div>
</div>
```

### Grid (`grid`)

Best for 2D layouts and rigid structures.

| Class         | CSS Equivalent                                      | Usage                 |
| :------------ | :-------------------------------------------------- | :-------------------- |
| `grid`        | `display: grid;`                                    | Enables grid context. |
| `grid-cols-3` | `grid-template-columns: repeat(3, minmax(0, 1fr));` | 3 equal columns.      |
| `gap-4`       | `gap: 1rem;`                                        | Space between cells.  |

**Example:**

```tsx
<div className="grid grid-cols-1 md:grid-cols-3 gap-4">
  {/* Stacks on mobile, 3 columns on medium screens+ */}
  <div className="bg-red-500">1</div>
  <div className="bg-blue-500">2</div>
  <div className="bg-green-500">3</div>
</div>
```

### Spacing & Sizing

Tailwind uses a 4px scale. `1` = `0.25rem` (4px).

- `p-4`: Padding 16px.
- `m-4`: Margin 16px.
- `w-full`: Width 100%.
- `h-screen`: Height 100vh.
- `max-w-md`: Max width ~28rem.

## 3. Styling Basics

### Typography

- `text-sm`, `text-base`, `text-lg`, `text-xl`: Font sizes.
- `font-bold`, `font-medium`: Font weights.
- `text-center`, `text-left`: Alignment.
- `text-gray-500`: Color.

### Colors & Backgrounds

- `bg-white`, `bg-black`: Background colors.
- `text-primary`: Text color using CSS variable.
- `border`, `border-gray-200`: Borders.

### Interactive States

Prefix utilities with the state name.

- `hover:bg-blue-600`: Change background on hover.
- `focus:ring-2`: Add ring on focus.
- `disabled:opacity-50`: Fade when disabled.

## 4. Next.js & Theming (CSS Variables)

We use **CSS Variables** for theming to support Dark Mode and dynamic themes easily. This is standard in our `shadcn/ui` setup.

### How it works

1. **Define Variables**: In `globals.css`, we define HSL values for semantic colors.

```css
:root {
  --primary: 222.2 47.4% 11.2%; /* H S L */
  --foreground: 210 40% 98%;
}
.dark {
  --primary: 210 40% 98%;
  --foreground: 222.2 47.4% 11.2%;
}
```

2. **Tailwind Config**: We map Tailwind classes to these variables in `tailwind.config.ts`.

```ts
theme: {
  extend: {
    colors: {
      primary: "hsl(var(--primary))",
      foreground: "hsl(var(--foreground))",
    }
  }
}
```

3. **Usage**: Use the semantic names in your code.

```tsx
<button className="bg-primary text-primary-foreground hover:bg-primary/90">
  Click Me
</button>
```

**Benefits**:

- Changing the theme only requires updating CSS variables.
- Dark mode works automatically by toggling the `.dark` class on the `html` tag.

## 5. Utility Composition (`cn`)

We use a helper function often named `cn` (short for classnames) to conditionally apply classes and resolve conflicts. It combines `clsx` and `tailwind-merge`.

### The Problem

If you have a component with default styles and want to override them:

```tsx
// Button.tsx
<button className={`bg-blue-500 p-2 ${className}`} />

// Usage
<Button className="bg-red-500" />
// Result: "bg-blue-500 p-2 bg-red-500" -> CSS conflict!
```

### The Solution: `cn`

`tailwind-merge` intelligently resolves conflicts (last one wins), and `clsx` handles conditional logic.

```ts
import { type ClassValue, clsx } from "clsx";
import { twMerge } from "tailwind-merge";

export function cn(...inputs: ClassValue[]) {
  return twMerge(clsx(inputs));
}
```

### Usage

```tsx
import { cn } from "@/lib/utils";

export function Button({ className, variant, ...props }) {
  return (
    <button
      className={cn(
        "rounded px-4 py-2 font-medium transition-colors", // Base styles
        "focus-visible:outline-none focus-visible:ring-2", // Focus styles
        variant === "primary" && "bg-primary text-primary-foreground", // Conditional
        className // Overrides (e.g., "mt-4")
      )}
      {...props}
    />
  );
}
```

Now `<Button className="bg-red-500" />` will result in `bg-red-500` correctly overriding the base style.

## Resources

- [Tailwind CSS Docs](https://tailwindcss.com/docs)
- [Tailwind Cheat Sheet](https://nerdcave.com/tailwind-cheat-sheet)
- [shadcn/ui Theming](https://ui.shadcn.com/docs/theming)
