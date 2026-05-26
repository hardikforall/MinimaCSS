# Changelog

All notable changes to MinimaCSS are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.3.0] — 2026-05-27

### Modernized for Baseline 2024+

#### Architecture
- **Sass module system (`@use` / `@forward`)**: every file imports tokens via `@use "../core" as *;`. No more deprecated `@import`. Build emits zero deprecation warnings on Dart Sass 1.100+.
- Theme tokens consolidated into a single `themes/_theme.scss` using `light-dark(...)` and `color-scheme`. Light and dark are now defined once; `[data-theme="dark"]` simply flips `color-scheme: dark`.
- Hover/focus tones derived via `color-mix(in oklch, var(--accent) 88%, light-dark(black, white))` instead of hand-tuned hex pairs — change the brand colour once, every state updates.

#### Layout
- **Grid system rewritten as native CSS Grid + `gap`**. No more negative-margin / per-column-padding gutters. `.col-{N}` still works (now `grid-column: span N`). New `.row-auto` for equal-width auto-flow. New `.grid-auto-fit` / `.grid-auto-fill` using `repeat(auto-fit, minmax(...))` — responsive grids without media queries.
- **Container queries**: new `.cq` / `.cq-named` / `.cq-size` utilities. `.card` is now its own query container and adapts its padding to its parent's width via `@container`.

#### Animation
- **Modal open + close animate from `display: none`** via `transition-behavior: allow-discrete` + `@starting-style`. The page-load flash is gone.
- **Toast** uses `@starting-style` for entry; dismissal is a CSS transition (no `animation-fill-mode` games).

