# Tooltip

The Tooltip component is a user interface element that provides additional information to users when they hover over a target element. It's commonly used to explain functions of buttons, links, or other UI elements. This Tooltip component is versatile, offering multiple placement options like top, left, right, and bottom.

## Usage

The Tooltip component is implemented with HTML and uses data attributes to determine the content and placement of the tooltip. Below is a detailed explanation of its structure and usage.

### Data Attributes

- `data-tooltip`: Specifies the text to be displayed in the tooltip.
- `data-placement`: Determines the placement of the tooltip (top, left, right, bottom).

### CSS Class

- `tooltip`: Base class for the tooltip component.

### HTML Structure



```html
<!-- Tooltip on top -->
<div class="tooltip" data-tooltip="Tooltip on top" data-placement="top">
    Hover over me
</div>

<!-- Tooltip on left -->
<div class="tooltip" data-tooltip="Tooltip on the left" data-placement="left">
    Hover over me
</div>

<!-- Tooltip on right -->
<div class="tooltip" data-tooltip="Tooltip on the right" data-placement="right">
    Hover over me
</div>

<!-- Tooltip on bottom -->
<div class="tooltip" data-tooltip="Tooltip on bottom" data-placement="bottom">
    Hover over me
</div>
```

<div class="component-preview">
<!-- Tooltip on top -->
<div class="tooltip" data-tooltip="Tooltip on top" data-placement="top">
    Hover over me
</div>

<!-- Tooltip on left -->
<div class="tooltip" data-tooltip="Tooltip on the left" data-placement="left">
    Hover over me
</div>

<!-- Tooltip on right -->
<div class="tooltip" data-tooltip="Tooltip on the right" data-placement="right">
    Hover over me
</div>

<!-- Tooltip on bottom -->
<div class="tooltip" data-tooltip="Tooltip on bottom" data-placement="bottom">
    Hover over me
</div>
</div>

