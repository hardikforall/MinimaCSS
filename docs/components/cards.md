# Cards

Cards are a versatile and easily customizable component in MinimaCSS that can be used to display different types of content. They provide a clean and organized way to present information on your website.

### Usage

The card component in MinimaCSS is built using the `.card` class. This class can be combined with other classes like `.shadow-sm` for shadow effects, `.card-header` and `.card-footer` for header and footer sections, and `.card-img-top` for top-placed images. Cards are typically placed within a grid layout, such as within columns of a `.row`.

### Card with Image

The card variant with an image allows you to display an image at the top of the card. Below the image, you can add a title and some text content.

```html
<div class="card shadow-sm">
  <img
    src="https://placehold.co/600x400"
    class="card-img-top"
    alt="Card Image"
  />
  <div class="card-body">
    <h3 class="card-title">Card Title</h3>
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk of
      the card's content.
    </p>
  </div>
</div>
```

<div class="component-preview">
<div class="mt-3">
    <div class="card shadow-sm">
        <img src="https://placehold.co/100x50" class="card-img-top" alt="Card Image">
        <div class="card-body">
            <h3 class="card-title">Card Title</h3>
            <p class="card-text">Some quick example text to build on the card title and make up the bulk of
                the card's content.</p>
        </div>
    </div>
</div>
</div>

### Card with Footer

The card variant with a footer allows you to include links or additional information at the bottom of the card.

```html
<div class="card shadow-sm">
  <div class="card-body">
    <h3 class="card-title">Card Title</h3>
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk of
      the card's content.
    </p>
  </div>
  <div class="card-footer">
    <a href="#" class="card-link">Card Link</a>
    <a href="#" class="card-link">Another Link</a>
  </div>
</div>
```

<div class="component-preview">
<div class="mt-3">
    <div class="card shadow-sm">
        <div class="card-body">
            <h3 class="card-title">Card Title</h3>
            <p class="card-text">Some quick example text to build on the card title and make up the bulk of
                the card's content.</p>
        </div>
        <div class="card-footer">
            <a href="#" class="card-link">Card Link</a>
            <a href="#" class="card-link">Another Link</a>
        </div>
    </div>
</div>
</div>

### Card with Header

The card variant with a header allows you to add a title at the top of the card. You can also include additional content below the header.

```html
<div class="card shadow-sm">
  <div class="card-header">This is Card Title</div>
  <div class="card-body">
    <h3 class="card-title">Card Title</h3>
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk of
      the card's content.
    </p>
  </div>
</div>
```

<div class="component-preview">
<div class="mt-3">
    <div class="card shadow-sm">
        <div class="card-header">
            This is Card Title
        </div>
        <div class="card-body">
            <h3 class="card-title">Card Title</h3>
            <p class="card-text">Some quick example text to build on the card title and make up the bulk of
                the card's content.</p>
        </div>
    </div>
</div>
</div>

### Card without Header or Footer

The card variant without a header or footer allows you to display content without any additional elements.

```html
<div class="card shadow-sm">
  <div class="card-body">
    <h3 class="card-title">Card Title</h3>
    <p class="card-text">
      Some quick example text to build on the card title and make up the bulk of
      the card's content.
    </p>
  </div>
</div>
```

<div class="component-preview">
<div class="mt-3">
    <div class="card shadow-sm">
        <div class="card-body">
            <h3 class="card-title">Card Title</h3>
            <p class="card-text">Some quick example text to build on the card title and make up the bulk of
                the card's content.</p>
        </div>
    </div>
</div>
</div>
