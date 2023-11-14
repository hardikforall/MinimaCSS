
# Typography Utilities 

This documentation provides a comprehensive guide to the typography utilities available in MinimaCSS. These utilities offer a range of options for manipulating text appearance, including font size, weight, alignment, and potentially more, depending on the provided utilities in the SCSS file.

### Font Size
Font size utilities allow for easy adjustment of text size across your web application.

#### Usage
To use a font size utility, simply add the relevant class to your HTML element. Classes follow the format `.text-[size]`


```html
<p class="text-xs">This is Extra Small text.</p>
<p class="text-sm">This is Small text.</p>
<p class="text-md">This is medium text.</p>
<p class="text-lg">This is large text.</p>
<p class="text-xl">This is Extra large text.</p>
<p class="text-2xl">This is 2xl text.</p>
<p class="text-3xl">This is 3xl text.</p>
<p class="text-4xl">This is 4xl text.</p>
<p class="text-5xl">This is 5xl text.</p>
```

<div class="component-preview d-block">
<p class="text-xs">This is Extra Small text.</p>
<p class="text-sm">This is Small text.</p>
<p class="text-md">This is medium text.</p>
<p class="text-lg">This is large text.</p>
<p class="text-xl">This is Extra large text.</p>
<p class="text-2xl">This is 2xl large text.</p>
<p class="text-3xl">This is 3xl large text.</p>
<p class="text-4xl">This is 4xl large text.</p>
<p class="text-5xl">This is 5xl large text.</p>
</div>

##### Text Size Respresentation
```css
$font-sizes: (
  'xs': 0.75rem,
  'sm': 0.875rem,
  'md': 1rem,
  'lg': 1.25rem,
  'xl': 1.5rem,
  '2xl': 1.75rem,
  '3xl': 2rem,
  '4xl': 2.5rem,
  '5xl': 3rem 
);
```
## Font Weight
Font weight utilities provide a method to adjust the weight (thickness) of the text.

#### Usage
Classes for font weight follow the format `.font-[weight]`, where `[weight]` is the name of the weight (e.g., `bold`, `light`).

#### Example
```html
<p class="font-light">Light weight text.</p>
<p class="font-normal">Normal weight text.</p>
<p class="font-medium">Medium weight text.</p>
<p class="font-semi-bold">Semi Bold weight text.</p>
<p class="font-bold">Bold weight text.</p>
<p class="font-extra-bold">Extra Bold weight text.</p>
<p class="font-black">Black weight text.</p>
```

<div class="component-preview d-block">
<p class="font-light">Light weight text.</p>
<p class="font-normal">Normal weight text.</p>
<p class="font-medium">Medium weight text.</p>
<p class="font-semi-bold">Semi Bold weight text.</p>
<p class="font-bold">Bold weight text.</p>
<p class="font-extra-bold">Extra Bold weight text.</p>
<p class="font-black">Black weight text.</p>
</div>

##### Font Weight Respresentation
```css
$font-weights: (
  'light': 300,
  'normal': 400,
  'medium': 500,
  'semi-bold': 600,
  'bold': 700,
  'extra-bold': 800,
  'black': 900 
);
```

## Text Alignment
Text alignment utilities offer easy text alignment within elements.

#### Usage
To align text, use the `.text-[alignment]` class, where `[alignment]` is `left`, `right`, `center`, or `justify`.

```html
<p class="text-left">Left aligned text.</p>
<p class="text-center">Center aligned text.</p>
<p class="text-right">Right aligned text.</p>
<p class="text-justify">Justified text.</p>
```

<div class="component-preview">
<p class="text-left w-full">Left aligned text.</p>
<p class="text-center w-full">Center aligned text.</p>
<p class="text-right w-full">Right aligned text.</p>
<p class="text-justify w-full"><strong>Justified text.</strong>  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut fringilla felis nec sem placerat, ac tincidunt odio lobortis. Nam at purus efficitur, tincidunt metus vitae, tristique mi. Etiam id hendrerit ligula. Integer ultricies dignissim molestie.   rhoncus luctus ipsum. Proin et faucibus ipsum. Phasellus ultricies tincidunt sem nec luctus.  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut fringilla felis nec sem placerat, ac tincidunt odio lobortis. Nam at purus efficitur, tincidunt metus vitae, tristique mi. Etiam id hendrerit ligula. Integer ultricies dignissim molestie.   rhoncus luctus ipsum. Proin et faucibus ipsum. Phasellus ultricies tincidunt sem nec luctus.  </p>
</div>



## Line Height 
Adjust line height using these utilities.

#### Usage
The class format is `.line-height-[height]`, referencing a line height variable.

