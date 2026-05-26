# Toast

Transient notifications. Render them inside a fixed-position container in
one of six positions. The component is CSS-only — bring your own JavaScript
to show/dismiss.

## Basic

```html
<div class="toast-container toast-top-right">
  <div class="toast" role="status">
    <div class="toast-body">Settings saved.</div>
    <button class="toast-close" aria-label="Dismiss">×</button>
  </div>
</div>
```

## With title

```html
<div class="toast-container toast-bottom-right">
  <div class="toast toast-success" role="status">
    <div>
      <div class="toast-title">Saved</div>
      <div class="toast-body">Your changes are live.</div>
    </div>
    <button class="toast-close" aria-label="Dismiss">×</button>
  </div>
</div>
```

## Positions

Add one of these classes to the container:

- `toast-top-left`, `toast-top-center`, `toast-top-right`
- `toast-bottom-left`, `toast-bottom-center`, `toast-bottom-right`

## Variants

The left border accent uses any context color:

```html
<div class="toast toast-primary" role="status">…</div>
<div class="toast toast-success" role="status">…</div>
<div class="toast toast-danger" role="alert">…</div>
<div class="toast toast-warning" role="alert">…</div>
<div class="toast toast-info" role="status">…</div>
```

Use `role="alert"` for assertive (error/warning) messages and
`role="status"` for polite (informational) ones.

## Dismissing

Add the class `toast-dismissing` (e.g. from JS when the close button is
clicked) to play the exit animation, then remove the element after the
animation ends.

```js
btn.addEventListener("click", () => {
  const t = btn.closest(".toast");
  t.classList.add("toast-dismissing");
  t.addEventListener("animationend", () => t.remove(), { once: true });
});
```
