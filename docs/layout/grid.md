The Grid System is a powerful layout tool for creating responsive web designs. It is similar to the Bootstrap grid system, employing a series of containers, rows, and columns to layout and align content. This system is built on a flexbox layout and is fully responsive.

## Usage

The Grid System uses a series of containers, rows, and columns to control the layout. Below is a detailed explanation of its structure and usage.

### Containers

Containers provide a means to center and horizontally pad your site's contents. Use `.container` for a responsive fixed-width container.

```html
<div class="container">
  <!-- Content here -->
</div>
```

### Rows

A row is used to create horizontal groups of columns. Use `.row` to ensure proper alignment and spacing.

```html
<div class="row">
  <!-- Columns here -->
</div>
```

### Columns

Columns are used to create the individual columns within a row. Use `.col`, `.col-{breakpoint}-{size}` to define the column size and responsiveness.

```html
<div class="col">
  <!-- Column content -->
</div>
```

### Breakpoints

The grid system is based on the following breakpoints:

- `col-xs`: Extra small devices (portrait phones)
- `col-sm`: Small devices (landscape phones)
- `col-md`: Medium devices (tablets)
- `col-lg`: Large devices (desktops)
- `col-xl`: Extra large devices (large desktops)

### Example

Here is an example of a grid layout:

```html
<div class="container">
  <div class="row">
    <div class="col-md-8">.col-md-8</div>
    <div class="col-md-4">.col-md-4</div>
  </div>
</div>
```

<div class="component-preview d-block">
  <div class="container">
  <div class="row">
    <div class="col-md-8">.col-md-8</div>
    <div class="col-md-4">.col-md-4</div>
  </div>
</div>
</div>
