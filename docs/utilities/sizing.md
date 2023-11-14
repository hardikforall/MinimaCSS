
# Sizing Utilities 

This documentation details the sizing utilities in MinimaCSS, crucial for responsive design and layout control, incorporating the provided values for spacers, sizes, breakpoints, and overflows.

## Width and Height
Control element width and height.

 #### Usage
Apply .w-[size] and .h-[size], with sizes like 1rem, 2rem, up to 32rem, and special values like auto and full, vw, vh, sm, md, lg, xl, xxl.

Width and height utilities follwo mixed appraoch of rems and percentage. you can adjust width and height from 1 to 15 rem and then 10%, 20% and so on. 

#### Width Example
```html
<div class="w-5 p-4 surface-tertiary" >Width 5rem</div>
<div class="w-10 p-3 surface-tertiary" >Width 10rem</div>
<div class="w-25 p-3 surface-tertiary" >Width 25%</div>
<div class="w-50 p-3 surface-tertiary" >Width 50%</div>
<div class="w-75 p-3 surface-tertiary" >Width 75%</div>
<div class="w-100 p-3 surface-tertiary" >Width 100%</div>
<div class="w-auto p-3 surface-tertiary" >Width auto</div>
```
<div class="component-preview d-block">
<div class="bg-secondary position-relative gap-2" >
<div class="w-5 p-4 surface-tertiary mt-2" >Width 5rem</div>
<div class="w-10 p-3 surface-tertiary mt-2" >Width 10rem</div>
<div class="w-25 p-3 surface-tertiary mt-2" >Width 25%</div>
<div class="w-50 p-3 surface-tertiary mt-2" >Width 50%</div>
<div class="w-75 p-3 surface-tertiary mt-2" >Width 75%</div>
<div class="w-full p-3 surface-tertiary mt-2" >Width 100%</div>
<div class="w-auto p-3 surface-tertiary mt-2" >Width auto</div>
</div>
</div>

#### Height Example
```html
<div class="h-5 p-4 surface-tertiary" >Width 5rem</div>
<div class="h-10 p-3 surface-tertiary" >Width 10rem</div>
<div class="h-25 p-3 surface-tertiary" >Width 25%</div>
<div class="h-50 p-3 surface-tertiary" >Width 50%</div>
<div class="h-75 p-3 surface-tertiary" >Width 75%</div>
<div class="h-full p-3 surface-tertiary" >Width 100%</div>
<div class="h-auto p-3 surface-tertiary" >Width auto</div>
```
<div class="component-preview d-block">
<div class="bg-secondary position-relative " style="height:300px">
<div class="h-5 p-3 surface-tertiary d-inline-block " >Height 5rem</div>
<div class="h-8 p-3 surface-tertiary d-inline-block " >Height 8rem</div>
<div class="h-25 p-3 surface-tertiary d-inline-block " >Height 25%</div>
<div class="h-50 p-3 surface-tertiary d-inline-block " >Height 50%</div>
<div class="h-75 p-3 surface-tertiary d-inline-block " >Height 75%</div>
<div class="h-full p-3 surface-tertiary d-inline-block " >Height 100%</div>
<div class="h-auto p-3 surface-tertiary d-inline-block " >Height auto</div>
</div>
</div>

## Margin and Padding Utilities
Adjust spacing using predefined spacer values.

 #### Usage
Use .m-[size] and .p-[size], with size values ranging from 0 (0rem) to 10 (4.5rem).

#### Example
```html
<div class="m-3 surface-tertiary">Margin of 1rem</div>
<div class="p-5 surface-tertiary">Padding of 2rem</div>
<div class="ml-3 surface-tertiary">Margin of 1rem</div>
```

<div class="component-preview">
<div class="m-3 surface-tertiary">Margin of 1rem</div>
<div class="ml-3 surface-tertiary">Margin of 1rem left</div>
<div class="pl-3 surface-tertiary">Padding of 1rem left</div>
<div class="p-5 surface-tertiary">Padding of 2rem</div>
</div>

## Responsive Margin and Padding Utilities
 Apply different margin and padding at specified breakpoints.

 #### Usage
Classes like .m-[size]-[breakpoint] and .p-[size]-[breakpoint], with breakpoints sm, md, lg, xl, xxl.

```html
<div class="m-3-md">Margin of 1rem on medium (md) breakpoint</div>
<div class="p-5-lg">Padding of 2rem on large (lg) breakpoint</div>
```

<div class="component-preview">
<div class="m-3-md">Margin of 1rem on medium (md) breakpoint</div>
<div class="p-5-lg">Padding of 2rem on large (lg) breakpoint</div>
</div>

## Overflow Utilities
Manage content overflow behavior.

 #### Usage
Use .overflow-[value], .overflow-x-[value], .overflow-y-[value] with values like auto, hidden, scroll, visible.

```css
$overflows: (
  auto,
  hidden,
  scroll,
  visible
);
```

```html
<div class="overflow-auto  w-10 h-5">overflow auto: overflow auto: overflow auto: overflow auto: overflow auto:</div>
<div class="overflow-hidden  w-10 h-5">overflow hidden: overflow hidden: overflow hidden: overflow hidden: overflow hidden:</div>
<div class="overflow-visible  w-10 h-5">overflow visible: overflow visible: overflow visible: overflow visible: overflow visible:</div>
<div class="overflow-scroll  w-10 h-5">overflow scroll: overflow scroll: overflow scroll: overflow scroll: </div>
<div class="overflow-y-scroll  w-10 h-5">overflow y scroll: overflow y scroll: overflow y scroll: overflow y scroll: </div>
```

<div class="component-preview ">
<div class="overflow-auto  w-10 h-5">overflow auto: overflow auto: overflow auto: overflow auto: overflow auto:</div>
<div class="overflow-hidden  w-10 h-5">overflow hidden: overflow hidden: overflow hidden: overflow hidden: overflow hidden:</div>
<div class="overflow-visible  w-10 h-5">overflow visible: overflow visible: overflow visible: overflow visible: overflow visible:</div>
<div class="overflow-scroll  w-10 h-5">overflow scroll: overflow scroll: overflow scroll: overflow scroll: </div>
<div class="overflow-y-scroll  w-10 h-5">overflow y scroll: overflow y scroll: overflow y scroll: overflow y scroll: </div>
</div>