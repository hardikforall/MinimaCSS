
# Typography

Typography in MinimaCSS is built to provide a harmonious and readable experience, leveraging the modern, web-friendly Inter font. Our typographic scale is based on two core elements: scale and rhythm.

#### Font Import

MinimaCSS uses the "Inter" font family, which is imported from a CDN for high-quality, versatile font rendering across different devices.

```css
@import url('https://cdn.jsdelivr.net/npm/inter-ui@3.19.3/inter.min.css');
```


## Global Settings
Text elements are styled with global settings in mind for a consistent look and feel.

```css
body {
  font-family: "Inter", sans-serif;
  line-height: 1.6;
  color: var(--text-primary-color);
  background-color: var(--surface-primary-color);
}
```

## Headings
All HTML headings, `h1` through `h6`, are styled with the Inter font, weights, and sizes. For a responsive design, sizes are adjusted using the `clamp` function to provide a fluid typographic scale.

```html
<!-- Example HTML for Headings -->
<h1>h1. Heading</h1>
<h2>h2. Heading</h2>
<h3>h3. Heading</h3>
<h4>h4. Heading</h4>
<h5>h5. Heading</h5>
<h6>h6. Heading</h6>
```

<div class="component-preview dir-col">
  <h1>h1. Heading</h1>
  <h2>h2. Heading</h2>
  <h3>h3. Heading</h3>
  <h4>h4. Heading</h4>
  <h5>h5. Heading</h5>
  <h6>h6. Heading</h6>
</div>

```css
// Example SCSS for Headings
h1 { font-size: var(--font-size-h1); }
h2 { font-size: var(--font-size-h2); }
h3 { font-size: var(--font-size-h3); }
// ... Continue for h4, h5, h6
```

## Body Copy
Body text is set with a base size and line-height to ensure readability on all devices.

```html
<p>This is an example of standard body text. It is styled to be easy on the eyes and understandable.</p>
```
<div class="component-preview dir-col">
<p>This is an example of standard body text. It is styled to be easy on the eyes and understandable. This is an example of standard body text. It is styled to be easy on the eyes and understandable. This is an example of standard body text. It is styled to be easy on the eyes and understandable. This is an example of standard body text. It is styled to be easy on the eyes and understandable.  </p>
</div>

## Inline Text Elements
Style inline elements such as bold (`<strong>`), italics (`<em>`), and others to stand out appropriately within body text.

```html
<p>You can use the mark tag to <mark>highlight</mark> text.</p>
<p><del>This line of text is meant to be treated as deleted text.</del></p>
<p><s>This line of text is meant to be treated as no longer accurate.</s></p>
<p><ins>This line of text is meant to be treated as an addition to the document.</ins></p>
<p><u>This line of text will render as underlined.</u></p>
<p><small>This line of text is meant to be treated as fine print.</small></p>
<p><strong>This line rendered as bold text.</strong></p>
<p><em>This line rendered as italicized text.</em></p>
```
<div class="component-preview dir-col">
<p>You can use the mark tag to <mark>highlight</mark> text.</p>
<p><del>This line of text is meant to be treated as deleted text.</del></p>
<p><s>This line of text is meant to be treated as no longer accurate.</s></p>
<p><ins>This line of text is meant to be treated as an addition to the document.</ins></p>
<p><u>This line of text will render as underlined.</u></p>
<p><small>This line of text is meant to be treated as fine print.</small></p>
<p><strong>This line rendered as bold text.</strong></p>
<p><em>This line rendered as italicized text.</em></p>
</div>

## Lists
Styled to provide a clear visual hierarchy for ordered and unordered lists, which is essential for reading comprehension.

```html
<ul>
  <li>Unordered list item</li>
  <li>Another list item</li>
</ul>
<ol>
  <li>Ordered list item</li>
  <li>Another list item</li>
</ol>
```

<div class="component-preview dir-col">
<ul>
  <li>Unordered list item</li>
  <li>Another list item</li>
</ul>
<ol>
  <li>Ordered list item</li>
  <li>Another list item</li>
</ol>
</div>

## Blockquotes
Blockquotes are given a distinct style to set them apart from the body text, indicating quoted content.

```html
<blockquote>
  <p>This is a blockquote, styled to stand out from the rest of your content.</p>
</blockquote>
```

<div class="component-preview dir-col">
<blockquote>
  This is a blockquote, styled to stand out from the rest of your content.
</blockquote>
</div>

#### Other Elements

- `hr` tags are styled to represent thematic breaks in content.
- `label` elements are styled for form usability.
- `img` tags are set to be responsive.
- `figure` and `figcaption` are formatted for image captions.
- `code` and `pre` tags are styled for inline and block code snippets.
- `small` tags are used for less emphasized text.

## SCSS Overview
The SCSS for typography is designed to be modular, using variables for font sizes, weights, and line heights to provide a consistent and easily customizable system. Utilizing modern CSS features like custom properties and `clamp`, MinimaCSS typography ensures scalability and responsiveness.

Remember to compile your SCSS to CSS to see these styles take effect in your project.
