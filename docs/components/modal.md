# Modal

The Modal component is a versatile UI element used for displaying content in a layer above the main application content. It's commonly used for alerts, user notifications, or custom content presentations. This modal is designed to be responsive, accessible, and easy to integrate within various web projects.

### Usage

The Modal component is structured with HTML and styled using CSS classes. Below is a detailed breakdown of its structure and classes.

### Base Classes

- `modal`: Base class for the modal.
- `modal-lg`: Modifier class for a large modal.
- `modal-header`: Container for the header section of the modal.
- `modal-body`: Container for the body content of the modal.
- `modal-footer`: Container for the footer section of the modal.

### Sizes

- `modal-sm`: Class for a small modal.
- `modal-lg`: Class for a large modal.
- `modal-xl`: Class for an extra large modal.

### HTML Structure

```html
<!-- Modal -->
<button
  onclick="document.getElementById('myModallg').showModal()"
  class="btn btn-primary"
>
  Open Large Modal
</button>

<dialog id="myModallg" class="modal modal-lg">
  <header class="modal-header">
    <h5 class="mb-0 font-semibold">Modal Header</h5>
    <p class="mb-0 text-secondary">This is long Modal sub title</p>
    <button
      class="close-icon"
      onclick="document.getElementById('myModal').close();"
      aria-label="Close"
    >
      &times;
    </button>
  </header>
  <div class="modal-body">
    <p class="my-10">
      Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce
      sed ex at est egestas vehicula. Integer sit amet lectus mi. Duis ut
      viverra mauris, at laoreet enim.
    </p>
  </div>
  <footer class="modal-footer">
    <button
      class="btn btn-outline-primary"
      onclick="document.getElementById('myModallg').close();"
    >
      Cancel
    </button>
    <button
      class="btn btn-primary ml-3"
      onclick="document.getElementById('myModallg').close();"
    >
      Save
    </button>
  </footer>
</dialog>
```

<div class="component-preview">
<!-- Modal -->
<button onclick="document.getElementById('myModalsm').showModal()" class="btn btn-primary">Open Small Modal</button>
<button onclick="document.getElementById('myModallg').showModal()" class="btn btn-primary">Open Large Modal</button>
<button onclick="document.getElementById('myModalxl').showModal()" class="btn btn-primary">Open Extra Large Modal</button>

<dialog id="myModalsm" class="modal modal-sm">
    <header class="modal-header">
        <h5 class="mb-0 font-semibold">Modal Header</h5>
        <p class="mb-0 text-secondary">This is long Modal sub title</p>
        <button class="close-icon" onclick="document.getElementById('myModalsm').close();"
            aria-label="Close">&times;</button>
    </header>
    <div class="modal-body">
        <p class="my-10">Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est
            egestas
            vehicula. Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.</p>
    </div>
    <footer class="modal-footer">
        <button class="btn btn-outline-primary"
            onclick="document.getElementById('myModalsm').close();">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="document.getElementById('myModalsm').close();">Save</button>
    </footer>
</dialog>

<dialog id="myModallg" class="modal modal-lg">
    <header class="modal-header">
        <h5 class="mb-0 font-semibold">Modal Header</h5>
        <p class="mb-0 text-secondary">This is long Modal sub title</p>
        <button class="close-icon" onclick="document.getElementById('myModallg').close();"
            aria-label="Close">&times;</button>
    </header>
    <div class="modal-body">
        <p class="my-10">Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est
            egestas
            vehicula. Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.</p>
    </div>
    <footer class="modal-footer">
        <button class="btn btn-outline-primary"
            onclick="document.getElementById('myModallg').close();">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="document.getElementById('myModallg').close();">Save</button>
    </footer>
</dialog>

<dialog id="myModalxl" class="modal modal-xl">
    <header class="modal-header">
        <h5 class="mb-0 font-semibold">Modal Header</h5>
        <p class="mb-0 text-secondary">This is long Modal sub title</p>
        <button class="close-icon" onclick="document.getElementById('myModalxl').close();"
            aria-label="Close">&times;</button>
    </header>
    <div class="modal-body">
        <p class="my-10">Aenean vestibulum nunc at libero congue, eu pretium nulla viverra. Fusce sed ex at est
            egestas
            vehicula. Integer sit amet lectus mi. Duis ut viverra mauris, at laoreet enim.</p>
    </div>
    <footer class="modal-footer">
        <button class="btn btn-outline-primary"
            onclick="document.getElementById('myModalxl').close();">Cancel</button>
        <button class="btn btn-primary ml-3" onclick="document.getElementById('myModalxl').close();">Save</button>
    </footer>
</dialog>
</div>
