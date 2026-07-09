# Frontend System Design

Hands-on examples and exercises from working through frontend system design fundamentals. Each folder is a self-contained example that runs in the browser — no build step required.

## Examples

| Example | What it covers |
| --- | --- |
| [`dom/`](dom/) | Building DOM components from a `<template>` element — cloning template content and populating it instead of parsing HTML strings. |
| [`intersection-observer/`](intersection-observer/) | Infinite scroll using the Intersection Observer API — batching DOM mutations in a `DocumentFragment` as new data loads. |

## Shared

- [`styles/`](styles/) — shared CSS used across examples.
- [`utils/`](utils/) — shared helpers (e.g. a mock DB for paginated data).

## Running

These are plain HTML/CSS/JS files. Since the examples use ES modules, serve the folder over HTTP rather than opening the file directly:

```bash
# from the repo root
npx serve .
# then open the printed URL and navigate to /dom/ or /intersection-observer/
```
