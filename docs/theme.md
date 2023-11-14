This documentation provides an overview of the implementation of dark and light themes using SCSS and HTML. These themes allow for a flexible and user-friendly interface, catering to different preferences and environments.

## Colors

##### Primary Colors

<div class="component-preview position-relative">
<div class="color-box" style="background-color: #c8d3f7; color: black;"><span>Primary-50<br>#c8d3f7</span></div>
<div class="color-box" style="background-color: #a6b8f2; color: black;"><span>Primary-100<br>#a6b8f2</span></div>
<div class="color-box" style="background-color: #859ded; color: black;"><span>Primary-200<br>#859ded</span></div>
<div class="color-box" style="background-color: #6482e9; color: white;"><span>Primary-300<br>#6482e9</span></div>
<div class="color-box" style="background-color: #4268e4; color: white;"><span>Primary-400<br>#4268e4</span></div>
<div class="color-box" style="background-color: #214ddf; color: white;"><span>Primary-500<br>#214ddf</span></div>
<div class="color-box" style="background-color: #1c41be; color: white;"><span>Primary-600<br>#1c41be</span></div>
<div class="color-box" style="background-color: #17369c; color: white;"><span>Primary-700<br>#17369c</span></div>
<div class="color-box" style="background-color: #122a7b; color: white;"><span>Primary-800<br>#122a7b</span></div>
<div class="color-box" style="background-color: #0d1f59; color: white;"><span>Primary-900<br>#0d1f59</span></div>
</div>

##### Dark (Tints) Shades

<div class="component-preview position-relative">
<div class="color-box" style="background-color: #f9f9fa; color: black;"><span>Gray-50<br>#f9f9fa</span></div>
<div class="color-box" style="background-color: #d9dbe0; color: black;"><span>Gray-100<br>#d9dbe0</span></div>
<div class="color-box" style="background-color: #b9bcc7; color: black;"><span>Gray-200<br>#b9bcc7</span></div>
<div class="color-box" style="background-color: #989ead; color: black;"><span>Gray-300<br>#989ead</span></div>
<div class="color-box" style="background-color: #787f94; color: white;"><span>Gray-400<br>#787f94</span></div>
<div class="color-box" style="background-color: #58617a; color: white;"><span>Gray-500<br>#58617a</span></div>
<div class="color-box" style="background-color: #384261; color: white;"><span>Gray-600<br>#384261</span></div>
<div class="color-box" style="background-color: #182447; color: white;"><span>Gray-700<br>#182447</span></div>
<div class="color-box" style="background-color: #151f3d; color: white;"><span>Gray-800<br>#151f3d</span></div>
<div class="color-box" style="background-color: #111a33; color: white;"><span>Gray-900<br>#111a33</span></div>
</div>

##### Other Context Colors
<div class="component-preview position-relative">
<div class="color-box " style="background-color: #214ddf; color: white;"><span>Primary<br>#214ddf</span></div>
<div class="color-box " style="background-color: #58617a; color: white;"><span>Secondary<br>#58617a</span></div>
<div class="color-box " style="background-color: #3F9142; color: white;"><span>Success<br>#3F9142</span></div>
<div class="color-box " style="background-color: #f44336; color: white;"><span>Danger<br>#f44336</span></div>
<div class="color-box " style="background-color: #F9703E; color: white;"><span>Warning<br>#F9703E</span></div>
<div class="color-box " style="background-color: #42a5f5; color: white;"><span>Info<br>#42a5f5</span></div>
<div class="color-box " style="background-color: #f9f9fa; color: black;"><span>Light<br>#f9f9fa</span></div>
<div class="color-box " style="background-color: #151f3d; color: white;"><span>Dark<br>#151f3d</span></div>
</div>


## Switching Themes - Dark & Light

Currently theme directly supports theme based on user preference. 

Switching between themes can be achieved by adding or removing the respective theme data attribute to body or root element of document

Light Theme : `data-theme="light"`
Dark Theme : `data-theme="dark"`

##### JavaScript Functionality

A JavaScript function can be used to toggle between the dark and light themes. This function would typically alter the class of the root element to switch the theme.

