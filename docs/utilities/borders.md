
# Border Utilities

This documentation outlines the border utilities available in MinimaCSS, enabling developers to style borders of elements effectively and responsively.

## Border Width Utilities
Control the width of borders.

 #### Usage
Use .border-[size] with sizes 1, 2, 3, 4, 5. etc. Default Border. without color specified adds default theme color of border - var(--border-primary-color)

#### Example
```html
<div class="border-1">1px border width</div>
<div class="border-3">3px border width</div>
```
<div class="component-preview d-block">
<div class="border-1">1px border width</div>
<div class="border-3">3px border width</div>

</div>


## Border Style Utilities
Define the style of borders.

 #### Usage
Apply .border-[style] with styles solid, dashed, dotted, double, none.

#### Example
```html
<div class="border-solid border-2">Solid border</div>
<div class="border-dashed border-3">Dashed border</div>
<div class="border-dotted border-3">Dotted border</div>
<div class="border-double border-3">Double border</div>
```

<div class="component-preview">
<div class="border-solid border-2">Solid border</div>
<div class="border-dashed border-3">Dashed border</div>
<div class="border-dotted border-3">Dotted border</div>
<div class="border-double border-3">Double border</div>
</div>

## Border Radius Utilities
Adjust the border radius.

 #### Usage
Use .rounded-[value] with values sm, md, lg, xl, full.

#### Example
```html
<div class="rounded-md border-1">Medium border radius</div>
<div class="rounded-full border-1">Fully rounded border</div>

```

<div class="component-preview">
<div class="rounded-md border-1">Medium border radius</div>
<div class="rounded-full border-1 w-10 h-10">Fully rounded border</div>
</div>

## Individual Side Border Utilities
Style individual sides of a border.

 #### Usage
Classes like .border-top-[size] and .border-right-[color-name].

#### Example
```html
<div class="border-0 border-top-4 p-1">Top border 2px</div>
<div class="border-0 border-right-4 border-top-4 border-right-primary border-top-warning p-1">Right border with primary color</div>
```

<div class="component-preview">
<div class="border-0 border-top-4 p-1">Top border 2px</div>
<div class="border-0 border-right-4 border-top-4 border-right-primary border-top-warning p-1">Right border with primary color</div>
</div>


## Border Reset Utility
Remove borders from elements.

 #### Usage
use `.border-none`

#### Example
```html
<div class="border-none">No border</div>
```

<div class="component-preview">
<div class="border-none">No border</div>
</div>