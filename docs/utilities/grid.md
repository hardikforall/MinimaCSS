# Grid Utilities

The grid system in MinimaCSS provides a powerful and flexible way to create responsive layouts in your web projects. It's based on a 12-column layout with support for various responsive breakpoints.

## Container

The container is used to center and constrain the width of your content.

#### Usage

- `.container` for a responsive fixed-width container
- `.container-fluid` for a full-width container

```html
<div class="container">
  <!-- Content here -->
</div>

<div class="container-fluid">
  <!-- Full-width content here -->
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Container</strong> (responsive fixed width)</p>
    <div class="container surface-tertiary p-2">
      <div class="surface-primary p-2 border border-primary">Container content</div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Container Fluid</strong> (full width)</p>
    <div class="container-fluid surface-tertiary p-2">
      <div class="surface-primary p-2 border border-primary">Container Fluid content</div>
    </div>
  </div>
</div>

## Row and Columns

The grid system uses rows and columns to layout content.

#### Basic Usage

```html
<div class="container">
  <div class="row">
    <div class="col-6">Half width column</div>
    <div class="col-6">Half width column</div>
  </div>
  <div class="row">
    <div class="col-4">One third</div>
    <div class="col-4">One third</div>
    <div class="col-4">One third</div>
  </div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Two equal columns</strong> (6 columns each)</p>
    <div class="container surface-tertiary p-2">
      <div class="row">
        <div class="col-6">
          <div class="surface-primary p-2 border border-primary">Half width column</div>
        </div>
        <div class="col-6">
          <div class="surface-primary p-2 border border-primary">Half width column</div>
        </div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Three equal columns</strong> (4 columns each)</p>
    <div class="container surface-tertiary p-2">
      <div class="row">
        <div class="col-4">
          <div class="surface-primary p-2 border border-primary">One third</div>
        </div>
        <div class="col-4">
          <div class="surface-primary p-2 border border-primary">One third</div>
        </div>
        <div class="col-4">
          <div class="surface-primary p-2 border border-primary">One third</div>
        </div>
      </div>
    </div>
  </div>
</div>

## Auto-layout Columns

#### Equal-width Columns

Use `.col` for equal width columns that automatically size based on the available space.

```html
<div class="row">
  <div class="col">Equal Width</div>
  <div class="col">Equal Width</div>
  <div class="col">Equal Width</div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Equal-width columns</strong> (auto sizing)</p>
    <div class="row surface-tertiary">
      <div class="col">
        <div class="surface-primary p-2 border border-primary">Equal Width</div>
      </div>
      <div class="col">
        <div class="surface-primary p-2 border border-primary">Equal Width</div>
      </div>
      <div class="col">
        <div class="surface-primary p-2 border border-primary">Equal Width</div>
      </div>
    </div>
  </div>
</div>

#### Auto-width Column

Use `.col-auto` for a column that only takes up the space it needs.

```html
<div class="row">
  <div class="col">Takes remaining space</div>
  <div class="col-auto">Auto width based on content</div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Auto-width column</strong> (only takes space it needs)</p>
    <div class="row surface-tertiary">
      <div class="col">
        <div class="surface-primary p-2 border border-primary">Takes remaining space</div>
      </div>
      <div class="col-auto">
        <div class="surface-primary p-2 border border-primary">Auto width</div>
      </div>
    </div>
  </div>
</div>

## Responsive Grid

The grid system includes six breakpoints for responsive layouts:

- Default (extra small): < 576px
- Small (sm): ≥ 576px
- Medium (md): ≥ 768px
- Large (lg): ≥ 992px
- Extra large (xl): ≥ 1200px
- Extra extra large (xxl): ≥ 1400px

#### Responsive Column Example

