# Image Utilities

---

> [!NOTE]
> _The content on this page is currently in progress and not yet complete. I am working to fully develop and refine the information here to ensure it meets the high standards of comprehensiveness and clarity. Other pages in this documentation may be complete. I appreciate your patience and understanding as I continue to enhance this page._

---

This documentation provides details about the image utilities in MinimaCSS, which offers various styles and functionalities for working with images.

## Responsive Image
`.img-responsive` is used to make an image responsive. It sets the maximum width to 100% and the height to auto.

#### Usage
```html
<img src="image.jpg" alt="Responsive Image" class="img-responsive">
```

## Disable dragging of Image
`.img-non-draggable` is used to prevent users from dragging an image.

#### Usage
```html
<img src="image.jpg" alt="Non-Draggable Image" class="img-non-draggable">
```

## Aspect Ratio Boxes
Aspect ratio boxes are used to maintain the aspect ratio of an element, typically an image or a video. They use the padding-top trick to achieve this.

To create an aspect ratio box, use one of the predefined aspect ratio classes: `.aspect-16-9`, `.aspect-4-3`, or `.aspect-1-1`.

#### Usage
```html
<div class="aspect-16-9">
  <img src="image.jpg" alt="Aspect Ratio 16:9">
</div>


```

## Image Shapes
The image shape utilities provide styles for creating different shapes such as circles and thumbnails.

### Circle
`.img-circle` is used to create a circular image by applying a border-radius of 50%.

#### Usage
```html
<img src="image.jpg" alt="Circle Image" class="img-circle">
```

### Thumbnail
`.img-thumbnail` is used to create a thumbnail for an image. It provides padding, background color, border, and a rounded border-radius.

#### Usage
```html
<img src="image.jpg" alt="Thumbnail Image" class="img-thumbnail">
```

## Image Shadow
`.img-shadow` can be used to apply a box shadow to an image.

#### Usage
```html
<img src="image.jpg" alt="Image with Shadow" class="img-shadow">
```
