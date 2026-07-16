# ADR-002: Enterprise Folder Structure

## Status

Accepted

## Context

As the application grows, a flat `src/` with no structure leads to:
- Difficulty finding files
- Merge conflicts from unrelated changes
- No clear ownership boundaries

We looked at patterns from large-scale React applications at companies like Meta, Airbnb, and Shopify.

## Decision

Adopt a **feature-agnostic layered structure** with clear separation:

- `pages/` for route-level components
- `components/` for reusable UI
- `layouts/` for page wrappers
- `hooks/`, `services/`, `utils/` for shared logic
- `types/`, `constants/` for shared definitions

As the app scales, we can introduce **feature folders** inside `pages/` or a dedicated `features/` directory.

## Consequences

**Positive:**
- Easy onboarding — devs know where things go
- Scales well from small to medium apps
- Clean import paths with barrel exports

**Negative:**
- May feel over-engineered for very small features initially
- Requires discipline to avoid dumping everything in `components/`
