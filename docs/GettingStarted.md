# Getting Started

MinimaCSS drops into any HTML page with one `<link>` tag, no build step
required. This guide walks you from a blank page to a working layout with
real MinimaCSS components.

## Quick Start

Add MinimaCSS to your `<head>`:

```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/hardikforall/MinimaCSS/dist/minimacss.min.css"
/>
```

> Tip: lock to a specific tag in production (e.g. `@v0.2.0`) rather than
> `@latest` from `gh`.

Or install from npm and copy from `dist/`:

```bash
npm install minimacss
```

```html
<link rel="stylesheet" href="/node_modules/minimacss/dist/minimacss.min.css" />
```

## Basic Template

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Your Project</title>
    <link
      rel="stylesheet"
      href="https://cdn.jsdelivr.net/gh/hardikforall/MinimaCSS/dist/minimacss.min.css"
    />
  </head>
  <body>
    <main class="container">
      <h1>Welcome to MinimaCSS</h1>
      <button class="btn btn-primary">Click Me</button>
    </main>
  </body>
</html>
```

## Using Components

A handful of common building blocks. See `docs/components/*` for the full
inventory.

**Buttons**

```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-outline-primary">Outline</button>
<button class="btn btn-success btn-sm">Save</button>
<button class="btn btn-danger" disabled>Disabled</button>
```

**Input with label and helper text**

```html
<div class="input-group">
  <label for="email">Email</label>
  <input id="email" class="input" type="email" placeholder="you@example.com" />
  <small class="helper-text">We never share your email.</small>
</div>
```

**Card**

```html
<div class="card">
  <div class="card-header">Stats</div>
  <div class="card-body">
    <p>1,284 active users this week.</p>
  </div>
  <div class="card-footer">
    <button class="btn btn-sm btn-primary">View</button>
  </div>
</div>
```

**Modal** (uses the native `<dialog>` element)

```html
<button class="btn btn-primary" onclick="document.getElementById('m').showModal()">
  Open modal
</button>

<dialog id="m" class="modal modal-md">
  <div class="modal-header">
    <h3>Confirm</h3>
    <button class="close-icon" onclick="this.closest('dialog').close()">×</button>
  </div>
  <div class="modal-body">Delete this item? This cannot be undone.</div>
  <div class="modal-footer">
    <button class="btn btn-light" onclick="this.closest('dialog').close()">Cancel</button>
    <button class="btn btn-error">Delete</button>
  </div>
</dialog>
```

**Toast**

```html
<div class="toast-container toast-top-right">
  <div class="toast toast-success" role="status">
    <div>
      <div class="toast-title">Saved</div>
      <div class="toast-body">Your changes are live.</div>
    </div>
    <button class="toast-close" aria-label="Dismiss">×</button>
  </div>
</div>
```

## Utility classes

Use utilities to tweak spacing, layout, color, and typography without
touching component CSS. They live in `@layer utilities`, so they always
win against component styles:

```html
<div class="d-flex justify-content-between align-items-center p-3 surface-secondary rounded-lg">
  <span class="font-semi-bold">Plan: Pro</span>
  <button class="btn btn-sm btn-primary">Upgrade</button>
</div>
```

Common utility families:

- **Spacing** — `m-{0..10}`, `mt-/mr-/mb-/ml-`, `mx-/my-`, and `p-*` equivalents
- **Sizing** — `w-{1..16,25,50,75,100,auto,full,vh,vw,sm,md,lg,xl,xxl}` and `h-*`
- **Flex** — `d-flex`, `justify-content-*`, `align-items-*`, `flex-grow-*`
- **Grid** — `grid`, `grid-cols-{1..12}`, `gap-{0..10}`, `col-span-*`
- **Typography** — `text-{xs..5xl}`, `font-{light..black}`, `text-{center,left,right}`, `line-clamp-{1..6}`
- **Colors** — `text-{primary,secondary,success,danger,warning,info,light,dark}`, `bg-*`, `border-*`
- **Visibility** — `hidden`, `visible`, `invisible`, `sr-only`, `hidden-{sm,md,lg,xl,xxl}`

## Theming

MinimaCSS ships with light and dark themes driven by CSS custom properties.

```html
<!-- Respect OS setting -->
<html>...</html>

<!-- Force dark -->
<html data-theme="dark">...</html>

<!-- Force light -->
<html data-theme="light">...</html>
```

Toggle at runtime:

```js
document.documentElement.dataset.theme =
  document.documentElement.dataset.theme === "dark" ? "light" : "dark";
```

See [theme.md](theme.md) for the full token table and how to override
colors.

## Customising the build

To trim utilities you don't need or change tokens at compile time, see
[customization.md](customization.md).
