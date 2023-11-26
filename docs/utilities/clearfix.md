## Clearfix

---

> [!NOTE] > _The content on this page is currently in progress and not yet complete. I am working to fully develop and refine the information here to ensure it meets the high standards of comprehensiveness and clarity. Other pages in this documentation may be complete. I appreciate your patience and understanding as I continue to enhance this page._

---

The clearfix utility class is used to fix the issue of parent containers not fully wrapping their child floats. It ensures that the parent container expands to the height of its floating child elements.

#### Usage

```scss
.clearfix {
}
```

Apply the `.clearfix` class to the parent container that contains floated elements.

```html
<div class="clearfix">
  <div class="float-left p-2 surface-primary">Left Floating Element</div>
  <div class="float-right p-2 surface-primary">Right Floating Element</div>
</div>
```

<div class="component-preview d-block">
    <div class="clearfix">
        <div class="float-left p-2 surface-primary">Left Floating Element</div>
        <div class="float-right p-2 surface-primary">Right Floating Element</div>
    </div>
</div>
