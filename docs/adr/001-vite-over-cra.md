# ADR-001: Vite over Create React App

## Status

Accepted

## Context

We needed a build tool for the React project. The main options considered were:

- **Create React App (CRA)** — officially deprecated, slow builds, limited config
- **Vite** — fast HMR, native ESM, minimal config, actively maintained
- **Next.js** — full-stack framework, SSR/SSG, overkill for a client-side SPA

## Decision

We chose **Vite** as the build tool.

## Consequences

**Positive:**
- Near-instant dev server startup via native ES modules
- Fast Hot Module Replacement (HMR)
- Simple configuration with sensible defaults
- Active community and ecosystem support
- Easy to extend with plugins

**Negative:**
- No built-in SSR (not needed for this project)
- Slightly different config patterns than webpack-based tools
