# MinimaCSS

**A minimal CSS framework, fully modern. ~24 KB gzipped. Built for Baseline 2024+.**

MinimaCSS isn't another Bootstrap-alike. It's a small CSS framework built on the features that finally let CSS solve problems that used to require JavaScript or huge utility-class bundles: `light-dark()`, `color-mix()`, `@starting-style`, `:user-invalid`, container queries, cascade layers, Popover + Anchor Positioning, and `:has()`.

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/hardikforall/MinimaCSS@v0.3.0/dist/minimacss.min.css">
```

[Live component showcase](https://hardikforall.github.io/MinimaCSS/examples/) · [Docs](https://hardikforall.github.io/MinimaCSS/docs/) · [Dashboard demo](https://hardikforall.github.io/MinimaCSS/examples/dashboard.html)

---

## Pain points it solves (that other frameworks don't)

### 1. One-token rebrand

Change a single CSS variable; every button, link, focus ring, and accent in the framework re-tints automatically via `color-mix(in oklch, …)`.

```css
:root { --accent-color: #ff5a5f; }
/* Hover, focus, ring, link, nav, progress bar, toast — all updated. */
```

No Tailwind config rebuild. No Bootstrap Sass recompile. No theme file with 80 redeclarations.

### 2. One declaration per token (light *and* dark)

Themes are defined once using `light-dark()`:

```css
--surface-primary-color: light-dark(#ffffff, #111a33);
--text-primary-color:    light-dark(#182447, #c8d3f7);
```

`<html data-theme="dark">` flips `color-scheme`; the values resolve automatically. No `dark:` utility prefixes. No second `.dark { … }` block.

### 3. Forms that aren't angry by default

`:user-invalid` styles only fire **after the user has interacted with the field** — no more red borders on every input the moment the page loads.

```html
<div class="field">
  <label for="email">Email</label>
  <input id="email" class="input" type="email" required>
  <small class="helper-text">We never share your email.</small>
</div>
```

The `.field` wrapper auto-appends a required asterisk (via `:has(:required)`) and flips the helper-text colour on `:user-invalid`. No JavaScript, no `.is-invalid` class to toggle.

### 4. JS-free menus, dropdowns, modals, accordions

| Component | How it works |
|---|---|
| **Modal** | Native `<dialog>` + `@starting-style` + `transition-behavior: allow-discrete` |
| **Dropdown / Popover** | Native `popover` attribute + CSS Anchor Positioning |
| **Accordion** | Native `<details>` / `<summary>` |
| **Tooltip** | CSS-only via `:hover` / `:focus-within` |
| **Theme switcher** | `<input type="radio">` + `:checked` + `color-scheme` |

No focus-trap library. No `aria-*` attribute juggling. The browser handles open/close, escape-to-dismiss, light-dismiss, focus restoration, and stacking.

### 5. Animate from `display: none`

Modal, slideover, toast, and popover all use `@starting-style` + `allow-discrete` so they animate both open *and* close — even though the closed state is `display: none`. No `animation-fill-mode` games, no `setTimeout` workarounds.

### 6. Container-query-aware components

`.card` is itself a query container. The same card adapts its padding to its own width — narrower in a sidebar, more generous in a hero. No JS observer, no breakpoint guess-work.

### 7. Cascade layers — no `!important`

```css
@layer reset, base, components, utilities;
```

Utility classes reliably override component styles because they live in a later layer. The framework ships ~13 `!important` declarations total — all in print or reduced-motion contexts.

### 8. Layout primitives for the patterns you actually write

```html
<div class="stack">…</div>            <!-- vertical rhythm -->
<div class="cluster">…</div>          <!-- wrap with gap -->
<article class="center">…</article>   <!-- centered measure -->
<div class="sidebar-layout">…</div>   <!-- sidebar + main, wraps -->
<div class="switcher">…</div>         <!-- row → column at threshold -->
```

Inspired by [Every-Layout](https://every-layout.dev/). One-line solutions for 80% of the layouts you currently write by hand.

### 9. Modern input affixes (without "input-group" choreography)

```html
<div class="input-affix">
  <span class="input-affix-prefix">$</span>
  <input class="input" type="number">
  <span class="input-affix-suffix">USD</span>
</div>
```

`:has(:focus-visible)` on the wrapper lifts the focus ring onto the whole affix. No nested-control choreography.

### 10. Drop-in skeleton, empty state, scroll-snap

```html
<div class="skeleton skeleton-text"></div>

<div class="empty-state">
  <h3 class="empty-state-title">No orders yet</h3>
  <p class="empty-state-description">When customers place an order it'll appear here.</p>
</div>

<div class="scroll-x snap-x">
  <article class="card snap-start">…</article>
  <article class="card snap-start">…</article>
</div>
```

Skeleton shimmer respects `prefers-reduced-motion`. Empty state is a one-line component. Carousels are a no-JS CSS pattern.

### 11. Named z-index scale (no more `9999`)

```css
--z-dropdown: 100;
--z-sticky:   200;
--z-overlay:  900;
--z-modal:    1000;
--z-popover:  1100;
--z-toast:    1200;
--z-tooltip:  1300;
```

Layer overlays by name. Modals can never sit above toasts by accident.

### 12. Self-contained

- No external font import (system stack by default; opt in to Inter via one variable).
- No icon font requirement (framework is icon-agnostic; examples use inline SVG).
- No JavaScript bundle. Pages that don't use Tabs work with zero JS.

---

## Quick feature list

- **25+ components** — buttons, inputs, **`.field`**, **`.input-affix`**, **`.kbd`**, modals, accordion, navigation, cards, slideovers, steps, tabs, segments, loader, progress, tables, avatars, badges, dividers, tooltips, toasts, pagination, alerts, **popover**, **skeleton**, **empty-state**
- **Layout primitives** — `.stack`, `.cluster`, `.center`, `.sidebar-layout`, `.switcher`, `.cover`, `.box`
- **Container queries** — `.cq`, `.cq-named`, plus `.card` is itself a container
- **Scroll-snap utilities** — `.scroll-x`, `.snap-x/-y`, `.snap-start/-center/-end`, plus `.scroll-x-hide-scrollbar`
- **Theme-aware visibility** — `.only-light` / `.only-dark`
- **Cascade layers** — utilities beat components without `!important`
- **Light & Dark mode** built in via `light-dark()` + `color-scheme`
- **Modern Sass** — `@use`/`@forward`, no `@import`, no `map-get`, no `green()`/`blue()` — zero deprecation warnings on Dart Sass 1.100+
- **Accessibility-first** — `:focus-visible`, WCAG-AA contrast tokens, `prefers-reduced-motion`, 40px+ touch targets, print stylesheet, `.sr-only`
- **Tiny** — ~126 KB minified, ~24 KB gzipped, **0 npm vulnerabilities**

## Installation

### From CDN

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/hardikforall/MinimaCSS@v0.3.0/dist/minimacss.min.css">
```

### From npm

```bash
npm install minimacss
```

```html
<link rel="stylesheet" href="/node_modules/minimacss/dist/minimacss.min.css">
```

### From source

```bash
git clone https://github.com/hardikforall/MinimaCSS.git
cd MinimaCSS
npm install
npm run build
```

`dist/minimacss.css` and `dist/minimacss.min.css` (with autoprefixer + source map) land in `dist/`.

## Theming

```css
:root {
  --accent-color: #4f46e5; /* every interactive accent re-tints */
}
```

Force a theme:

```html
<html data-theme="dark">  <!-- or "light", or omit for OS-driven -->
```

Customise any token — every CSS variable in [`src/themes/_theme.scss`](src/themes/_theme.scss) is fair game.

## Documentation

- [Getting Started](docs/GettingStarted.md)
- [Theming & Dark Mode](docs/theme.md)
- [Customisation](docs/customization.md)
- [Accessibility](docs/accessibility.md)
- [Best practices](docs/best-practices.md)
- [Changelog](docs/changelog.md)

[Full docs](https://hardikforall.github.io/MinimaCSS/docs/) · [Component showcase](https://hardikforall.github.io/MinimaCSS/examples/) · [Dashboard demo](https://hardikforall.github.io/MinimaCSS/examples/dashboard.html)

## Browser support

Baseline 2024+ — Safari 17.5+, Chrome 117+, Firefox 121+. Uses `light-dark()`, `color-mix()`, `@starting-style`, `transition-behavior: allow-discrete`, `:user-invalid`, `field-sizing`, container queries, cascade layers, `text-wrap: balance/pretty`, Popover API, and CSS Anchor Positioning.

For older browsers, stay on [MinimaCSS 0.2](https://www.npmjs.com/package/minimacss/v/0.2.0).

## Contributing

```bash
npm install
npm run dev    # watches SCSS + serves examples/ at http://localhost:4200
npm run lint   # stylelint
npm run build  # produces dist/ with autoprefixer
```

Open a PR. Linting and a clean build are required.

## License

MIT.
