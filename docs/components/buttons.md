# Buttons
Buttons are a fundamental interactive element in any user interface. MinimaCSS provides a range of button styles that are easily customizable and adaptable to your design needs.

## Button Variants

Here is the base button without any styling

```html
<button class="btn">Base</button>
```

<div class="component-preview">
<button class="btn">Base</button>
</div>

### Solid Buttons
The solid buttons come with a default style that is bold and eye-catching. They are used for primary actions.

```html
<button class="btn btn-primary">Primary</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-info">Info</button>
<button class="btn btn-warning">Warning</button>
<button class="btn btn-danger">Danger</button>
<button class="btn btn-dark">Dark</button>
<button class="btn btn-light">Light</button>
```

<div class="component-preview">
<button class="btn btn-primary">Primary</button>
<button class="btn btn-error">Error</button>
<button class="btn btn-success">Success</button>
<button class="btn btn-warning">Warning</button>
<button class="btn btn-info">Info</button>
<button class="btn btn-light">Light</button>
<button class="btn btn-dark">Dark</button>
<button class="btn btn-link">Link</button>
</div>

### Outline Buttons
Outline buttons are used for less pronounced actions and pair well with solid buttons for hierarchy.

```html
<button class="btn btn-outline-primary">Primary</button>
<button class="btn btn-outline-error">Error</button>
<button class="btn btn-outline-success">Success</button>
<button class="btn btn-outline-warning">Warning</button>
<button class="btn btn-outline-info">Info</button>
<button class="btn btn-outline-light">Light</button>
<button class="btn btn-outline-dark">Dark</button>
```
<div class="component-preview">
<button class="btn btn-outline-primary">Primary</button>
<button class="btn btn-outline-error">Error</button>
<button class="btn btn-outline-success">Success</button>
<button class="btn btn-outline-warning">Warning</button>
<button class="btn btn-outline-info">Info</button>
<button class="btn btn-outline-light">Light</button>
<button class="btn btn-outline-dark">Dark</button>
</div>

## Sizes
You can choose from a range of sizes for buttons to suit your design.

```html
<button class="btn btn-primary btn-sm">Small</button>
<button class="btn btn-primary btn-md">Medium</button>
<button class="btn btn-primary ">Base</button>
<button class="btn btn-primary btn-lg">Large</button>
```

<div class="component-preview">
<button class="btn btn-primary btn-sm">Small</button>
<button class="btn btn-primary btn-md">Medium</button>
<button class="btn btn-primary ">Base</button>
<button class="btn btn-primary btn-lg">Large</button>
</div>

## Block Buttons
Block level buttons extend the full width of a parent.

```html
<button class="btn btn-primary btn-block">Block Level</button>
```

<div class="component-preview">
<button class="btn btn-primary btn-block">Block Level</button>
</div>

## Icon Buttons
Icon buttons can be used for showing icons in buttons

```html
<button class="btn btn-primary m-1 "><span class="material-symbols-rounded">add_circle</span>Icon Button</button>
```

<div class="component-preview">
<button class="btn btn-primary m-1 "><span class="material-symbols-rounded">add_circle</span>Icon Button</button>
</div>

### Round Buttons

```html
<button class="btn btn-primary btn-round m-1"><span class="material-symbols-rounded">add</span></button>
<button class="btn btn-outline-primary btn-round m-1"><span class="material-symbols-rounded">shopping_cart</span></button>
```

<div class="component-preview">
<button class="btn btn-primary btn-round m-1"><span class="material-symbols-rounded">add</span></button>
<button class="btn btn-outline-primary btn-round m-1"><span class="material-symbols-rounded">shopping_cart</span></button>
</div>

## Button Groups

Group buttons together for a unified component using the `.btn-group` class:

```html
<div class="btn-group">
  <button class="btn btn-primary">Left</button>
  <button class="btn btn-primary">Middle</button>
  <button class="btn btn-primary">Right</button>
</div>
<div class="btn-group">
  <button class="btn btn-outline-primary">Left</button>
  <button class="btn btn-outline-primary">Middle</button>
  <button class="btn btn-outline-primary">Right</button>
</div>
```


<div class="component-preview">
<div class="btn-group">
  <button class="btn btn-primary">Left</button>
  <button class="btn btn-primary">Middle</button>
  <button class="btn btn-primary">Right</button>
</div>
<div class="btn-group">
  <button class="btn btn-outline-primary">Left</button>
  <button class="btn btn-outline-primary">Middle</button>
  <button class="btn btn-outline-primary">Right</button>
</div>
</div>


## Dropdown Buttons

Dropdown buttons are created using the `.dropdown` class in conjunction with `.dropdown-toggle` and `.dropdown-menu`:

```html
<details class="dropdown">
  <summary class="dropdown-toggle btn btn-primary">
    Dropdown Button
  </summary>
  <div class="dropdown-menu">
    <a class="dropdown-item" href="#">Action</a>
    <!-- ... more dropdown items ... -->
  </div>
</details>
```

<div class="component-preview">
<details class="dropdown">
   <summary class="dropdown-toggle btn btn-primary">
     Dropdown Button
   </summary>
   <div class="dropdown-menu">
      <a class="dropdown-item" href="#">Action</a>
      <a class="dropdown-item" href="#">Another action</a>
      <a class="dropdown-item" href="#">Something else here</a>
  </div>
</details>
</div>


## SCSS Mixin for Button Variants
The SCSS for MinimaCSS buttons includes mixins for creating different styles and states of buttons.

```css
// SCSS Mixin Example
@mixin button-variant($color, $hover-color, $text-color, $focus-ring, $type: solid) {
    ...
}
```

Utilize this mixin to customize button styles throughout your project.

At the bottom of your styling files, the SCSS for buttons is defined with mixins for easy customization and extendability. The `button-variant` mixin creates the core styles for each button type. For a detailed look at the SCSS structure and how to use the mixins, refer to the `_buttons.scss` file included with MinimaCSS.

