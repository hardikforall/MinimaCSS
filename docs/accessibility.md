# Accessibility

MinimaCSS aims to ship sensible defaults so the components you copy from the
docs are accessible out of the box. This page documents what the framework
does for you and where you, the application author, still need to do work.

## What the framework provides

- **Reduced motion**. The reset (`src/base/_reset.scss`) honors
  `@media (prefers-reduced-motion: reduce)` and collapses animation /
  transition durations to ~0ms.
- **`:focus-visible` rings**. Buttons render their focus ring only on
  keyboard focus, not on mouse click — see `.btn` in `_buttons.scss`.
- **Touch targets**. `.btn` is at least 2.5rem (~40px) tall; `.btn-lg` is
  3rem. Pair with adequate padding for the 44×44 WCAG 2.5.5 guideline.
- **Color contrast tokens**. The light theme uses `--text-primary-color:
  gray-700` and `--text-secondary-color: gray-500`, both of which pass
  WCAG AA against the default white surface. The dark theme uses
  light-on-dark equivalents.
- **Screen-reader utility**. `.sr-only` (in `utilities/_visibility.scss`)
  hides content visually while leaving it discoverable to assistive tech.
- **Print stylesheet**. `base/_print.scss` removes interactive chrome
  (nav, modal, tooltip, buttons) and surfaces link URLs after their text.
- **Native semantics**. The accordion (`<details>/<summary>`) and modal
  (`<dialog>`) components are built on native elements so keyboard and
  screen reader behavior comes for free.
- **CSS cascade layers**. Utilities live in `@layer utilities`, so you can
  override component styles without `!important` and without losing
  accessibility defaults from the components themselves.

## What you still need to do

- **Label every input.** `<label for="…">` or wrap the input in a label.
  The `.input` class styles, it does not label.
- **`aria-expanded` / `aria-controls`** on disclosure controls
  (`.dropdown-toggle`, accordion summaries) when you build them.
- **`role`/`aria-live`** on `.toast` and `.alert` when content updates
  dynamically. Static alerts don't need it; live notifications do.
- **Visible focus on link buttons.** `.btn-link` inherits `:focus-visible`
  but verify in your specific layouts.
- **Translate the `chevron` icon and check colors against your custom
  themes.** The default chevron is `#787f94`; override with your own SVG
  if your background is lighter than `gray-500`.

## Testing checklist

- Tab through the page — every interactive control must show a visible focus indicator.
- Trigger every modal/toast/dropdown via keyboard. They must be dismissible with `Esc`.
- Set OS dark mode. Re-test contrast (Chrome DevTools "Emulate vision
  deficiencies" + Lighthouse contrast audit).
- Set OS reduced-motion. Modals should snap in/out; the dropdown fadeIn
  should be instant.
- Print preview the page. The print stylesheet should leave a clean,
  inked document with no UI chrome.

## Known limitations

- Tooltips (`.tooltip`) are CSS-only and rely on `:hover`/`:focus-within`.
  They are not a substitute for `aria-describedby` on form fields.
- The slideover/modal components manage open state via the `open`
  attribute on `<dialog>`. If you fall back to a `<div>`, you must
  implement focus trapping yourself.
