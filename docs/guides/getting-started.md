# Getting Started

## Prerequisites

- Node.js v24.18.0+
- npm 10+

## Setup

```bash
# Clone the repository
git clone <repo-url>
cd time

# Install dependencies
npm install

# Start development server
npm run dev
```

## Available Scripts

| Command         | Description                          |
| --------------- | ------------------------------------ |
| `npm run dev`   | Start dev server at localhost:5173   |
| `npm run build` | Type-check and build for production  |
| `npm run lint`  | Run ESLint                           |
| `npm run preview` | Preview production build locally   |

## Project Conventions

- **File naming:** PascalCase for components (`HomePage.tsx`), camelCase for utils/hooks (`useAuth.ts`)
- **Exports:** Use named exports (avoid default exports)
- **Imports:** Use absolute paths via `@/` alias
- **Components:** Functional components with TypeScript interfaces for props
