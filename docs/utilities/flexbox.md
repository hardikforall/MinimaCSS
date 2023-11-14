
# Flexbox Utilities

---

> [!NOTE]
> _The content on this page is currently in progress and not yet complete. I am working to fully develop and refine the information here to ensure it meets the high standards of comprehensiveness and clarity. Other pages in this documentation may be complete. I appreciate your patience and understanding as I continue to enhance this page._

---


This documentation offers a detailed guide to the flexbox utilities in MinimaCSS, crucial for building flexible and responsive web layouts.

## Flex Container
Flex Container:

#### Usage
- `.flex` for a standard flex container.
- `.flex-inline` for an inline flex container.

```html
<div class="flex surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are displayed in a row. -->
<div class="flex-inline surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are displayed inline in a row. -->
```
<div class="component-preview d-block">
<div class="flex surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<div class="flex-inline surface-tertiary p-2 gap-2 mt-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
</div>

## Flex Direction
Control the direction of flex items.

- `.flex-row` sets items in a row.
- `.flex-row-reverse` sets items in a reverse row.

```html
<div class="flex flex-row surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are laid out horizontally. -->
<div class="flex flex-row-reverse surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are laid out horizontally from opposite side. -->
```
<div class="component-preview d-block">
<div class="flex flex-row  surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<div class="flex flex-row-reverse surface-tertiary p-2 gap-2 mt-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
</div>


- `.flex-column` sets items in a row.
- `.flex-column-reverse` sets items in a reverse column.

```html
<div class="flex flex-column surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are laid out vertically. -->
<div class="flex flex-column-reverse surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are laid out vertically from opposite side. -->

```
<div class="component-preview d-block">
<div class="flex flex-column surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<div class="flex flex-column-reverse surface-tertiary p-2 gap-2 mt-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
</div>


## Justify Content
Align items horizontally.

- `.justify-content-start` Justify items to start of the container horizontally.
- `.justify-content-end` Justify items to end of the container horizontally.
- `.justify-content-center` Justify items to center of the container horizontally.
- `.justify-content-between` Justify items to between of the container horizontally.
- `.justify-content-around` Justify items to around of the container horizontally.
- `.justify-content-evenly` Justify items to evenly of the container horizontally.

```html
<div class="flex justify-content-start surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are justified horizontally to start of container. -->
<div class="flex justify-content-end surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are justified horizontally to end of container. -->
<div class="flex justify-content-center surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are justified horizontally to center of container -->
<div class="flex justify-content-between surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are justified horizontally in between of container. -->
<div class="flex justify-content-around surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are justified horizontally to around of container. -->
<div class="flex justify-content-evenly surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are justified horizontally and evenly of container. -->
```

<div class="component-preview d-block">
<code>.justify-content-start</code>
<div class="flex justify-content-start surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.justify-content-end</code>
<div class="flex justify-content-end surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.justify-content-center </code>
<div class="flex justify-content-center surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.justify-content-between</code>
<div class="flex justify-content-between surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.justify-content-around</code>
<div class="flex justify-content-around surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.justify-content-evenly</code>
<div class="flex justify-content-evenly surface-tertiary p-2 gap-2 mb-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
</div>



## Align Items
Align items vertically.

- `.align-items-start` Align items in to start of container vertically.
- `.align-items-end` Align items in to end of container vertically.
- `.align-items-center` Align items in to center of container vertically.
- `.align-items-baseline` Align items in to baseline of container vertically.
- `.align-items-stretch` Align items in to stretch of container vertically.

```html
<div class="flex align-items-start surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are aligned to start of the container Vertically. -->
<div class="flex align-items-end surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are aligned to end of the container Vertically. -->
<div class="flex align-items-center surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are aligned to center of the container Vertically. -->
<div class="flex align-items-baseline surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are aligned to baseline of the container Vertically. -->
<div class="flex align-items-stretch surface-tertiary p-2 gap-2">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<!-- Items are aligned to stretch across the container Vertically. -->
```

<div class="component-preview d-block">
<code>.align-items-start</code>
<div class="flex align-items-start surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-items-end</code>
<div class="flex align-items-end surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-items-center </code>
<div class="flex align-items-center surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-items-baseline</code>
<div class="flex align-items-baseline surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
<code>.align-items-stretch</code>
<div class="flex align-items-stretch surface-tertiary p-2 gap-2 mb-2 h-10">
   <div class="p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
   <div class="p-2 surface-primary">Item 3</div>
