# Grid Utilities

---

> [!NOTE]
> _The content on this page is currently in progress and not yet complete. I am working to fully develop and refine the information here to ensure it meets the high standards of comprehensiveness and clarity. Other pages in this documentation may be complete. I appreciate your patience and understanding as I continue to enhance this page._

---

The grid utilities in MinimaCSS provide a powerful way to create grid layouts in your web projects.

## Grid Container

#### Usage
- `.grid` for a standard grid container.
- `.grid-inline` for an inline grid container.

```html
<div class="grid surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are displayed in a grid. -->
<div class="grid-inline surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are displayed inline in a grid. -->

```
<div class="component-preview d-block">
<div class="grid surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are displayed in a grid. -->
<div class="grid-inline surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are displayed inline in a grid. -->
</div>

## Grid Template Columns

#### Usage
- `.grid-cols-{number}` to define the number of columns in the grid.

```html
<div class="grid grid-cols-3 surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- A grid with 3 columns. -->
```
<div class="component-preview d-block">
<div class="grid grid-cols-3 surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
</div>

## Grid Template Rows

#### Usage
- `.grid-rows-{number}` to define the number of rows in the grid.

```html
<div class="grid grid-rows-2 surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- A grid with 2 rows. -->
```
<div class="component-preview d-block">
<div class="grid grid-rows-2 surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
</div>

## Grid Gap Utilities

#### Usage
- `.gap-{size}` to add gap between grid items.
- `.gap-x-{size}` to add horizontal gap between grid columns.
- `.gap-y-{size}` to add vertical gap between grid rows.

```html
<div class="grid gap-2 surface-tertiary p-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Grid items have a gap of 2. -->
<div class="grid gap-x-2 gap-y-4 surface-tertiary p-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Grid columns have a horizontal gap of 2 and vertical gap of 4. -->
```
<div class="component-preview d-block">
<div class="grid gr gap-2 surface-tertiary p-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Grid items have a gap of 2. -->
<div class="grid gap-x-2 gap-y-4 surface-tertiary p-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
</div>

## Grid Justification

#### Usage

- `.justify-grid-items-start` to justify grid items to the start.
- `.justify-grid-items-center` to justify grid items to the center.
- `.justify-grid-items-end` to justify grid items to the end.

- `.justify-grid-content-start` to justify grid content to the start.
- `.justify-grid-content-end` to justify grid content to the end.
- `.justify-grid-content-center` to justify grid content to the center.
- `.justify-grid-content-between` to justify grid content with space between.
- `.justify-grid-content-around` to justify grid content with space around.

```html
<div class="grid justify-grid-items-start surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>

<div class="grid justify-grid-items-center surface-tertiary p-2 gap-2 mb-2">
...
</div>

<div class="grid justify-grid-items-end surface-tertiary p-2 gap-2 mb-2">
...
</div>

<div class="grid justify-grid-content-start surface-tertiary p-2 gap-2 mb-2">
...
</div>
<div class="grid justify-grid-content-center surface-tertiary p-2 gap-2 mb-2">
...
</div>
<div class="grid justify-grid-content-end surface-tertiary p-2 gap-2 mb-2">
...
</div>
<div class="grid justify-grid-content-between surface-tertiary p-2 gap-2 mb-2">
...
</div>
<div class="grid justify-grid-content-around surface-tertiary p-2 gap-2 mb-2">
...
</div>
```
<div class="component-preview d-block">
<code>.justify-grid-items-start</code>
<div class="grid grid-cols-3 justify-grid-items-start surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
   <div class="p-2 surface-primary">Item 4</div>
</div>
<code>.justify-grid-items-center</code>
<div class="grid grid-cols-3 justify-grid-items-center surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.justify-grid-items-end</code>
<div class="grid grid-cols-3 justify-grid-items-end surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.justify-grid-content-start</code>
<div class="grid  justify-grid-content-start surface-tertiary p-2 gap-2 mb-2 h-20">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.justify-grid-content-center</code>
<div class="grid  justify-grid-content-center surface-tertiary p-2 gap-2 mb-2 h-20">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
   <div class="p-2 surface-primary">Item 4</div>
</div>
<code>.justify-grid-content-end</code>
<div class="grid  justify-grid-content-end surface-tertiary p-2 gap-2 mb-2 h-20">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
   <div class="p-2 surface-primary">Item 4</div>
</div>
<code>.justify-grid-content-between</code>
<div class="grid justify-grid-content-between surface-tertiary p-2 gap-2 mb-2 h-20">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.justify-grid-content-around </code>
<div class="grid justify-grid-content-around surface-tertiary p-2 gap-2 mb-2 h-20">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
</div>
</div>

## Grid Alignment

#### Usage

- `.align-grid-items-start` to align grid items to the start.
- `.align-grid-items-end` to align grid items to the end.
- `.align-grid-items-center` to align grid items to the center.
- `.align-grid-content-start` to align grid content to the start.
- `.align-grid-content-end` to align grid content to the end.
- `.align-grid-content-center` to align grid content to the center.
- `.align-grid-content-stretch` to stretch grid content.

```html
<div class="grid align-grid-items-start surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<div class="grid align-grid-items-end surface-tertiary p-2 gap-2 mb-2">
...
</div>
<div class="grid align-grid-items-center surface-tertiary p-2 gap-2 mb-2">
...
</div>
<div class="grid align-grid-content-start surface-tertiary p-2 gap-2 mb-2">
...
</div>
<div class="grid align-grid-content-end surface-tertiary p-2 gap-2 mb-2">
...
</div>
<div class="grid align-grid-content-center surface-tertiary p-2 gap-2 mb-2">
...
</div>
<div class="grid align-grid-content-stretch surface-tertiary p-2 gap-2 mb-2">
...
</div>
```
<div class="component-preview d-block">
<code>.align-grid-items-start</code>
<div class="grid grid-cols-3  align-grid-items-start surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-grid-items-end</code>
<div class="grid grid-cols-3  align-grid-items-end surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-grid-items-center</code>
<div class="grid grid-cols-3  align-grid-items-center surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-grid-content-start</code>
<div class="grid grid-cols-3   align-grid-content-start surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-grid-content-end</code>
<div class="grid grid-cols-3  align-grid-content-end surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-grid-content-center</code>
<div class="grid grid-cols-3 align-grid-content-center surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-grid-content-stretch</code>
<div class="grid grid-cols-3 align-grid-content-stretch surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
</div>

## Responsive Grid Utilities

#### Usage
- `.grid-cols-{number}-{breakpoint}` to define the number of columns in the grid for a specific breakpoint.

```html
<div class="grid grid-cols-2 grid-cols-3-md surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- On small screens, a grid with 2 columns. On medium screens and above, a grid with 3 columns. -->

```
<div class="component-preview d-block">
<div class="grid grid-cols-2 grid-cols-3-md surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- On small screens, a grid with 2 columns. On medium screens and above, a grid with 3 columns. -->
</div>
