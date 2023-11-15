# Navigation

Navigation bars are important in any webpage to make it easily accessible and user-friendly. This documentation explains the implementation of two types of navigation bars in MinimaCSS: Horizontal Navbar and Vertical Navbar. The nav classes are designed to be used with the `<nav>` element. 

## Horizontal Navbar

The `nav nav-primary` classes creates a horizontal navigation bar. It's typically used for the main navigation of a website. This bar includes a logo section, a mobile menu toggle, and a list of navigation links. Some of these links can be dropdowns for organizing multiple items.

```html
<nav class="nav nav-primary rounded-lg">
    <div class="nav-container">
        <!-- Logo -->
        <div class="nav-logo">
            <img src="logo-url"
                alt="Logo" class="nav-logo-img">
            <span class="nav-logo-text">MinimaCSS</span>
        </div>
        <!-- Mobile Menu Toggle -->
        <div class="nav-toggle">
            <span class="nav-toggle-icon">☰</span>
        </div>
        <!-- Navigation Links -->
        <ul class="nav-links">
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link active">Home</a>
            </li>
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link">About</a>
            </li>
            <!-- Dropdown -->
            <li class="nav-links-item">
                <details class="dropdown">
                    <summary class="dropdown-toggle nav-links-item-link">
                        Dropdown Menu
                    </summary>
                    <div class="dropdown-menu">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </details>
            </li>
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link">Contact</a>
            </li>
        </ul>
    </div>
</nav>


```

<div class="component-preview d-block">
<nav class="nav nav-primary rounded-lg">
    <div class="nav-container">
        <!-- Logo -->
        <div class="nav-logo">
            <img src="https://camo.githubusercontent.com/c606dbcb46fd8e055677968286b429f454245afc8d5c5b73eb8efd3be429acc8/68747470733a2f2f692e6962622e636f2f7a687a673976332f4d2e706e67"
                alt="Logo" class="nav-logo-img">
            <span class="nav-logo-text">MinimaCSS</span>
        </div>
        <!-- Mobile Menu Toggle -->
        <div class="nav-toggle">
            <span class="nav-toggle-icon">☰</span>
        </div>
        <!-- Navigation Links -->
        <ul class="nav-links">
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link active">
                    <span class="material-symbols-rounded">home</span> Home</a>
            </li>
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link">About</a>
            </li>
            <!-- Dropdown -->
            <li class="nav-links-item">
                <details class="dropdown">
                    <summary class="dropdown-toggle nav-links-item-link">
                        <span class="material-symbols-rounded">
                            feed
                        </span> Dropdown Menu
                    </summary>
                    <div class="dropdown-menu">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </details>
            </li>
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link"><span class="material-symbols-rounded">
                        mail
                    </span>Contact</a>
            </li>
        </ul>
    </div>
</nav>

</div>

## Vertical Navbar

The `nav-vertical` class is used for vertical navigation, often seen in sidebars or as secondary navigation elements. Like the primary navigation, it includes a logo and navigation links, which can also include dropdown menus.
For applications where Horizontal Navbar doesn't fit, Vertical Navbar can be implemented as below:

```html
<nav class="nav-vertical nav-secondary mt-5 rounded-lg">
    <div class="nav-container">
        <!-- Logo -->
        <div class="nav-logo">
            <img src="logo-url"
                alt="Logo" class="nav-logo-img">
            <span class="nav-logo-text">MinimaCSS</span>
        </div>
        <!-- Navigation Links -->
        <ul class="nav-links">
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link active">Home</a>
            </li>
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link">About</a>
            </li>
            <!-- Dropdown -->
            <li class="nav-links-item">
                <details class="dropdown">
                    <summary class="dropdown-toggle nav-links-item-link">
                        Dropdown Menu
                    </summary>
                    <div class="dropdown-menu">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </details>
            </li>
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link">Contact</a>
            </li>
        </ul>
    </div>
</nav>
```

<div class="component-preview">
<nav class="nav-vertical nav-secondary mt-5 rounded-lg w-full" style="max-width:400px">
    <div class="nav-container">
        <!-- Logo -->
        <div class="nav-logo">
            <img src="https://camo.githubusercontent.com/c606dbcb46fd8e055677968286b429f454245afc8d5c5b73eb8efd3be429acc8/68747470733a2f2f692e6962622e636f2f7a687a673976332f4d2e706e67"
                alt="Logo" class="nav-logo-img">
            <span class="nav-logo-text">MinimaCSS</span>
        </div>
        <!-- Navigation Links -->
        <ul class="nav-links">
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link active">Home</a>
            </li>
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link">About</a>
            </li>
            <!-- Dropdown -->
            <li class="nav-links-item">
                <details class="dropdown">
                    <summary class="dropdown-toggle nav-links-item-link">
                        Dropdown Menu
                    </summary>
                    <div class="dropdown-menu">
                        <a class="dropdown-item" href="#">Action</a>
                        <a class="dropdown-item" href="#">Another action</a>
                        <a class="dropdown-item" href="#">Something else here</a>
                    </div>
                </details>
            </li>
            <li class="nav-links-item">
                <a href="#" class="nav-links-item-link">Contact</a>
            </li>
        </ul>
    </div>
</nav>

</div>

## Dropdown Menu

In both Horizontal and Vertical Navbars, dropdown menu has been implemented with `<details>` and `<summary>` tags. The dropdown classes are designed to use these tags for creating dropdown menus. Details and summary are HTML5 tags and are used to create a disclosure widget in which information is visible only when the widget is toggled into an "open" state.
A summary is provided in a `<summary>` element. The `<details>` and `<summary>` tags allow for the creation of user-friendly, interactive designs that are fully customizable in CSS. Note that the `dropdown` class can tie these elements together in a neat, stylish package.

```html
<details class="dropdown">
    <summary class="dropdown-toggle nav-links-item-link">
        Dropdown Menu
    </summary>
    <div class="dropdown-menu">
        <a class="dropdown-item" href="#">Action</a>
        <a class="dropdown-item" href="#">Another action</a>
        <a class="dropdown-item" href="#">Something else here</a>
    </div>
</details>
```