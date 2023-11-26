# Slideover

The Slideover component is a dynamic UI element for presenting additional content in a sliding panel overlaying the main content. This updated documentation covers various placements (left, right, top, bottom) and sizes (small, medium, large, extra large).

## Usage

The Slideover component can be placed on different sides of the screen. It's implemented using HTML and controlled through JavaScript functions. Below is the updated structure and classes.

#### Slideover Variations

```html
<!-- Right Aligned Slideover (Small) -->
<div class="slideover left size-sm" id="left">
  <div class="slideover-header">
    <h5 class="mb-0 font-semibold">Slideover Header</h5>
    <p class="mb-0">This is long Slideover sub title</p>
    <button
      class="close-icon"
      onclick="toggleSlideover('#left')"
      aria-label="Close"
    >
      ×
    </button>
  </div>
  <div class="slideover-body">
    Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed
    ex at est egestas vehicula. Integer sit amet lectus mi. Duis ut viverra
    mauris, at laoreet enim.
  </div>
  <div class="slideover-footer">
    <button class="btn btn-outline-primary" onclick="toggleSlideover('#left')">
      Cancel
    </button>
    <button class="btn btn-primary ml-3" onclick="toggleSlideover('#left')">
      Save
    </button>
  </div>
</div>

<!-- Left Aligned Slideover -->
<div class="slideover left size-sm" id="left">
  <!-- Slideover content -->
</div>

<!-- Top Aligned Slideover -->
<div class="slideover top size-sm" id="top">
  <!-- Slideover content -->
</div>

<!-- Bottom Aligned Slideover -->
<div class="slideover bottom size-sm" id="bottom">
  <!-- Slideover content -->
</div>
```

### CSS Classes

- `slideover`: Base class for the Slideover component.
- `left`, `right`, `top`, `bottom`: Classes defining the placement of the Slideover.
- `size-sm`, `size-md`, `size-lg`, `size-xl`: Classes defining the size of the Slideover.
- `slideover-header`, `slideover-body`, `slideover-footer`: Classes for structuring the Slideover content.

<div class="component-preview">
   <button class="btn btn-primary m-1" onclick="toggleSlideover('#left')">Open Left</button>
<button class="btn btn-primary m-1" onclick="toggleSlideover('#right')">Open Right sm</button>
<button class="btn btn-primary m-1" onclick="toggleSlideover('#rightmd')">Open Right md</button>
<button class="btn btn-primary m-1" onclick="toggleSlideover('#rightlg')">Open Right lg</button>
<button class="btn btn-primary m-1" onclick="toggleSlideover('#rightxl')">Open Right xl</button>
<button class="btn btn-primary m-1" onclick="toggleSlideover('#top')">Open Top</button>
<button class="btn btn-primary m-1" onclick="toggleSlideover('#bottom')">Open Bottom</button>
<!-- Right Aligned Slideover -->
<div class="slideover left size-sm" id="left">
    <div class="slideover-header">
        <h5 class="mb-0 font-semibold">Slideover Header</h5>
        <p class="mb-0">This is long Slideover sub title</p>
        <button class="close-icon" onclick="toggleSlideover('#left')" aria-label="Close">×</button>
    </div>
    <div class="slideover-body">
        Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est egestas vehicula.
        Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.
    </div>
    <div class="slideover-footer">
        <button class="btn btn-outline-primary" onclick="toggleSlideover('#left')">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="toggleSlideover('#left')">Save</button>
    </div>
</div>
<div class="slideover right size-sm" id="right">
    <div class="slideover-header">
        <h5 class="mb-0 font-semibold">Slideover Header</h5>
        <p class="mb-0">This is long Slideover sub title</p>
        <button class="close-icon" onclick="toggleSlideover('#right')" aria-label="Close">×</button>
    </div>
    <div class="slideover-body">
        Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est egestas vehicula.
        Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.
    </div>
    <div class="slideover-footer">
        <button class="btn btn-outline-primary" onclick="toggleSlideover('#right')">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="toggleSlideover('#right')">Save</button>
    </div>
</div>
<div class="slideover right size-md" id="rightmd">
    <div class="slideover-header">
        <h5 class="mb-0 font-semibold">Slideover Header</h5>
        <p class="mb-0">This is long Slideover sub title</p>
        <button class="close-icon" onclick="toggleSlideover('#rightmd')" aria-label="Close">×</button>
    </div>
    <div class="slideover-body">
        Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est egestas vehicula.
        Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.
    </div>
    <div class="slideover-footer">
        <button class="btn btn-outline-primary" onclick="toggleSlideover('#rightmd')">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="toggleSlideover('#rightmd')">Save</button>
    </div>
</div>
<div class="slideover right size-lg" id="rightlg">
    <div class="slideover-header">
        <h5 class="mb-0 font-semibold">Slideover Header</h5>
        <p class="mb-0">This is long Slideover sub title</p>
        <button class="close-icon" onclick="toggleSlideover('#rightlg')" aria-label="Close">×</button>
    </div>
    <div class="slideover-body">
        Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est egestas vehicula.
        Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.
    </div>
    <div class="slideover-footer">
        <button class="btn btn-outline-primary" onclick="toggleSlideover('#rightlg')">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="toggleSlideover('#rightlg')">Save</button>
    </div>
</div>
<div class="slideover right size-xl" id="rightxl">
    <div class="slideover-header">
        <h5 class="mb-0 font-semibold">Slideover Header</h5>
        <p class="mb-0">This is long Slideover sub title</p>
        <button class="close-icon" onclick="toggleSlideover('#rightxl')" aria-label="Close">×</button>
    </div>
    <div class="slideover-body">
        Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est egestas vehicula.
        Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.
    </div>
    <div class="slideover-footer">
        <button class="btn btn-outline-primary" onclick="toggleSlideover('#rightxl')">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="toggleSlideover('#rightxl')">Save</button>
    </div>
</div>
<div class="slideover top size-sm" id="top">
    <div class="slideover-header">
        <h5 class="mb-0 font-semibold">Slideover Header</h5>
        <p class="mb-0">This is long Slideover sub title</p>
        <button class="close-icon" onclick="toggleSlideover('#top')" aria-label="Close">×</button>
    </div>
    <div class="slideover-body">
        Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est egestas vehicula.
        Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.
    </div>
    <div class="slideover-footer">
        <button class="btn btn-outline-primary" onclick="toggleSlideover('#top')">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="toggleSlideover('#top')">Save</button>
    </div>
</div>
<div class="slideover bottom size-sm" id="bottom">
    <div class="slideover-header">
        <h5 class="mb-0 font-semibold">Slideover Header</h5>
        <p class="mb-0">This is long Slideover sub title</p>
        <button class="close-icon" onclick="toggleSlideover('#bottom')" aria-label="Close">×</button>
    </div>
    <div class="slideover-body">
        Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est egestas vehicula.
        Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.
    </div>
    <div class="slideover-footer">
        <button class="btn btn-outline-primary" onclick="toggleSlideover('#bottom')">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="toggleSlideover('#bottom')">Save</button>
    </div>
</div>
<div class="slideover-backdrop blur-backdrop " onclick="toggleSlideover()"></div>
</div>

### JavaScript Functionality

A JavaScript function `toggleSlideover` is used to control the opening and closing of the Slideover. The implementation details of this function are not provided in the snippet.
