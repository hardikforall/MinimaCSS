# Position Utilities

---

> [!NOTE] > _The content on this page is currently in progress and not yet complete. I am working to fully develop and refine the information here to ensure it meets the high standards of comprehensiveness and clarity. Other pages in this documentation may be complete. I appreciate your patience and understanding as I continue to enhance this page._

---

This documentation offers a detailed guide to the position utilities in MinimaCSS, which provide flexibility and control over the positioning of elements on a web page.

## Position Classes

The position classes in MinimaCSS allow you to easily set the position of an element.

#### Usage

- `.position-static` to set the position property to static.
- `.position-relative` to set the position property to relative.
- `.position-absolute` to set the position property to absolute.
- `.position-fixed` to set the position property to fixed.
- `.position-sticky` to set the position property to sticky.

```html
<div class="position-static">This div has a static position.</div>
<div class="position-relative">This div has a relative position.</div>
<div class="position-absolute">This div has an absolute position.</div>
<div class="position-fixed">This div has a fixed position.</div>
<div class="position-sticky">This div has a sticky position.</div>
```

<div class="component-preview d-block position-relative">
<div class="position-static surface-tertiary text-white p-2 mb-2 h-5 w-5">static</div>
<div class="position-relative surface-tertiary text-white p-2 mb-2 h-5 w-5">relative</div>
<div class="position-absolute surface-tertiary text-white p-2 mb-2 h-5 w-5">absolute</div>
<div class="position-fixed surface-tertiary text-white p-2 mb-2 h-5 w-5 right-0 top-0">Fixed</div>
<div class="position-sticky surface-tertiary text-white p-2 mb-2 h-5 w-5 ">sticky</div>
</div>

## Spacing Utilities

The spacing utilities in MinimaCSS allow you to easily set the top, right, bottom, and left properties of an element.

#### Usage

The available spacing classes range from `top-0` to `top-10`, `right-0` to `right-10`, `bottom-0` to `bottom-10`, and `left-0` to `left-10`, allowing you to set the desired spacing value.

```html
<div class="top-2 left-4 surface-tertiary text-white p-2 mb-2">
  This div has 2 units of top spacing and 4 units of left spacing.
</div>
<div class="right-6 bottom-8 surface-tertiary text-white p-2 mb-2">
  This div has 6 units of right spacing and 8 units of bottom spacing.
</div>
```

<div class="component-preview d-block">
<div class="top-2 left-4 surface-tertiary text-white p-2 mb-2">This div has 2 units of top spacing and 4 units of left spacing.</div>
<div class="right-6 bottom-8 surface-tertiary text-white p-2 mb-2">This div has 6 units of right spacing and 8 units of bottom spacing.</div>
</div>

## Z-Index Utilities

The z-index utilities in MinimaCSS allow you to easily set the z-index property of an element.

#### Usage

The available z-index classes range from `z-10` to `z-100`, allowing you to set the desired z-index value.

```html
<div class="z-30 surface-tertiary text-white p-2 mb-2">
  This div has a z-index of 30.
</div>
<div class="z-70 surface-tertiary text-white p-2 mb-2">
  This div has a z-index of 70.
</div>
```

<div class="component-preview d-block">
<div class="z-30 surface-tertiary text-white p-2 mb-2">This div has a z-index of 30.</div>
<div class="z-70 surface-tertiary text-white p-2 mb-2">This div has a z-index of 70.</div>
</div>

## Object Fit Utilities

The object fit utilities in MinimaCSS allow you to easily set the object-fit property of an image or video element.

#### Usage

The available object-fit classes include `object-fit-contain`, `object-fit-cover`, `object-fit-fill`, `object-fit-none`, and `object-fit-scale-down`, allowing you to set the desired object-fit value.

```html
<div class="object-fit-cover surface-tertiary text-white p-2 mb-2">
  This is an image with object-fit set to "cover".
</div>
<div class="object-fit-contain surface-tertiary text-white p-2 mb-2">
  This is a video with object-fit set to "contain".
</div>
```

<div class="component-preview d-block">

</div>

## Object Position Utilities

The object position utilities in MinimaCSS allow you to easily set the object-position property of an image or video element.

#### Usage

The available object-position classes include `object-position-top`, `object-position-bottom`, `object-position-left`, `object-position-right`, and `object-position-center`, allowing you to set the desired object-position value.

```html
<div class="object-position-top surface-tertiary text-white p-2 mb-2">
  This is an image with object-position set to "top".
</div>
<div class="object-position-center surface-tertiary text-white p-2 mb-2">
  This is a video with object-position set to "center".
</div>
```

<div class="component-preview d-block">
</div>

## Full Positioning Shortcut

The `.full-position` class in MinimaCSS provides a convenient shortcut to set an element to have a position of absolute and cover the full width and height of its containing element.

#### Usage

```html
<div class="full-position surface-tertiary text-white p-2 mb-2">
  This div has a full position.
</div>
```

<div class="component-preview d-block">
</div>

## Centering Utility - Absolute Center

The `.center-absolute` class in MinimaCSS can be used to easily center an element horizontally and vertically using absolute positioning and the transform property.

#### Usage

```html
<div class="center-absolute surface-tertiary text-white p-2 mb-2">
  This div is centered using absolute positioning and transform.
</div>
```

<div class="component-preview d-block">
<div class="center-absolute surface-tertiary text-white p-2 mb-2">This div is centered using absolute positioning and transform.</div>
</div>