```html
<p class="line-height-none">1 spaced text</p>
<p class="line-height-tight">tight spaced text</p>
<p class="line-height-snug">snug spaced text</p>
<p class="line-height-normal">normal spaced text</p>
<p class="line-height-relaxed">relaxed spaced text</p>
<p class="line-height-loose">Loosely spaced text</p>
```
<div class="component-preview d-block">
<p class="line-height-none"><strong>No Spaced text</strong> <br> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut fringilla felis nec sem placerat, ac tincidunt odio lobortis. Nam at purus efficitur, tincidunt metus vitae, tristique mi. Etiam id hendrerit ligula. Integer ultricies dignissim molestie.  </p><hr>
<p class="line-height-tight"><strong>Tight spaced text</strong> <br> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut fringilla felis nec sem placerat, ac tincidunt odio lobortis. Nam at purus efficitur, tincidunt metus vitae, tristique mi. Etiam id hendrerit ligula. Integer ultricies dignissim molestie.  </p><hr>
<p class="line-height-snug"><strong>Snug spaced text</strong> <br> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut fringilla felis nec sem placerat, ac tincidunt odio lobortis. Nam at purus efficitur, tincidunt metus vitae, tristique mi. Etiam id hendrerit ligula. Integer ultricies dignissim molestie.  </p><hr>
<p class="line-height-normal"><strong>Normal spaced text</strong> <br> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut fringilla felis nec sem placerat, ac tincidunt odio lobortis. Nam at purus efficitur, tincidunt metus vitae, tristique mi. Etiam id hendrerit ligula. Integer ultricies dignissim molestie.  </p><hr>
<p class="line-height-relaxed"><strong>Relaxed spaced text</strong> <br> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut fringilla felis nec sem placerat, ac tincidunt odio lobortis. Nam at purus efficitur, tincidunt metus vitae, tristique mi. Etiam id hendrerit ligula. Integer ultricies dignissim molestie.  </p><hr>
<p class="line-height-loose"><strong>Loosely spaced text</strong> <br> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut fringilla felis nec sem placerat, ac tincidunt odio lobortis. Nam at purus efficitur, tincidunt metus vitae, tristique mi. Etiam id hendrerit ligula. Integer ultricies dignissim molestie.  </p>
</div>

##### Line-height Respresentation
```css
$line-heights: (
  'none': 1,
  'tight': 1.25,
  'snug': 1.375,
  'normal': 1.5,
  'relaxed': 1.625,
  'loose': 2
);

```


## Letter Spacing
Modify letter spacing with these classes.

#### Usage
Classes follow the `.letter-spacing-[spacing]` format, where `[spacing]` is a variable.

```html
<p class="letter-spacing-tighter">Tighter letter spacing</p>
<p class="letter-spacing-tight">Slightly tight letter spacing</p>
<p class="letter-spacing-normal">Default letter spacing</p>
<p class="letter-spacing-wide">Slightly wide letter spacing</p>
<p class="letter-spacing-wider">Wider letter spacing</p>
<p class="letter-spacing-widest">Widest letter spacing</p>
```
<div class="component-preview d-block">
<p class="letter-spacing-tighter">Tighter letter spacing</p>
<p class="letter-spacing-tight">Slightly tight letter spacing</p>
<p class="letter-spacing-normal">Default letter spacing</p>
<p class="letter-spacing-wide">Slightly wide letter spacing</p>
<p class="letter-spacing-wider">Wider letter spacing</p>
<p class="letter-spacing-widest">Widest letter spacing</p>
</div>

##### Letter Spacing Respresentation
```css
$letter-spacings: (
  'tighter': -0.05em,
  'tight': -0.025em,
  'normal': 0, 
  'wide': 0.025em,      
  'wider': 0.05em,
  'widest': 0.1em 
);

```

## Text Transformation 
Transform text using these classes.

#### Usage
The format is `.text-[transform]`, with `[transform]` being a transformation type.

#### Example
```html
<p class="text-uppercase">Uppercase text</p>
<p class="text-lowercase">Lowercase text</p>
<p class="text-capitalize">Capitalized text</p>
```
<div class="component-preview">
<p class="text-uppercase">Uppercase text</p>
<p class="text-lowercase">Lowercase text</p>
<p class="text-capitalize">Capitalized text</p>
</div>

## Font Style 
Apply different font styles.

#### Usage
Use `.font-italic` or `.font-normal`.

#### Example
```html
<p class="font-italic">Italic text</p>
<p class="font-normal">Normal text</p>
```
<div class="component-preview">
<p class="font-italic">Italic text</p>
<p class="font-normal">Normal text</p>
</div>

## Text Decoration 
Decorate text with these classes.

#### Usage
Classes include `.text-decoration-none`, `.text-decoration-underline`, `text-decoration-line-through`, `text-decoration-overline` etc.

#### Usage
```html
<p class="text-decoration-none">No Decoration</p>
<p class="text-decoration-underline">Underlined text</p>
<p class="text-decoration-line-through">Line Trough text</p>
<p class="text-decoration-overline">Overline text</p>
```

<div class="component-preview">
<p class="text-decoration-none">No Decoration</p>
<p class="text-decoration-underline">Underlined text</p>
<p class="text-decoration-line-through">Line Trough text</p>
<p class="text-decoration-overline">Overline text</p>
</div>

## Word Wrap and Text Overflow
Control word wrapping and text overflow.

#### Usage
Classes like `.text-wrap`, `.text-nowrap`, and `.text-truncate`, `.text-ellipsis`, `.text-clip` are available.

#### Example
```html
<p class="text-wrap w-10">Truncated text : Integer ultricies dignissim molestie.</p>
<p class="text-nowrap w-10">Truncated text: Integer ultricies dignissim molestie.</p>
<p class="text-truncate w-10">Truncated text: Integer ultricies dignissim molestie.</p>
<p class="text-ellipsis w-10">Ellipsis text: Integer ultricies dignissim molestie.</p>
<p class="text-clip w-10">Clip text: Integer ultricies dignissim molestie.</p>
```

<div class="component-preview d-block">
<p class="text-wrap w-10">Truncated text : Integer ultricies dignissim molestie.</p>
<p class="text-nowrap w-10">Truncated text: Integer ultricies dignissim molestie.</p>
<p class="text-truncate w-10">Truncated text: Integer ultricies dignissim molestie.</p>
<p class="text-ellipsis w-10">Ellipsis text: Integer ultricies dignissim molestie.</p>
<p class="text-clip w-10">Clip text: Integer ultricies dignissim molestie.</p>
</div>