</div>
</div>

## Align Self
Utilize align-self utilities on individual flexbox items to customize their alignment on the cross axis. This axis is the y-axis by default, or the x-axis if `flex-direction` is set to column. You can select from options similar to align-items, which include `auto`, `start`, `end`, `center`, `baseline`, or `stretch` (the default setting in browsers).

- `.align-self-auto` place item to auto.
- `.align-self-start` place item to start of container.
- `.align-self-end` place item end of container.
- `.align-self-center` place item to center of container.
- `.align-self-baseline` place item to baseline  of container.
- `.align-self-stretch` stretch item across container.

```html
<div class="flex flex-row surface-tertiary p-2 gap-2 h-10">
   <div class="align-self-auto p-2 surface-primary">auto</div>
   <div class="align-self-start p-2 surface-primary">start</div>
   <div class="align-self-end p-2 surface-primary">end</div>
   <div class="align-self-center p-2 surface-primary">center</div>
   <div class="align-self-baseline p-2 surface-primary">baseline</div>
   <div class="align-self-stretch p-2 surface-primary">stretch</div>
</div>
<div class="flex flex-column surface-tertiary p-2 gap-2 mt-2">
   <div class="align-self-auto p-2 surface-primary">auto</div>
   <div class="align-self-start p-2 surface-primary">start</div>
   <div class="align-self-end p-2 surface-primary">end</div>
   <div class="align-self-center p-2 surface-primary">center</div>
   <div class="align-self-baseline p-2 surface-primary">baseline</div>
   <div class="align-self-stretch p-2 surface-primary">stretch</div>
</div>
```
<div class="component-preview d-block">
<pre>Flex row</pre>
<div class="flex flex-row surface-tertiary p-2 gap-2 h-10">
   <div class="align-self-auto p-2 surface-primary">auto</div>
   <div class="align-self-start p-2 surface-primary">start</div>
   <div class="align-self-end p-2 surface-primary">end</div>
   <div class="align-self-center p-2 surface-primary">center</div>
   <div class="align-self-baseline p-2 surface-primary">baseline</div>
   <div class="align-self-stretch p-2 surface-primary">stretch</div>
</div>
<pre>Flex column</pre>
<div class="flex flex-column surface-tertiary p-2 gap-2 mt-2">
   <div class="align-self-auto p-2 surface-primary">auto</div>
   <div class="align-self-start p-2 surface-primary">start</div>
   <div class="align-self-end p-2 surface-primary">end</div>
   <div class="align-self-center p-2 surface-primary">center</div>
   <div class="align-self-baseline p-2 surface-primary">baseline</div>
   <div class="align-self-stretch p-2 surface-primary">stretch</div>
</div>
</div>

## Grow and shrink
Apply the `.flex-grow-[]` utilities to control a flex item's capacity to expand and fill the available space. In the provided example, the .flex-grow-1 element occupies all the space it can, while still leaving sufficient space for the other two flex items.
Implement `.flex-shrink-[]` utilities to manage the shrinking capability of a flex item when needed. 

- `.flex-grow-1` The item will grow and will try to take available space.
- `.flex-shrink-1` The item will shrink whenever the space is needed
- `.flex-grow-0` will not grow
- `.flex-shrink-0` will not shrink

>`.flex-auto` class makes the element flexible by allowing it to grow and shrink based on available space and its content size. It's particularly useful in responsive layouts where you want elements to adjust their size dynamically to fit the container. This acts like `.flex-fill` from boostrp. 

```html
<div class="flex flex-row surface-tertiary p-2 gap-2 mt-2">
   <div class="flex-grow-1 p-2 surface-primary">Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
</div>
```
<div class="component-preview d-block">
<div class="flex flex-row surface-tertiary p-2 gap-2 mt-2">
   <div class="flex-grow-1 p-2 surface-primary">Grow Item 1</div>
   <div class="p-2 surface-primary">Item 2</div>
</div>
<div class="flex flex-row surface-tertiary p-2 gap-2 mt-2">
   <div class="w-full p-2 surface-primary ">Grow Item 1</div>
   <div class="flex-shrink-1 p-2 surface-primary">Shrink Item 2</div>
</div>
</div>

