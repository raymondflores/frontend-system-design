# Frontend System Design

Hands-on examples and exercises from working through frontend system design fundamentals. Each folder is a self-contained example that runs in the browser — no build step required.

## Examples

| Example | What it covers |
| --- | --- |
| [`dom/`](dom/) | Building DOM components from a `<template>` element — cloning template content and populating it instead of parsing HTML strings. |
| [`intersection-observer/`](intersection-observer/) | Infinite scroll using the Intersection Observer API — batching DOM mutations in a `DocumentFragment` as new data loads. |
| [`mutation-observer/`](mutation-observer/) | Reacting to DOM changes with the Mutation Observer API — a Notion-style editor that turns `/h1`–`/h3` shortcuts into heading elements as you type. |
| [`resize-observer/`](resize-observer/) | Responding to element size changes with the Resize Observer API — restyling resizable boxes based on their `borderBoxSize` as the user drags them. |
| [`virtualisation/`](virtualisation/) | List virtualisation — keeping a fixed pool of DOM nodes and recycling them via CSS transforms as top/bottom Intersection Observers fire, so a long list stays cheap to render. |

## Shared

- [`styles/`](styles/) — shared CSS used across examples.
- [`utils/`](utils/) — shared helpers (e.g. a mock DB for paginated data).

## Running

These are plain HTML/CSS/JS files. Since the examples use ES modules, serve the folder over HTTP rather than opening the file directly:

```bash
# from the repo root
npx serve .
# then open the printed URL and navigate to any example folder, e.g. /dom/ or /virtualisation/
```