```html
<div class="row">
  <div class="col-12 col-md-6 col-lg-4">
    Responsive column: 12 columns on small screens, 6 on medium, 4 on large
  </div>
  <div class="col-12 col-md-6 col-lg-4">
    Responsive column: 12 columns on small screens, 6 on medium, 4 on large
  </div>
  <div class="col-12 col-md-12 col-lg-4">
    Responsive column: 12 columns on small screens, 12 on medium, 4 on large
  </div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Responsive columns</strong> (resize browser to see changes)</p>
    <div class="row surface-tertiary">
      <div class="col-12 col-md-6 col-lg-4">
        <div class="surface-primary p-2 border border-primary">
          12 columns on small screens, 6 on medium, 4 on large
        </div>
      </div>
      <div class="col-12 col-md-6 col-lg-4">
        <div class="surface-primary p-2 border border-primary">
          12 columns on small screens, 6 on medium, 4 on large
        </div>
      </div>
      <div class="col-12 col-md-12 col-lg-4">
        <div class="surface-primary p-2 border border-primary">
          12 columns on small screens, 12 on medium, 4 on large
        </div>
      </div>
    </div>
  </div>
</div>

## Column Offset

Use `.offset-*` classes to offset columns to the right.

```html
<div class="row">
  <div class="col-4">Column</div>
  <div class="col-4 offset-4">Offset column</div>
</div>
<div class="row">
  <div class="col-3 offset-3">Offset column</div>
  <div class="col-3 offset-3">Offset column</div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Basic offset</strong> (4 columns)</p>
    <div class="row surface-tertiary">
      <div class="col-4">
        <div class="surface-primary p-2 border border-primary">Column</div>
      </div>
      <div class="col-4 offset-4">
        <div class="surface-primary p-2 border border-primary">Offset column</div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Multiple offsets</strong> (3 columns each)</p>
    <div class="row surface-tertiary">
      <div class="col-3 offset-3">
        <div class="surface-primary p-2 border border-primary">Offset column</div>
      </div>
      <div class="col-3 offset-3">
        <div class="surface-primary p-2 border border-primary">Offset column</div>
      </div>
    </div>
  </div>
</div>

## Responsive Offset

Offsets can also be responsive:

```html
<div class="row">
  <div class="col-sm-4 offset-sm-4 col-md-3 offset-md-0">
    Responsive offset: centered on small screens, left-aligned on medium+
  </div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Responsive offset</strong> (resize browser to see changes)</p>
    <div class="row surface-tertiary">
      <div class="col-sm-4 offset-sm-4 col-md-3 offset-md-0">
        <div class="surface-primary p-2 border border-primary">
          Centered on small screens, left-aligned on medium+
        </div>
      </div>
    </div>
  </div>
</div>

## Row Alignment

### Horizontal Alignment

Control the horizontal alignment of columns within a row.

```html
<div class="row row-start">
  <div class="col-4">Left aligned (default)</div>
</div>
<div class="row row-center">
  <div class="col-4">Center aligned</div>
</div>
<div class="row row-end">
  <div class="col-4">Right aligned</div>
</div>
<div class="row row-around">
  <div class="col-2">Space around</div>
  <div class="col-2">Space around</div>
</div>
<div class="row row-between">
  <div class="col-2">Space between</div>
  <div class="col-2">Space between</div>
</div>
<div class="row row-evenly">
  <div class="col-2">Space evenly</div>
  <div class="col-2">Space evenly</div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Left aligned</strong> (default)</p>
    <div class="row row-start surface-tertiary">
      <div class="col-4">
        <div class="surface-primary p-2 border border-primary">Left aligned</div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Center aligned</strong></p>
    <div class="row row-center surface-tertiary">
      <div class="col-4">
        <div class="surface-primary p-2 border border-primary">Center aligned</div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Right aligned</strong></p>
    <div class="row row-end surface-tertiary">
      <div class="col-4">
        <div class="surface-primary p-2 border border-primary">Right aligned</div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Space around</strong></p>
    <div class="row row-around surface-tertiary">
      <div class="col-2">
        <div class="surface-primary p-2 border border-primary">Space around</div>
      </div>
      <div class="col-2">
        <div class="surface-primary p-2 border border-primary">Space around</div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Space between</strong></p>
    <div class="row row-between surface-tertiary">
      <div class="col-2">
        <div class="surface-primary p-2 border border-primary">Space between</div>
      </div>
      <div class="col-2">
        <div class="surface-primary p-2 border border-primary">Space between</div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Space evenly</strong></p>
    <div class="row row-evenly surface-tertiary">
      <div class="col-2">
        <div class="surface-primary p-2 border border-primary">Space evenly</div>
      </div>
      <div class="col-2">
        <div class="surface-primary p-2 border border-primary">Space evenly</div>
      </div>
    </div>
  </div>