## Wrap
Alter the wrapping behavior of flex items within a flex container. You have the option to select from three settings: .flex-nowrap for no wrapping (which is the default behavior in browsers), .flex-wrap for standard wrapping, or .flex-wrap-reverse for wrapping in reverse order.

- `.flex-wrap` allows items to wrap onto multiple lines.
- `.flex-nowrap` do not allow items to wrap onto multiple lines.
- `.flex-wrap-reverse` allows items to wrap onto multiple lines and reverse the order.

```html
<div class="flex flex-row flex-wrap surface-tertiary p-2 gap-2 mb-2 h-10 ">
    <div class="p-2 surface-primary">Flex Item 1</div>
    <div class="p-2 surface-primary">Flex Item 2</div>
    <div class="p-2 surface-primary">Flex Item 3</div>        
    <div class="p-2 surface-primary">Flex Item 4</div>
    <div class="p-2 surface-primary">Flex Item 5</div>
    <div class="p-2 surface-primary">Flex Item 6</div>        
    <div class="p-2 surface-primary">Flex Item 7</div>
    <div class="p-2 surface-primary">Flex Item 8</div>
    <div class="p-2 surface-primary">Flex Item 9</div>
    <div class="p-2 surface-primary">Flex Item 10</div>
    <div class="p-2 surface-primary">Flex Item 11</div>
    <div class="p-2 surface-primary">Flex Item 12</div>
    <div class="p-2 surface-primary">Flex Item 13</div>
    <div class="p-2 surface-primary">Flex Item 14</div>
    <div class="p-2 surface-primary">Flex Item 15</div>
</div>
<div class="flex flex-row flex-nowrap surface-tertiary p-2 gap-2 mb-2 h-10 ">
...
</div>
<div class="flex flex-row flex-wrap-reverse surface-tertiary p-2 gap-2 mb-2 h-10 ">
...
</div>
```
<div class="component-preview d-block">
<code>.flex-wrap</code>
<div class="flex flex-row flex-wrap surface-tertiary p-2 gap-2 mb-2">
    <div class="p-2 surface-primary">Flex Item 1</div>
    <div class="p-2 surface-primary">Flex Item 2</div>
    <div class="p-2 surface-primary">Flex Item 3</div>        
    <div class="p-2 surface-primary">Flex Item 4</div>
    <div class="p-2 surface-primary">Flex Item 5</div>
    <div class="p-2 surface-primary">Flex Item 6</div>        
    <div class="p-2 surface-primary">Flex Item 7</div>
    <div class="p-2 surface-primary">Flex Item 8</div>
    <div class="p-2 surface-primary">Flex Item 9</div>
    <div class="p-2 surface-primary">Flex Item 10</div>
    <div class="p-2 surface-primary">Flex Item 11</div>
    <div class="p-2 surface-primary">Flex Item 12</div>
    <div class="p-2 surface-primary">Flex Item 13</div>
    <div class="p-2 surface-primary">Flex Item 14</div>
    <div class="p-2 surface-primary">Flex Item 15</div>
</div>
<code>.flex-nowrap</code>
<div class="flex flex-row flex-nowrap surface-tertiary p-2 gap-2 mb-2">
    <div class="p-2 surface-primary">Flex Item 1</div>
    <div class="p-2 surface-primary">Flex Item 2</div>
    <div class="p-2 surface-primary">Flex Item 3</div>        
    <div class="p-2 surface-primary">Flex Item 4</div>
    <div class="p-2 surface-primary">Flex Item 5</div>
    <div class="p-2 surface-primary">Flex Item 6</div>        
    <div class="p-2 surface-primary">Flex Item 7</div>
    <div class="p-2 surface-primary">Flex Item 8</div>
    <div class="p-2 surface-primary">Flex Item 9</div>
    <div class="p-2 surface-primary">Flex Item 10</div>
    <div class="p-2 surface-primary">Flex Item 11</div>
    <div class="p-2 surface-primary">Flex Item 12</div>
    <div class="p-2 surface-primary">Flex Item 13</div>
    <div class="p-2 surface-primary">Flex Item 14</div>
    <div class="p-2 surface-primary">Flex Item 15</div>
