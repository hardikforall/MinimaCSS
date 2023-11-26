# Hover State Utilities

---

> [!NOTE] > _The content on this page is currently in progress and not yet complete. I am working to fully develop and refine the information here to ensure it meets the high standards of comprehensiveness and clarity. Other pages in this documentation may be complete. I appreciate your patience and understanding as I continue to enhance this page._

---

This section provides utility classes for applying hover styles to elements based on color values defined in the `$colors` variable.

## Usage

### Background color

- `.hover-bg-{color-name}`: Applies the background color specified by `{color-name}` when the element is hovered.

### Text color

- `.hover-text-{color-name}`: Applies the text color specified by `{color-name}` when the element is hovered.

### Border color

- `.hover-border-{color-name}`: Applies the border color specified by `{color-name}` when the element is hovered.

```html
<button class="hover-bg-primary">Hover me</button>
<p class="hover-text-secondary">Hover me</p>
<input class="hover-border-danger" type="text" placeholder="Hover me" />
```

## Focus State Utilities

This section provides utility classes for applying focus styles to elements based on color values defined in the `$colors` variable.

### Background color

- `.focus-bg-{color-name}`: Applies the background color specified by `{color-name}` when the element is focused.

### Text color

- `.focus-text-{color-name}`: Applies the text color specified by `{color-name}` when the element is focused.

### Border color

- `.focus-border-{color-name}`: Applies the border color specified by `{color-name}` when the element is focused.

```html
<button class="focus-bg-primary">Focus me</button>
<p class="focus-text-secondary">Focus me</p>
<input class="focus-border-danger" type="text" placeholder="Focus me" />
```

## Active State Utilities

This section provides utility classes for applying active styles to elements based on color values defined in the `$colors` variable.

### Background color

- `.active-bg-{color-name}`: Applies the background color specified by `{color-name}` when the element is active.

### Text color

- `.active-text-{color-name}`: Applies the text color specified by `{color-name}` when the element is active.

### Border color

- `.active-border-{color-name}`: Applies the border color specified by `{color-name}` when the element is active.

```html
<button class="active-bg-primary">Click me</button>
<p class="active-text-secondary">Click me</p>
<input class="active-border-danger" type="text" placeholder="Click me" />
```

## Cursor Utilities

This section provides utility classes for customizing the cursor style of elements.

- `.cursor-pointer`: Sets the cursor to a pointer.
- `.cursor-default`: Sets the cursor to the default.
- `.cursor-move`: Sets the cursor to a move.
- `.cursor-not-allowed`: Sets the cursor to not-allowed.

```html
<button class="cursor-pointer">Pointer cursor</button>
<p class="cursor-move">Move cursor</p>
<div class="cursor-not-allowed">Not allowed cursor</div>
```

## Transition Utilities

This section provides utility classes for applying smooth transitions to elements.

- `.transition`: Applies a transition with a duration of 0.3 seconds and an easing function.
- `.transition-fast`: Applies a faster transition with a duration of 0.15 seconds and an easing function.
- `.transition-slow`: Applies a slower transition with a duration of 0.5 seconds and an easing function.

```html
<button class="transition">Smooth transition</button>
<p class="transition-fast">Faster transition</p>
<div class="transition-slow">Slower transition</div>
```

## Transform Utilities

This section provides utility classes for applying transformations to elements.

- `.scale-hover:hover`: Scales the element to 1.1 times its original size when hovered.
- `.rotate-hover:hover`: Rotates the element by 5 degrees when hovered.

```html
<div class="scale-hover">Hover me to scale</div>
<div class="rotate-hover">Hover me to rotate</div>
```

## Opacity Utilities

This section provides utility classes for adjusting the opacity of elements.

- `.opacity-{value}`: Sets the opacity of the element to the specified `{value}` (0 to 10, where 0 is completely transparent and 10 is fully opaque).
- `.opacity-hover:hover`: Sets the opacity of the element to 0.8 when hovered.

```html
<div class="opacity-5">Opacity 0.5</div>
<div class="opacity-hover">Hover me to change opacity</div>
```
