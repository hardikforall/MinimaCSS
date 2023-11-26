# Avatars

Avatars are used to represent individuals or entities in a graphical user interface. They can be images, icons, or text-based representations. MinimaCSS provides a range of avatar styles that can be easily customized to fit your design needs.

## Image Avatar

An image avatar is a representation of an individual or entity that uses an image. The `avatar` class is used to create an avatar, and the `avatar-md` class sets the size of the avatar to medium.

```html
<div class="avatar avatar-md">
  <img src="https://i.pravatar.cc/300" alt="Cat" />
</div>
```

<div class="component-preview">
<div class="avatar avatar-md">
    <img src="https://i.pravatar.cc/300" alt="Cat">
</div>
</div>

## Icon Avatar

An icon avatar is a representation of an individual or entity that uses an icon. The `avatar` class is used to create an avatar, the `avatar-md` class sets the size of the avatar to medium, and the `avatar-primary-outline` class adds a primary outline style to the avatar.

```html
<div class="avatar avatar-md avatar-primary-outline">
  <span class="material-symbols-rounded">group</span>
</div>
```

<div class="component-preview">
<div class="avatar avatar-md avatar-primary-outline">
    <span class="material-symbols-rounded">group</span>
</div>
</div>

## Text Avatar (Filled)

A text avatar is a representation of an individual or entity that uses text. The `avatar` class is used to create an avatar, the `avatar-md` class sets the size of the avatar to medium, and the `avatar-primary` class sets a primary filled style to the avatar.

```html
<div class="avatar avatar-md avatar-primary"><span>AB</span></div>
<div class="avatar avatar-md avatar-secondary"><span>AB</span></div>
<div class="avatar avatar-md avatar-success"><span>AB</span></div>
<div class="avatar avatar-md avatar-danger"><span>AB</span></div>
<div class="avatar avatar-md avatar-warning"><span>AB</span></div>
<div class="avatar avatar-md avatar-info"><span>AB</span></div>
<div class="avatar avatar-md avatar-dark"><span>AB</span></div>
<div class="avatar avatar-md avatar-light"><span>AB</span></div>
```

<div class="component-preview">
<div class="avatar avatar-md avatar-primary"><span>AB</span></div>
<div class="avatar avatar-md avatar-secondary"><span>AB</span></div>
<div class="avatar avatar-md avatar-success"><span>AB</span></div>
<div class="avatar avatar-md avatar-danger"><span>AB</span></div>
<div class="avatar avatar-md avatar-warning"><span>AB</span></div>
<div class="avatar avatar-md avatar-info"><span>AB</span></div>
<div class="avatar avatar-md avatar-dark"><span>AB</span></div>
<div class="avatar avatar-md avatar-light"><span>AB</span></div>
</div>

There are also other color variants available: `avatar-secondary`, `avatar-success`, `avatar-danger`, `avatar-warning`, `avatar-info`, `avatar-light`, and `avatar-dark`. All of these variants follow the same structure as the primary variant.

## Text Avatar (Outline)

A text avatar with an outline style is a representation of an individual or entity that uses text with an outline. The `avatar` class is used to create an avatar, the `avatar-md` class sets the size of the avatar to medium, and the `avatar-primary-outline` class adds a primary outline style to the avatar.

```html
<div class="avatar avatar-md avatar-primary-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-secondary-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-success-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-danger-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-warning-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-info-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-dark-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-light-outline"><span>AB</span></div>
```

<div class="component-preview">
<div class="avatar avatar-md avatar-primary-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-secondary-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-success-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-danger-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-warning-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-info-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-dark-outline"><span>AB</span></div>
<div class="avatar avatar-md avatar-light-outline"><span>AB</span></div>
</div>

There are also other color variants available with an outline style: `avatar-secondary-outline`, `avatar-success-outline`, `avatar-danger-outline`, `avatar-warning-outline`, `avatar-info-outline`, `avatar-light-outline`, and `avatar-dark-outline`. All of these variants follow the same structure as the primary variant.

## Avatar Sizes

Avatars can be displayed in different sizes. The sizes available are: small (`avatar-sm`), medium (`avatar-md`), large (`avatar-lg`), and extra large (`avatar-xl`).

```html
<div class="avatar avatar-sm avatar-primary-outline"><span>SM</span></div>
<div class="avatar avatar-md avatar-primary-outline"><span>MD</span></div>
<div class="avatar avatar-lg avatar-primary-outline"><span>LG</span></div>
<div class="avatar avatar-xl avatar-primary-outline"><span>XL</span></div>
```

<div class="component-preview">
<div class="avatar avatar-sm avatar-primary-outline"><span>SM</span></div>
<div class="avatar avatar-md avatar-primary-outline"><span>MD</span></div>
<div class="avatar avatar-lg avatar-primary-outline"><span>LG</span></div>
<div class="avatar avatar-xl avatar-primary-outline"><span>XL</span></div>
</div>

## Avatar Stack

An avatar stack is a group of avatars stacked together. The `avatar-stack` class is used to create an avatar stack, and each avatar is represented by an `avatar` div. In this example, we have four avatars stacked together.

```html
<div class="avatar-stack">
  <div class="avatar avatar-md avatar-primary"><span>AB</span></div>
  <div class="avatar avatar-md">
    <img src="https://i.pravatar.cc/300" alt="Cat" />
  </div>
  <div class="avatar avatar-md avatar-info"><span>AB</span></div>
  <div class="avatar avatar-md avatar-secondary"><span>+4</span></div>
</div>
```

<div class="component-preview">
<div class="avatar-stack">
    <div class="avatar avatar-md avatar-primary"><span>AB</span></div>
    <div class="avatar avatar-md">
        <img src="https://i.pravatar.cc/300" alt="Cat">
    </div>
    <div class="avatar avatar-md avatar-info"><span>AB</span></div>
    <div class="avatar avatar-md avatar-secondary"><span>+4</span></div>
</div>
</div>