```javascript
    document.addEventListener("DOMContentLoaded", (event) => {
      const toggleSwitch = document.querySelector("#theme-toggle");
      function switchTheme(e) {
        if (e.target.checked) {
          document.documentElement.setAttribute("data-theme", "dark");
          localStorage.setItem("theme", "dark");
        } else {
          document.documentElement.setAttribute("data-theme", "light");
          localStorage.setItem("theme", "light");
        }
      }

      toggleSwitch.addEventListener("change", switchTheme, false);

      const currentTheme = localStorage.getItem("theme")
        ? localStorage.getItem("theme")
        : null;
      if (currentTheme) {
        document.documentElement.setAttribute("data-theme", currentTheme);
        if (currentTheme === "dark") {
          toggleSwitch.checked = true;
        }
      }
    });
```

For customising Themes and Colors I will be creating a detailed guide for it soon.

## Theme Structure

#### SCSS Color Variables (`_variables.scss`)

```css

//Primary Shades

$primary-50:#c8d3f7;
$primary-100:#a6b8f2;
$primary-200:#859ded;
$primary-300:#6482e9;
$primary-400:#4268e4;
$primary-500:#214ddf;
$primary-600:#1c41be;
$primary-700:#17369c;
$primary-800:#122a7b;
$primary-900:#0d1f59;

// above Colors are generated from below source
// https://noeldelgado.github.io/shadowlord/#214ddf  15%

//dark-shades
/* for grays https://noeldelgado.github.io/shadowlord/#182447 13.9% */
//above Colors are generated from below source
$gray-50: #f9f9fa;
$gray-100: #d9dbe0;
$gray-200: #b9bcc7;
$gray-300: #989ead;
$gray-400: #787f94;
$gray-500: #58617a;
$gray-600: #384261;
$gray-700: #182447;
$gray-800: #151f3d;
$gray-900: #111a33; 

//Other utility Colors Defined

$white: #ffffff;
$black: #111a33;

$red-50: #ffebee;
$red-100: #ffcdd2;
$red-200: #ef9a9a;
$red-300: #e57373;
$red-400: #ef5350;
$red-500: #f44336;
$red-600: #e53935;
$red-700: #d32f2f;
$red-800: #c62828;
$red-900: #b71c1c;

$green-50: #E3F9E5;
$green-100: #C1EAC5;
$green-200: #A3D9A5;
$green-300: #7BC47F;
$green-400: #57AE5B;
$green-500: #3F9142;
$green-600: #2F8132;
$green-700: #207227;
$green-800: #0E5814;
$green-900: #05400A;

$orange-50: #FFE8D9;
$orange-100: #FFD0B5;
$orange-200: #FFB088;
$orange-300: #FF9466;
$orange-400: #F9703E;
$orange-500: #F35627;
$orange-600: #DE3A11;
$orange-700: #C52707;
$orange-800: #AD1D07;
$orange-900: #841003;

$blue-50: #e3f2fd;
$blue-100: #bbdefb;
$blue-200: #90caf9;
$blue-300: #64b5f6;
$blue-400: #42a5f5;
$blue-500: #2196f3;
$blue-600: #1e88e5;
$blue-700: #1976d2;
$blue-800: #1565c0;
$blue-900: #0d47a1;

$colors: (
  "primary": $primary-500,
  "secondary": $gray-500,
  "success": $green-500,
  "danger": $red-500,
  "warning": $orange-400,
  "info": $blue-400,
  "light": $gray-50,
  "dark": $gray-800
);

```

#### Dark Theme SCSS (`_dark.scss`)