</div>
<code>.flex-wrap-reverse</code>
<div class="flex flex-row flex-wrap-reverse surface-tertiary p-2 gap-2 mb-2">
    <div class="p-2 surface-primary">Flex Item 1</div>
    <div class="p-2 surface-primary">Flex Item 2</div>
    <div class="p-2 surface-primary">Flex Item 3</div>        
    <div class="p-2 surface-primary">Flex Item 4</div>
    <div class="p-2 surface-primary">Flex Item 5</div>
    <div class="p-2 surface-primary">Flex Item 6</div>        
    <div class="p-2 surface-primary">Flex Item 7</div>
    <div class="p-2 surface-primary">Flex Item 8</div>
    <div class="p-2 surface-primary">Flex Item 9</div>
    <div class="p-2 surface-primary">Flex Item 10</div>
    <div class="p-2 surface-primary">Flex Item 11</div>
    <div class="p-2 surface-primary">Flex Item 12</div>
    <div class="p-2 surface-primary">Flex Item 13</div>
    <div class="p-2 surface-primary">Flex Item 14</div>
    <div class="p-2 surface-primary">Flex Item 15</div>
</div>
</div>


## Align content
Adjust the positioning of flex items within a flexbox container using the align-content property. This allows you to align items along the cross axis with several options: `start` (which is the default behavior in browsers), `end`, `center`, `between`, `around`, or `stretch`.

> Note: This property is ineffective on flex containers with only a single row of items.

- `.align-content-start` Align content to start of container.
- `.align-content-end` Align content to end of container.
- `.align-content-center` Align content to center of container.
- `.align-content-between` Align content in space between container.
- `.align-content-around` Align content around the container.

```html
<div class="flex align-content-start surface-tertiary p-2 gap-2">
...
</div>

<div class="flex align-content-end surface-tertiary p-2 gap-2">
 ...
</div>

<div class="flex align-content-center surface-tertiary p-2 gap-2">
 ...
</div>

<div class="flex align-content-between surface-tertiary p-2 gap-2">
 ...
</div>

<div class="flex align-content-around surface-tertiary p-2 gap-2">
  ...
</div>

<div class="flex align-content-stretch surface-tertiary p-2 gap-2">
  ...
</div>
```

<div class="component-preview d-block">
<code>. align-content-start</code>
<div class="flex align-content-start surface-tertiary p-2 gap-2 mb-2 h-10 flex-wrap">
        <div class="p-2 surface-primary">Flex Item 1</div>
        <div class="p-2 surface-primary">Flex Item 2</div>
        <div class="p-2 surface-primary">Flex Item 3</div>        
        <div class="p-2 surface-primary">Flex Item 4</div>
        <div class="p-2 surface-primary">Flex Item 5</div>
        <div class="p-2 surface-primary">Flex Item 6</div>        
        <div class="p-2 surface-primary">Flex Item 7</div>
        <div class="p-2 surface-primary">Flex Item 8</div>
        <div class="p-2 surface-primary">Flex Item 9</div>
        <div class="p-2 surface-primary">Flex Item 10</div>
        <div class="p-2 surface-primary">Flex Item 11</div>
        <div class="p-2 surface-primary">Flex Item 12</div>
        <div class="p-2 surface-primary">Flex Item 13</div>
        <div class="p-2 surface-primary">Flex Item 14</div>
        <div class="p-2 surface-primary">Flex Item 15</div>
</div>
<code>.align-content-end</code>
<div class="flex align-content-end surface-tertiary p-2 gap-2 mb-2 h-10 flex-wrap">
     <div class="p-2 surface-primary">Flex Item 1</div>
        <div class="p-2 surface-primary">Flex Item 2</div>
        <div class="p-2 surface-primary">Flex Item 3</div>        
        <div class="p-2 surface-primary">Flex Item 4</div>
        <div class="p-2 surface-primary">Flex Item 5</div>
        <div class="p-2 surface-primary">Flex Item 6</div>        
        <div class="p-2 surface-primary">Flex Item 7</div>
        <div class="p-2 surface-primary">Flex Item 8</div>
        <div class="p-2 surface-primary">Flex Item 9</div>
        <div class="p-2 surface-primary">Flex Item 10</div>
        <div class="p-2 surface-primary">Flex Item 11</div>
        <div class="p-2 surface-primary">Flex Item 12</div>
        <div class="p-2 surface-primary">Flex Item 13</div>
        <div class="p-2 surface-primary">Flex Item 14</div>
        <div class="p-2 surface-primary">Flex Item 15</div>

