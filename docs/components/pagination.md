# Pagination

A page navigator for paged content (search results, tables, listings).
Use a `<nav aria-label>` so assistive tech announces its purpose, and
mark the current page with `aria-current="page"`.

## Basic

```html
<nav aria-label="Search results">
  <ul class="pagination">
    <li><a href="?page=1" class="page-link" aria-label="Previous">‹</a></li>
    <li><a href="?page=1" class="page-link" aria-current="page">1</a></li>
    <li><a href="?page=2" class="page-link">2</a></li>
    <li><a href="?page=3" class="page-link">3</a></li>
    <li><a href="?page=4" class="page-link">4</a></li>
    <li><a href="?page=2" class="page-link" aria-label="Next">›</a></li>
  </ul>
</nav>
```

## Sizes

```html
<ul class="pagination pagination-sm">…</ul>
<ul class="pagination pagination-lg">…</ul>
```

## Joined

Visually connected segments instead of separated chips:

```html
<ul class="pagination pagination-joined">
  <li><a href="#" class="page-link">‹</a></li>
  <li><a href="#" class="page-link" aria-current="page">1</a></li>
  <li><a href="#" class="page-link">2</a></li>
  <li><a href="#" class="page-link">3</a></li>
  <li><a href="#" class="page-link">›</a></li>
</ul>
```

## Disabled state

Use `aria-disabled="true"` (or the `disabled` class) to grey out a link.
The CSS sets `pointer-events: none` for both selectors.

```html
<li><a href="#" class="page-link" aria-disabled="true" aria-label="Previous">‹</a></li>
```