```css
@mixin dark {
    --accent-color:#{$primary-500};

    --light-color: #{$white};
    --dark-color: #{$black};

    --text-primary-color: #{$primary-50};
    --text-secondary-color: #{hex-to-rgba($primary-50, 0.75)};
    --text-tertiary-color:  #{hex-to-rgba($primary-50, 0.5)};

    --surface-primary-color:  #{$gray-900};
    --surface-secondary-color: #{$gray-700};
    --surface-tertiary-color: #{$gray-600};

    --scrollbarBG: var(--surface-secondary-color);
    --thumbBG: var(--surface-tertiary-color);;
    //border
    --border-primary-color: #{$gray-600};
    --border-secondary-color: #{$gray-700};
    --border-tertiary-color: #{$gray-800};

    // Typography
    --link-text-color: #{$primary-400};
    --link-hover-color: #{$primary-500};
    --blockquote-border-color: #{$primary-600};
    --blockquote-text-color: var(--text-primary-color);
    --blockquote-bg-color: var(--surface-secondary-color);
    --hr-border-color:var(--border-primary-color);
    --figcaption-text-color: var(--text-secondary-color);
    --code-bg-color: var(--surface-secondary-color);

    //Button
    --button-primary-color: #{$primary-500};
    --button-primary-hover-color: #{$primary-300};
    --button-primary-text-color: #{$white};
    --button-primary-focus-ring-color: #{hex-to-rgba($primary-500,0.4)};

    --button-highlight-border-color: #{hex-to-rgba($white, 0.2)};

    --button-error-color: #{$red-400};
    --button-error-hover-color: #{$red-300};
    --button-error-text-color: #{$white};
    --button-error-focus-ring-color: #{hex-to-rgba($red-400,0.4)};

    --button-success-color: #{$green-400};
    --button-success-hover-color: #{$green-300};
    --button-success-text-color: #{$white};
    --button-success-focus-ring-color: #{hex-to-rgba($green-400,0.4)};

    --button-info-color: #{$blue-400};
    --button-info-hover-color: #{$blue-300};
    --button-info-text-color: #{$white};
    --button-info-focus-ring-color: #{hex-to-rgba($blue-400,0.4)};

    --button-warning-color: #{$orange-400};
    --button-warning-hover-color: #{$orange-300};
    --button-warning-text-color: #{$white};
    --button-warning-focus-ring-color: #{hex-to-rgba($orange-400,0.4)};

    --button-light-color: #{$gray-100};
    --button-light-hover-color: #{$gray-200};
    --button-light-text-color: #{$gray-900};
    --button-light-focus-ring-color: #{hex-to-rgba($gray-300,0.4)};

    --button-dark-color: #{$gray-600};
    --button-dark-hover-color: #{$gray-500};
    --button-dark-text-color: #{$white};
    --button-dark-focus-ring-color: #{hex-to-rgba($gray-500,0.4)};
    
    --button-link-hover-color: #{$primary-500};
    --button-link-text-color: #{$primary-500};

    //Cards
    --card-bg-color:var(--surface-primary-color);
    --card-header-bg-color:var(--surface-secondary-color);
    --card-footer-bg-color:var(--surface-secondary-color);

     //inputs
     --input-bg-color:var(--surface-primary-color);
     --input-focus-ring-color: #{hex-to-rgba($primary-500,0.25)};
     --input-focus-border-color: #{$primary-500};
     --input-shadow-color:#{hex-to-rgba($black,1)};
     --input-valid-text-color:#{$green-500};
     --input-valid-border-color: #{$green-500};
     --input-focus-valid-ring-color: #{hex-to-rgba($green-400, 0.5)};
     --input-invalid-text-color:#{$red-500};
     --input-invalid-border-color: #{$red-500};
     --input-focus-invalid-ring-color: #{hex-to-rgba($red-500, 0.25)};
     --input-disabled-bg-color: var(--surface-secondary-color);

      //table
    --table-bg-color:var(--surface-primary-color);
    --table-accent-bg-color:var(--surface-secondary-color);
    --table-hover-bg-color:#{$gray-600};
    --table-border-color:var(--border-primary-color);

     //Nav
     --nav-primary-bg-color: #{$primary-500};
     --nav-primary-text-color: #{$white};
     --nav-primary-link-hover-color: #{hex-to-rgba($white, 0.2)};
     --nav-primary-dropdown-link-color: var(--text-primary-color);
     --nav-primary-dropdown-bg-color: var(--surface-secondary-color);

    //Circle Loader
    --loader-light-bg-color:#{hex-to-rgba($white, 0.7)};
    --loader-light-border-color:#{hex-to-rgba($white, 0.4)};

    --loader-dark-bg-color:#{hex-to-rgba($primary-300, 0.7)};;
    --loader-dark-border-color:#{hex-to-rgba($primary-300, 0.4)};

    
}
```

#### Light Theme SCSS (`_light.scss`)