#### Forms
- `accent-color: var(--accent-color)` + `caret-color: var(--accent-color)` on `:root` — native checkboxes, radios, range, and text carets pick up the brand.
- `:user-invalid` / `:user-valid` styling: validation feedback appears only after the user interacts — no JS class toggling needed.
- `.textarea { field-sizing: content; }` — textareas auto-grow as you type.
- `:focus-visible` everywhere (replaces `:focus` so mouse clicks don't show the ring).

#### Typography & polish
- `text-wrap: balance` on `h1`–`h6` for orphan-free headlines.
- `text-wrap: pretty` on `p` for orphan-free body copy.
- `scrollbar-gutter: stable` on `html` so opening a modal doesn't shift layout.
- `caret-color: var(--accent-color)`.

#### Spacing scale
- Expanded `$spacers` to include half-steps (`0.5`, `1.5`, `2.5`, `3.5`) and larger sizes (`11`, `12`, `14`, `16`, `20`, `24`, `32`, `48`, `64`). Class names with half-steps use the standard escaped-period convention (`class="p-1.5"` matches `.p-1\.5`).
- New `$spacers-fluid` scale (`sm`, `md`, `lg`, `xl`, `2xl`) using `clamp()` for hero-section breathing room. Exposed as `.p-fluid-lg`, `.py-fluid-xl`, etc.

#### Logical properties
- Margin / padding utilities now ship both physical (`.mt-3`, `.pl-2`) and logical (`.mbs-3`, `.ps-2`, `.mi-4`, `.pblock-3`) variants for RTL and vertical writing modes.
- `.inset-{N}`, `.inset-x-{N}`, `.inset-y-{N}` utilities.

### Removed (breaking)
- Legacy padding-trick `.aspect-{16-9, 4-3, 1-1}` classes. Use the modern `.ratio-{video, 4-3, square}` (CSS `aspect-ratio` property).
- Unused `%clearfix` placeholder.
- Unused `$grid-columns-row` variable.
- `themes/_light.scss`, `themes/_dark.scss`, `themes/_apply.scss` → merged into `themes/_theme.scss`.
- `.col` without a number now spans 1 (was: flexbox auto-fill). Use `.row-auto` for the old behaviour.
- `live-server` (abandoned) replaced with `browser-sync@3`. `npm run dev` now reloads on file change without the vulnerabilities.

### Dependencies
- Refreshed to current: `sass@1.100`, `cssnano@8`, `stylelint@17`, `stylelint-config-standard-scss@17`, `postcss-cli@11`, `concurrently@9`, `prettier@3.8`, `autoprefixer@10.5`.
- `npm audit`: 0 vulnerabilities (was 44).
- node_modules: 444 packages (was 715).

### Browser baseline
MinimaCSS 0.3 targets browsers shipped from early 2024 onward — that's Safari 17.5+, Chrome 117+, Firefox 121+. The framework relies on `light-dark()`, `@starting-style`, `transition-behavior: allow-discrete`, `:user-invalid`, `field-sizing`, `color-mix()`, container queries, cascade layers, and `text-wrap: balance/pretty`. For older browsers, MinimaCSS 0.2 remains available on `npm`.

## [0.2.0] — 2026-05-27

### Added
- **CSS cascade layers** (`@layer reset, base, components, utilities`). Utilities now reliably override component styles without `!important`.
- **Progress** component (`.progress` / `.progress-bar`) with sm/lg sizes, color variants, striped / animated / indeterminate states.
- **Toast** component (`.toast`, `.toast-container`) with six positions, color variants, and an exit animation hook.
- **Pagination** component (`.pagination`, `.page-link`) with sm/lg sizes and a joined variant.
- **Print stylesheet** (`base/_print.scss`) — strips interactive chrome, surfaces link URLs, ink-friendly typography.
- **Utility classes**: `.line-clamp-1..6`, `.line-clamp-none`, `.ratio-{square,video,4-3,3-2,21-9}` (modern `aspect-ratio`), `.pointer-events-{none,auto,all}`, `.select-{none,text,all,auto}`.
- **`docs/accessibility.md`** — what the framework guarantees, what you still need to do, testing checklist.
- **GitHub Actions workflow** (`.github/workflows/build.yml`) — lint + build on every push and PR.
- **Stylelint** config (`.stylelintrc.json`) with `stylelint-config-standard-scss`.
- **`npm run dev`** — concurrent Sass watcher + live-server on port 4200.

### Changed
- **Removed the Inter CDN `@import`** from typography (SPOF). The framework now uses a system font stack by default and exposes `--font-family-base` / `--font-family-mono` for opt-in customisation.
- **`autoprefixer` is now in the build pipeline** (was installed but unused). Vendor prefixes ship in `dist/minimacss.css` and `dist/minimacss.min.css`.
- **Stripped `~140 !important` declarations** from utility files. Layer order handles cascade priority now.
- **Light theme text contrast** improved (`--text-primary-color: gray-700`, `--text-secondary-color: gray-500`) so both pass WCAG AA against light surfaces.
- **Dark theme `btn-light` variant** repainted to use `gray-600`/`gray-500` rather than near-white, so it stays visible on dark backgrounds.
- **`.btn` minimum height** is now 2.5 rem (`.btn-sm` 1.75 rem, `.btn-lg` 3 rem) for comfortable touch targets.
- **Button focus** now uses `:focus-visible` so the ring only appears on keyboard interaction.
- **Container max-widths** moved from a deeply-nested `if()` chain to a `$container-max-widths` map.
- **Modal `@keyframes`** are now complete (both `from` and `to` defined for `showModal` and `hideModal`).
- **Accordion content** no longer caps at `max-height: 1000px`; tall content is no longer clipped.
- **`code` / `pre`** typography refined with padding, mono variable, and small radius.

### Fixed
- Invalid hex `#cccc` in `_inputs.scss`.
- `"transparent"` string (instead of the keyword) for `--button-highlight-border-color` in the light theme.
- Trailing typo commas (`,,,`) in variable-map comments.
- Input focus ring sizing inconsistent with buttons (now both `0.25rem`).

### Tooling
- `npm run lint`, `npm run lint:fix`, `npm run format`, `npm run test` (lint + build) scripts added.
- `package.json` now declares a `browserslist` (modern targets — last 2 versions, no IE 11).
- Author field updated from placeholder.

## [0.1.0] — Initial release

- Initial component and utility set, light/dark themes, docs site.
