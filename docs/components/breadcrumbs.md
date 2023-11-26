# Breadcrumbs

Breadcrumbs are a type of navigation that display the user's current location within a website or application. They provide a hierarchy of pages or sections leading back to the home page.

The `.breadcrumbs` class is used to create a breadcrumb navigation container. Inside this container, each breadcrumb item is wrapped in a `<li>` element with the `.breadcrumbs-item` class.

To indicate the current page or active section, use the `.active` class on the corresponding breadcrumb item. Additionally, set the `aria-current` attribute to "page".

Example:

```html
<nav aria-label="breadcrumb">
  <ol class="breadcrumbs">
    <li class="breadcrumbs-item"><a href="#">Home</a></li>
    <li class="breadcrumbs-item"><a href="#">Library</a></li>
    <li class="breadcrumbs-item active" aria-current="page">Data</li>
  </ol>
</nav>
```

<div class="component-preview">
<nav aria-label="breadcrumb">
    <ol class="breadcrumbs">
        <li class="breadcrumbs-item"><a href="#">Home</a></li>
        <li class="breadcrumbs-item"><a href="#">Library</a></li>
        <li class="breadcrumbs-item active" aria-current="page">Data</li>
    </ol>
</nav>
</div>
