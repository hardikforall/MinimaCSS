# Color Utilities

This document provides a foundational understanding of the color utilities in MinimaCSS, with examples and component previews to aid in practical implementation

## Text Color

Text color utilities are based on the color variables defined in `_variables.scss`. They allow for the straightforward application of color to text.

#### Usage

To use a text color utility, add a `.text-[color]` class to an HTML element, where `[color]` corresponds to a color variable.

#### Example

```html
<p class="text-primary">Primary color text</p>
<p class="text-secondary">Secondary color text</p>
<p class="text-success">Success color text</p>
<p class="text-danger">Danger color text</p>
<p class="text-warning">Warning color text</p>
<p class="text-info">Info color text</p>
<p class="text-light">Light color text</p>
<p class="text-dark">Dark color text</p>
```

<div class="component-preview d-block">
<p class="text-primary">Primary color text</p>
<p class="text-secondary">Secondary color text</p>
<p class="text-success">Success color text</p>
<p class="text-danger">Danger color text</p>
<p class="text-warning">Warning color text</p>
<p class="text-info">Info color text</p>
<p class="text-light">Light color text</p>
<p class="text-dark">Dark color text</p>
</div>

## Surface Color (Support theme)

Surface color utilities are used to apply background colors to elements. These Colors support Light and dark By default.

#### Usage

Classes such as `.surface-primary`, `.surface-secondary`, and `.surface-tertiary` apply predefined background colors.

#### Example

```html
<div class="surface-primary">Primary surface</div>
<div class="surface-secondary">Secondary surface</div>
<div class="surface-tertiary">Tertiary surface</div>
```

<div class="component-preview">
<div class="surface-primary p-4">Primary surface</div>
<div class="surface-secondary p-4">Secondary surface</div>
<div class="surface-tertiary p-4">Tertiary surface</div>
</div>

## Background Color

Background color utilities are used to apply background colors to elements.

#### Usage

Classes such as `.bg-primary`, `.bg-secondary`, etc. apply predefined background colors.

#### Example

```html
<div class="bg-primary">Primary Background</div>
<div class="bg-secondary">Secondary Background</div>
<div class="bg-success">Success Background</div>
<div class="bg-danger">Danger Background</div>
<div class="bg-warning">Warning Background</div>
<div class="bg-info">Info Background</div>
<div class="bg-light">Light Background</div>
<div class="bg-dark">Dark Background</div>
```

<div class="component-preview">
<div class="bg-primary p-4 text-light">Primary Background</div>
<div class="bg-secondary p-4 text-light">Secondary Background</div>
<div class="bg-success p-4 text-light">Success Background</div>
<div class="bg-danger p-4 text-light">Danger Background</div>
<div class="bg-warning p-4 text-light">Warning Background</div>
<div class="bg-info p-4 text-light">Info Background</div>
<div class="bg-light p-4 text-dark">Light Background</div>
<div class="bg-dark p-4 text-light">Dark Background</div>
</div>