</div>

### Vertical Alignment

Control the vertical alignment of columns within a row.

```html
<div class="row row-items-start" style="height: 100px;">
  <div class="col-4">Top aligned</div>
</div>
<div class="row row-items-center" style="height: 100px;">
  <div class="col-4">Center aligned</div>
</div>
<div class="row row-items-end" style="height: 100px;">
  <div class="col-4">Bottom aligned</div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Top aligned</strong></p>
    <div class="row row-items-start surface-tertiary" style="height: 100px;">
      <div class="col-4">
        <div class="surface-primary p-2 border border-primary">Top aligned</div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Center aligned</strong> (vertically)</p>
    <div class="row row-items-center surface-tertiary" style="height: 100px;">
      <div class="col-4">
        <div class="surface-primary p-2 border border-primary">Center aligned</div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>Bottom aligned</strong></p>
    <div class="row row-items-end surface-tertiary" style="height: 100px;">
      <div class="col-4">
        <div class="surface-primary p-2 border border-primary">Bottom aligned</div>
      </div>
    </div>
  </div>
</div>

## Row Gutter Modifiers

Control the spacing between columns. The grid system includes different gutter options to adjust the spacing between columns.

```html
<div class="row">
  <div class="col-6">Default gutter</div>
  <div class="col-6">Default gutter</div>
</div>
<div class="row row-no-gutters">
  <div class="col-6">No gutters</div>
  <div class="col-6">No gutters</div>
</div>
<div class="row row-gutter-sm">
  <div class="col-6">Small gutters</div>
  <div class="col-6">Small gutters</div>
</div>
<div class="row row-gutter-lg">
  <div class="col-6">Large gutters</div>
  <div class="col-6">Large gutters</div>
</div>
```

<div class="component-preview d-block">
  <!-- Default gutters -->
  <div class="mb-4">
    <p class="mb-2"><strong>Default gutters</strong> (15px on each side)</p>
    <div class="row surface-tertiary">
      <div class="col-6">
        <div class="surface-primary p-2 border border-primary">Column with default gutter</div>
      </div>
      <div class="col-6">
        <div class="surface-primary p-2 border border-primary">Column with default gutter</div>
      </div>
    </div>
  </div>
  
  <!-- No gutters -->
  <div class="mb-4">
    <p class="mb-2"><strong>No gutters</strong> (0px spacing)</p>
    <div class="row row-no-gutters surface-tertiary">
      <div class="col-6">
        <div class="surface-primary p-2 border border-primary">Column with no gutter</div>
      </div>
      <div class="col-6">
        <div class="surface-primary p-2 border border-primary">Column with no gutter</div>
      </div>
    </div>
  </div>
  
  <!-- Small gutters -->
  <div class="mb-4">
    <p class="mb-2"><strong>Small gutters</strong> (7.5px on each side)</p>
    <div class="row row-gutter-sm surface-tertiary">
      <div class="col-6">
        <div class="surface-primary p-2 border border-primary">Column with small gutter</div>
      </div>
      <div class="col-6">
        <div class="surface-primary p-2 border border-primary">Column with small gutter</div>
      </div>
    </div>
  </div>
  
  <!-- Large gutters -->
  <div class="mb-4">
    <p class="mb-2"><strong>Large gutters</strong> (30px on each side)</p>
    <div class="row row-gutter-lg surface-tertiary">
      <div class="col-6">
        <div class="surface-primary p-2 border border-primary">Column with large gutter</div>
      </div>
      <div class="col-6">
        <div class="surface-primary p-2 border border-primary">Column with large gutter</div>
      </div>
    </div>
  </div>
</div>

## Column Order

Control the visual order of columns.

```html
<div class="row">
  <div class="col order-3">First in DOM, third in display</div>
  <div class="col order-2">Second in DOM, second in display</div>
  <div class="col order-1">Third in DOM, first in display</div>
