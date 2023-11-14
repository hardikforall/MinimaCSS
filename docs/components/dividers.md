# Dividers

Dividers are used to separate content and create visual hierarchy in a user interface. MinimaCSS provides several types of dividers that can be used to divide sections or elements within a page.

## Horizontal Divider

To add a horizontal divider, use the `<hr>` element with the class `hr-divider`.

```html
<hr class="hr-divider">
```
<div class="component-preview d-block">
<hr class="hr-divider">
</div>

## Vertical Divider

For a vertical divider, use a `<div>` element with the class `vr-divider`. You can adjust the height and alignment of the divider using CSS.

```html
<div>Content on the left</div>
<span class="vr-divider"></span>
<div>Content on the right</div>

```
<div class="component-preview d-block">
<div style="display: flex; align-items: center; height:100px">
    <div>Content on the left</div>
    <span class="vr-divider"></span>
    <div>Content on the right</div>
</div>
</div>

## Dashed Divider

To create a dashed divider, use the `<hr>` element with the class `dashed-divider`.

```html
<hr class="dashed-divider">
```
<div class="component-preview d-block">
<hr class="dashed-divider" style="border-top: 2px dashed var(--border-primary-color); border-bottom:0px;">
</div>

## Text Divider

A text divider can be used to label sections or provide visual separation between content. Use the `<div>` element with the class `text-divider` and add the desired title or text inside.

```html
<div class="text-divider">Section Title</div>
```
<div class="component-preview d-block">
<div class="text-divider">Section Title</div>
</div>