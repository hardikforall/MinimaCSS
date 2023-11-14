# Accordion

The Accordion component in MinimaCSS is a versatile UI element used for presenting content in a collapsible format. This component is particularly useful for FAQs, informational sections, and organizing content in a compact form. The accordion allows users to expand and collapse sections to reveal or hide information as needed.

### Usage

Accordions in MinimaCSS are created using the `<details>` and `<summary>` HTML elements. The `accordion-item` class is applied to the `<details>` element to style it as an accordion, and the `accordion-title` class is applied to the `<summary>` element to style the title of each accordion section. The content of the accordion is placed inside a `div` with the `accordion-content` class.

```html
<details class="accordion-item">
    <summary class="accordion-title">Accordion Title #1</summary>
    <div class="accordion-content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque urna diam, tincidunt nec porta
        sed, auctor id velit. Etiam venenatis nisl ut orci consequat, vitae tempus quam commodo. Nulla non
        mauris ipsum. Aliquam eu posuere orci. Nulla convallis lectus rutrum quam hendrerit, in facilisis elit
        sollicitudin. Mauris pulvinar pulvinar mi, dictum tristique elit auctor quis. Maecenas ac ipsum
        ultrices, porta turpis sit amet, congue turpis.
    </div>
</details>
<details class="accordion-item">
    <summary class="accordion-title">Accordion Title #2</summary>
    <div class="accordion-content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque urna diam, tincidunt nec porta
        sed, auctor id velit. Etiam venenatis nisl ut orci consequat, vitae tempus quam commodo. Nulla non
        mauris ipsum. Aliquam eu posuere orci. Nulla convallis lectus rutrum quam hendrerit, in facilisis elit
        sollicitudin. Mauris pulvinar pulvinar mi, dictum tristique elit auctor quis. Maecenas ac ipsum
        ultrices, porta turpis sit amet, congue turpis.
    </div>
</details>

```
<div class="component-preview">
<div class="w-full">
<details class="accordion-item">
    <summary class="accordion-title">Accordion Title #1</summary>
    <div class="accordion-content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque urna diam, tincidunt nec porta
        sed, auctor id velit. Etiam venenatis nisl ut orci consequat, vitae tempus quam commodo. Nulla non
        mauris ipsum. Aliquam eu posuere orci. Nulla convallis lectus rutrum quam hendrerit, in facilisis elit
        sollicitudin. Mauris pulvinar pulvinar mi, dictum tristique elit auctor quis. Maecenas ac ipsum
        ultrices, porta turpis sit amet, congue turpis.
    </div>
</details>

<details class="accordion-item">
    <summary class="accordion-title">Accordion Title #2</summary>
    <div class="accordion-content">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Pellentesque urna diam, tincidunt nec porta
        sed, auctor id velit. Etiam venenatis nisl ut orci consequat, vitae tempus quam commodo. Nulla non
        mauris ipsum. Aliquam eu posuere orci. Nulla convallis lectus rutrum quam hendrerit, in facilisis elit
        sollicitudin. Mauris pulvinar pulvinar mi, dictum tristique elit auctor quis. Maecenas ac ipsum
        ultrices, porta turpis sit amet, congue turpis.
    </div>
</details>
</div>

</div>