</div>
<div class="row">
  <div class="col order-last">First in DOM, last in display</div>
  <div class="col">Middle in DOM and display</div>
  <div class="col order-first">Last in DOM, first in display</div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Numeric ordering</strong></p>
    <div class="row surface-tertiary">
      <div class="col order-3">
        <div class="surface-primary p-2 border border-primary">First in DOM, third in display</div>
      </div>
      <div class="col order-2">
        <div class="surface-primary p-2 border border-primary">Second in DOM, second in display</div>
      </div>
      <div class="col order-1">
        <div class="surface-primary p-2 border border-primary">Third in DOM, first in display</div>
      </div>
    </div>
  </div>
  
  <div class="mb-4">
    <p class="mb-2"><strong>First/last ordering</strong></p>
    <div class="row surface-tertiary">
      <div class="col order-last">
        <div class="surface-primary p-2 border border-primary">First in DOM, last in display</div>
      </div>
      <div class="col">
        <div class="surface-primary p-2 border border-primary">Middle in DOM and display</div>
      </div>
      <div class="col order-first">
        <div class="surface-primary p-2 border border-primary">Last in DOM, first in display</div>
      </div>
    </div>
  </div>
</div>

## Responsive Order

Order can also be responsive:

```html
<div class="row">
  <div class="col order-2 order-md-1">
    Second on small screens, first on medium+
  </div>
  <div class="col order-1 order-md-2">
    First on small screens, second on medium+
  </div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Responsive ordering</strong> (resize browser to see changes)</p>
    <div class="row surface-tertiary">
      <div class="col order-2 order-md-1">
        <div class="surface-primary p-2 border border-primary">
          Second on small screens, first on medium+
        </div>
      </div>
      <div class="col order-1 order-md-2">
        <div class="surface-primary p-2 border border-primary">
          First on small screens, second on medium+
        </div>
      </div>
    </div>
  </div>
</div>

## Nesting

Rows can be nested inside columns to create more complex layouts.

```html
<div class="row">
  <div class="col-8">
    <div class="p-2 surface-primary">Parent column</div>
    <div class="row">
      <div class="col-6">
        <div class="p-2 surface-secondary">Nested column</div>
      </div>
      <div class="col-6">
        <div class="p-2 surface-secondary">Nested column</div>
      </div>
    </div>
  </div>
  <div class="col-4">
    <div class="p-2 surface-primary h-100">Parent column</div>
  </div>
</div>
```

<div class="component-preview d-block">
  <div class="mb-4">
    <p class="mb-2"><strong>Nested grid</strong></p>
    <div class="row surface-tertiary">
      <div class="col-8">
        <div class="surface-primary p-2 border border-primary mb-2">Parent column</div>
        <div class="row">
          <div class="col-6">
            <div class="surface-secondary p-2 border border-secondary">Nested column</div>
          </div>
          <div class="col-6">
            <div class="surface-secondary p-2 border border-secondary">Nested column</div>
          </div>
        </div>
      </div>
      <div class="col-4">
        <div class="surface-primary p-2 border border-primary h-100">Parent column</div>
      </div>
    </div>
  </div>
</div>

## CSS Grid Utilities

In addition to the flexbox-based grid system, MinimaCSS also provides CSS Grid utilities as documented in the [Grid Utilities](../utilities/grid.md) section.
