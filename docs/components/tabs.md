# Tabs

The Tabs component is an interactive interface element used to organize content into separate panes that are viewable one at a time. This component is highly effective in improving user experience by reducing clutter and focusing the user's attention on a specific category of content at a time.

## Usage

The Tabs component consists of a navigation bar with tab items and corresponding content sections. JavaScript is used for the interactive switching between tabs. Here is a detailed breakdown of its structure, classes, and implementation.

### CSS Classes

- `tabs-container`: Container for the tabs component.
- `tabs`: Class for the tabs navigation area.
- `tab`: Class for individual tab items.
- `active`: Class indicating the active tab.
- `tab-content`: Class for the content area of each tab.

### HTML Structure

```html
<!-- Tabs -->
<div class="tabs-container">
    <nav class="tabs" aria-label="Tabs">
        <a href="#" class="tab active" onclick="changeTab(event, 'tab1')" aria-current="page">Profile</a>
        <a href="#" class="tab" onclick="changeTab(event, 'tab2')">Account</a>
        <a href="#" class="tab " onclick="changeTab(event, 'tab3')">History Log</a>
    </nav>
</div>
<!-- Tab content -->
<div id="tab1" class="tab-content p-4">
    Content for Profile
</div>
<div id="tab2" class="tab-content p-4" style="display: none;">
    Content for Account
</div>
<div id="tab3" class="tab-content p-4" style="display: none;">
    Content for History
</div>
```

<div class="component-preview d-block">
<!-- Tabs -->
<div class="tabs-container">
    <nav class="tabs" aria-label="Tabs">
        <a href="#" class="tab active" onclick="changeTab(event, 'tab1')" aria-current="page">Profile</a>
        <a href="#" class="tab" onclick="changeTab(event, 'tab2')">Account</a>
        <a href="#" class="tab " onclick="changeTab(event, 'tab3')">History Log</a>
    </nav>
</div>
<!-- Tab content -->
<div id="tab1" class="tab-content p-4">
    Content for Profile
</div>
<div id="tab2" class="tab-content p-4" style="display: none;">
    Content for Account
</div>
<div id="tab3" class="tab-content p-4" style="display: none;">
    Content for History
</div>
</div>

### JavaScript Functionality

A JavaScript function `changeTab` is mentioned in the code. which is not icluded in the framework. This function controls the display of the tab content based on the tab clicked. The implementation details of this function are not provided in the snippet.