```css
// _light.scss
[data-theme="light"],
:root:not([data-theme="dark"]) {
    --accent-color: #{$primary-500};

    --light-color: #{$white};
    --dark-color: #{$black};

    --text-primary-color: #{$gray-600};
    --text-secondary-color: #{$gray-400};
    --text-tertiary-color: #{$gray-300};

    --surface-primary-color: #{$white};
    --surface-secondary-color: #{$gray-50};
    --surface-tertiary-color: #{$gray-100};

    --scrollbarBG: var(--surface-secondary-color);
    --thumbBG: var(--surface-tertiary-color);;
    //border
    --border-primary-color: #{$gray-100};
    --border-secondary-color: #{$gray-200};
    --border-tertiary-color: #{$gray-300};

    // Typography
    --link-text-color: #{$primary-600};
    --link-hover-color: #{$primary-700};
    --blockquote-border-color: #{$primary-600};
    --blockquote-text-color: var(--text-primary-color);
    --blockquote-bg-color: var(--surface-secondary-color);
    --hr-border-color: var(--border-primary-color);
    --figcaption-text-color: var(--text-secondary-color);
    --code-bg-color: var(--surface-secondary-color);

    //Button
    --button-primary-color: #{$primary-500};
    --button-primary-hover-color: #{$primary-400};
    --button-primary-text-color: #{$white};
    --button-primary-focus-ring-color: #{hex-to-rgba($primary-500, 0.25)};

    --button-highlight-border-color: "transparent";

    --button-error-color: #{$red-500};
    --button-error-hover-color: #{$red-400};
    --button-error-text-color: #{$white};
    --button-error-focus-ring-color: #{hex-to-rgba($red-500, 0.25)};

    --button-success-color: #{$green-500};
    --button-success-hover-color: #{$green-400};
    --button-success-text-color: #{$white};
    --button-success-focus-ring-color: #{hex-to-rgba($green-500, 0.25)};

    --button-info-color: #{$blue-500};
    --button-info-hover-color: #{$blue-400};
    --button-info-text-color: #{$white};
    --button-info-focus-ring-color: #{hex-to-rgba($blue-500, 0.25)};

    --button-warning-color: #{$orange-400};
    --button-warning-hover-color: #{$orange-300};
    --button-warning-text-color: #{$white};
    --button-warning-focus-ring-color: #{hex-to-rgba($orange-500, 0.25)};

    --button-light-color: #{$gray-100};
    --button-light-hover-color: #{$gray-200};
    --button-light-text-color: #{$gray-900};
    --button-light-focus-ring-color: #{hex-to-rgba($gray-300, 0.25)};

    --button-dark-color: #{$gray-600};
    --button-dark-hover-color: #{$gray-500};
    --button-dark-text-color: #{$white};
    --button-dark-focus-ring-color: #{hex-to-rgba($gray-300, 0.25)};

    --button-link-hover-color: #{$primary-400};
    --button-link-text-color: #{$primary-500};

    //Cards
    --card-bg-color: var(--surface-primary-color);
    --card-header-bg-color: var(--surface-secondary-color);
    --card-footer-bg-color: var(--surface-secondary-color);

    //inputs
    --input-bg-color: var(--surface-primary-color);
    --input-focus-ring-color: #{hex-to-rgba($primary-500, 0.25)};
    --input-focus-border-color: #{$primary-500};
    --input-shadow-color:#{hex-to-rgba($black,0.05)};
    --input-valid-text-color:#{$green-500};
    --input-valid-border-color: #{$green-500};
    --input-focus-valid-ring-color: #{hex-to-rgba($green-400, 0.5)};
    --input-invalid-text-color:#{$red-500};
    --input-invalid-border-color: #{$red-500};
    --input-focus-invalid-ring-color: #{hex-to-rgba($red-500, 0.25)};
    --input-disabled-bg-color:var(--surface-secondary-color);

    //table
    --table-bg-color: var(--surface-primary-color);
    --table-accent-bg-color: #{$gray-50};
    --table-hover-bg-color: var(--surface-tertiary-color);
    --table-border-color: var(--border-primary-color);

    //Nav
    --nav-primary-bg-color: #{$primary-500};
    --nav-primary-text-color: #{$white};
    --nav-primary-link-hover-color: #{hex-to-rgba($white, 0.2)};
    --nav-primary-dropdown-link-color: var(--text-primary-color);
    --nav-primary-dropdown-bg-color: var(--surface-secondary-color);
    
    //Circle Loader
    --loader-light-bg-color:#{hex-to-rgba($white, 0.7)};
    --loader-light-border-color:#{hex-to-rgba($white, 0.4)};

    --loader-dark-bg-color:#{hex-to-rgba($primary-500, 0.5)};;
    --loader-dark-border-color:#{hex-to-rgba($primary-500, 0.2)};

    //Steps 
    --steps-accent-color:
}
```


#### Usage and Implementation

The dark and light themes are defined using SCSS variables, which are then applied in the respective theme SCSS files. These styles can be toggled in the HTML through classes or other mechanisms.