</div>
<code>.align-content-center </code>
<div class="flex align-content-center surface-tertiary p-2 gap-2 mb-2 h-10 flex-wrap">
     <div class="p-2 surface-primary">Flex Item 1</div>
        <div class="p-2 surface-primary">Flex Item 2</div>
        <div class="p-2 surface-primary">Flex Item 3</div>        
        <div class="p-2 surface-primary">Flex Item 4</div>
        <div class="p-2 surface-primary">Flex Item 5</div>
        <div class="p-2 surface-primary">Flex Item 6</div>        
        <div class="p-2 surface-primary">Flex Item 7</div>
        <div class="p-2 surface-primary">Flex Item 8</div>
        <div class="p-2 surface-primary">Flex Item 9</div>
        <div class="p-2 surface-primary">Flex Item 10</div>
        <div class="p-2 surface-primary">Flex Item 11</div>
        <div class="p-2 surface-primary">Flex Item 12</div>
        <div class="p-2 surface-primary">Flex Item 13</div>
        <div class="p-2 surface-primary">Flex Item 14</div>
        <div class="p-2 surface-primary">Flex Item 15</div>
</div>
<code>.align-content-between</code>
<div class="flex align-content-between surface-tertiary p-2 gap-2 mb-2 h-10 flex-wrap">
    <div class="p-2 surface-primary">Flex Item 1</div>
        <div class="p-2 surface-primary">Flex Item 2</div>
        <div class="p-2 surface-primary">Flex Item 3</div>        
        <div class="p-2 surface-primary">Flex Item 4</div>
        <div class="p-2 surface-primary">Flex Item 5</div>
        <div class="p-2 surface-primary">Flex Item 6</div>        
        <div class="p-2 surface-primary">Flex Item 7</div>
        <div class="p-2 surface-primary">Flex Item 8</div>
        <div class="p-2 surface-primary">Flex Item 9</div>
        <div class="p-2 surface-primary">Flex Item 10</div>
        <div class="p-2 surface-primary">Flex Item 11</div>
        <div class="p-2 surface-primary">Flex Item 12</div>
        <div class="p-2 surface-primary">Flex Item 13</div>
        <div class="p-2 surface-primary">Flex Item 14</div>
        <div class="p-2 surface-primary">Flex Item 15</div>
</div>
<code>.align-content-around</code>
<div class="flex align-content-around surface-tertiary p-2 gap-2 mb-2 h-10 flex-wrap">
      <div class="p-2 surface-primary">Flex Item 1</div>
        <div class="p-2 surface-primary">Flex Item 2</div>
        <div class="p-2 surface-primary">Flex Item 3</div>        
        <div class="p-2 surface-primary">Flex Item 4</div>
        <div class="p-2 surface-primary">Flex Item 5</div>
        <div class="p-2 surface-primary">Flex Item 6</div>        
        <div class="p-2 surface-primary">Flex Item 7</div>
        <div class="p-2 surface-primary">Flex Item 8</div>
        <div class="p-2 surface-primary">Flex Item 9</div>
        <div class="p-2 surface-primary">Flex Item 10</div>
        <div class="p-2 surface-primary">Flex Item 11</div>
        <div class="p-2 surface-primary">Flex Item 12</div>
        <div class="p-2 surface-primary">Flex Item 13</div>
        <div class="p-2 surface-primary">Flex Item 14</div>
        <div class="p-2 surface-primary">Flex Item 15</div>
</div>
<code>.align-content-stretch</code>
<div class="flex align-content-stretch surface-tertiary p-2 gap-2 mb-2 h-10 flex-wrap">
      <div class="p-2 surface-primary">Flex Item 1</div>
        <div class="p-2 surface-primary">Flex Item 2</div>
        <div class="p-2 surface-primary">Flex Item 3</div>        
        <div class="p-2 surface-primary">Flex Item 4</div>
        <div class="p-2 surface-primary">Flex Item 5</div>
        <div class="p-2 surface-primary">Flex Item 6</div>        
        <div class="p-2 surface-primary">Flex Item 7</div>
        <div class="p-2 surface-primary">Flex Item 8</div>
        <div class="p-2 surface-primary">Flex Item 9</div>
        <div class="p-2 surface-primary">Flex Item 10</div>
        <div class="p-2 surface-primary">Flex Item 11</div>
        <div class="p-2 surface-primary">Flex Item 12</div>
        <div class="p-2 surface-primary">Flex Item 13</div>
        <div class="p-2 surface-primary">Flex Item 14</div>
        <div class="p-2 surface-primary">Flex Item 15</div>
</div>
</div>




