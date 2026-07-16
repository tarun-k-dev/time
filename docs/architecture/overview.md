# Architecture Overview

## Tech Stack

- **Framework:** React 19
- **Build Tool:** Vite 8
- **Language:** TypeScript 6
- **Routing:** React Router DOM
- **Node:** v24.18.0

## Folder Structure

```
src/
├── assets/          # Static assets (images, fonts, icons)
├── components/      # Reusable UI components
│   └── common/      # Shared components (Button, Input, Modal, etc.)
├── constants/       # App-wide constants and enums
├── hooks/           # Custom React hooks
├── layouts/         # Page layout wrappers
├── pages/           # Route-level page components
├── routes/          # Routing configuration
├── services/        # API calls and external service integrations
├── styles/          # Global styles, theme, variables
├── types/           # TypeScript type definitions and interfaces
└── utils/           # Utility/helper functions
```

## Design Principles

1. **Separation of Concerns** — Each folder has a single responsibility
2. **Colocation** — Related files stay close together
3. **Flat over nested** — Avoid deep nesting; prefer flat structures within folders
4. **Barrel exports** — Use index.ts files for clean imports
5. **Lazy loading** — Route-level code splitting for performance
