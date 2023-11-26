# Show and Hide Utilities

---

> [!NOTE] > _The content on this page is currently in progress and not yet complete. I am working to fully develop and refine the information here to ensure it meets the high standards of comprehensiveness and clarity. Other pages in this documentation may be complete. I appreciate your patience and understanding as I continue to enhance this page._

---

These utilities allow you to show or hide elements on your webpage using the `display` property.

#### Usage

- `.hidden` to hide an element.
- `.visible` to show an element.

```html
<div class="hidden surface-primary p-2 mt-2">This element will be hidden.</div>

<div class="visible surface-primary p-2 mt-2">
  This element will be visible.
</div>
```

<div class="component-preview">
<div class="hidden surface-primary p-2 mt-2">
   This element will be hidden.
</div>

<div class="visible surface-primary p-2 mt-2">
   This element will be visible.
</div>
</div>

### Visibility Utilities

These utilities allow you to control the visibility of elements on your webpage using the `visibility` property.

#### Usage

- `.invisible` to make an element invisible.
- `.visible` to make an element visible.

```html
<div class="invisible surface-primary p-2 mt-2">
  This element will be invisible.
</div>

<div class="visible surface-primary p-2 mt-2">
  This element will be visible.
</div>
```

<div class="component-preview">
<div class="invisible surface-primary p-2 mt-2">
   This element will be invisible.
</div>

<div class="visible surface-primary p-2 mt-2">
   This element will be visible.
</div>
</div>

### Screen Reader Only Utility

This utility hides an element visually but keeps it accessible to screen readers.

#### Usage

- `.sr-only` to make an element screen reader only.

```html
<div class="sr-only p-2 mt-2">
  This element is hidden visually but accessible to screen readers.
</div>
```

<div class="component-preview">
<div class="sr-only p-2 mt-2">
   This element is hidden visually but accessible to screen readers.
</div>
</div>

### Responsive Visibility Utilities

These utilities allow you to control the visibility of elements based on different breakpoints using media queries.

#### Usage

- `.hidden-{breakpoint}` to hide an element at a specific breakpoint.
- `.visible-{breakpoint}` to show an element at a specific breakpoint.

```html
<div class="hidden-md surface-primary p-2 mt-2">
  This element will be hidden on medium screens and above.
</div>

<div class="visible-md surface-primary p-2 mt-2">
  This element will be visible on medium screens and above.
</div>
```

<div class="component-preview">
<div class="hidden-md surface-primary p-2 mt-2">
   This element will be hidden on medium screens and above.
</div>

<div class="visible-md surface-primary p-2 mt-2">
   This element will be visible on medium screens and above.
</div>
</div>
