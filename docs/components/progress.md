# Progress

Linear progress indicator. Pair it with `role="progressbar"` and the
`aria-value*` attributes so screen readers report the percentage.

## Basic

```html
<div
  class="progress"
  role="progressbar"
  aria-valuenow="40"
  aria-valuemin="0"
  aria-valuemax="100"
>
  <div class="progress-bar" style="width: 40%">40%</div>
</div>
```

## Sizes

```html
<div class="progress progress-sm">
  <div class="progress-bar" style="width: 25%"></div>
</div>

<div class="progress progress-lg">
  <div class="progress-bar" style="width: 80%">80%</div>
</div>
```

## Variants

The bar accepts any of the framework's context colors.

```html
<div class="progress">
  <div class="progress-bar progress-bar-success" style="width: 60%"></div>
</div>
<div class="progress">
  <div class="progress-bar progress-bar-danger" style="width: 30%"></div>
</div>
```

## Striped & animated

```html
<div class="progress progress-striped progress-animated">
  <div class="progress-bar progress-bar-info" style="width: 55%"></div>
</div>
```

## Indeterminate

Use when you don't know how long a task will take.

```html
<div
  class="progress progress-indeterminate"
  role="progressbar"
  aria-label="Loading"
>
  <div class="progress-bar"></div>
</div>
```
