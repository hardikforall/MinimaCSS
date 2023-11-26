# Alert

Alert components in MinimaCSS are versatile and visually distinct elements used to convey various types of messages to users, such as notifications, warnings, and errors. These components are designed to be flexible and adaptable for different contexts.

## Variants

### Filled Alerts

Filled alerts have a solid background color. They are used to draw strong attention to the message.

#### Usage

```html
<div class="alert alert-primary">...</div>
<div class="alert alert-success">...</div>
<div class="alert alert-warning">...</div>
<div class="alert alert-danger">...</div>
<div class="alert alert-info">...</div>
<div class="alert alert-light">...</div>
<div class="alert alert-dark">...</div>
```

### Outline Alerts

Outline alerts have a border and a lighter background color. They are subtler compared to filled alerts.

#### Usage

```html
<div class="alert alert-outline-primary">...</div>
<div class="alert alert-outline-success">...</div>
<div class="alert alert-outline-warning">...</div>
<div class="alert alert-outline-danger">...</div>
<div class="alert alert-outline-info">...</div>
<div class="alert alert-outline-light">...</div>
<div class="alert alert-outline-dark">...</div>
```

## Components

### Icon

An optional icon to represent the type of alert. add class `.alert-icon` to any icon to make it visible

```html
<span class="alert-icon material-symbols-rounded">info</span>
```

### Title

A concise title for the alert message. `.alert-body-title`

```html
<div class="alert-body-title">Alert Title</div>
```

### Description

The main content or message of the alert. `.alert-body-description`

```html
<div class="alert-body-description">Detailed description of the alert.</div>
```

### Close Button

An optional close button for dismissing the alert. `.alert-close`

```html
<button class="alert-close">&times;</button>
```

## Detailed Usage Examples

(Here, include detailed examples for each type of alert, demonstrating the structure and how to use the icon, title, description, and close button.)

```html
<div class="alert alert-warning">
  <span class="alert-icon material-symbols-rounded"> error </span
  ><!-- Replace with your icon -->
  <div class="alert-body">
    <div class="alert-body-title">Attention needed</div>
    <div class="alert-body-description">
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquid pariatur,
      ipsum similique veniam quo totam eius aperiam dolorum.
    </div>
  </div>
  <button class="alert-close">&times;</button>
</div>
<div class="alert alert-outline-danger">
  <span class="alert-icon material-symbols-rounded"> error </span
  ><!-- Replace with your icon -->
  <div class="alert-body">
    <div class="alert-body-title">
      There were 2 errors with your form submission
    </div>
    <div class="alert-body-description">
      <ul role="list">
        <li>Your password must be at least 12 characters</li>
        <li>Your password must include All Letters in capital</li>
      </ul>
    </div>
  </div>
  <button class="alert-close">&times;</button>
</div>
<div class="alert alert-outline-success">
  <span class="alert-icon material-symbols-rounded"> error </span
  ><!-- Replace with your icon -->
  <div class="alert-body">
    <div class="alert-body-title">Order Placed</div>
    <div class="alert-body-description">
      <p>
        ipsum dolor sit amet consectetur adipisicing elit. Aliquid pariatur,
        ipsum similique veniam.
      </p>
      <a href="">Download Invoice</a> <a href="" class="ml-3">Dismiss</a>
    </div>
  </div>
</div>
<div class="alert alert-info">
  <span class="alert-icon material-symbols-rounded"> error </span
  ><!-- Replace with your icon -->
  <div class="alert-body">
    <div class="alert-body-title">New Update Received</div>
    <div class="alert-body-description">
      <p>A new software update is available. See what’s new!</p>
      <a href="">Get Details →</a>
    </div>
  </div>
  <button class="alert-close">&times;</button>
</div>
<div class="alert alert-outline-info">
  <span class="alert-icon material-symbols-rounded"> error </span
  ><!-- Replace with your icon -->
  <div class="alert-body">
    <div class="alert-body-title">New Update Received</div>
    <div class="alert-body-description">
      <p>A new software update is available. See what’s new!</p>
      <a href="">Get Details →</a>
    </div>
  </div>
  <button class="alert-close">&times;</button>
</div>
```

<div class="component-preview d-block">
<div class="alert alert-warning">
    <span class="alert-icon material-symbols-rounded">
        error
    </span><!-- Replace with your icon -->
    <div class="alert-body">
        <div class="alert-body-title">Attention needed</div>
        <div class="alert-body-description">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquid pariatur, ipsum similique veniam
            quo totam eius aperiam dolorum.
        </div>
    </div>
    <button class="alert-close">&times;</button>
</div>
<div class="alert alert-outline-danger">
    <span class="alert-icon material-symbols-rounded">
        error
    </span><!-- Replace with your icon -->
    <div class="alert-body">
        <div class="alert-body-title">There were 2 errors with your form submission</div>
        <div class="alert-body-description">
            <ul role="list">
                <li>Your password must be at least 12 characters</li>
                <li>Your password must include All Letters in capital</li>
            </ul>
        </div>
    </div>
    <button class="alert-close">&times;</button>
</div>
<div class="alert alert-outline-success">
    <span class="alert-icon material-symbols-rounded">
        error
    </span><!-- Replace with your icon -->
    <div class="alert-body">
        <div class="alert-body-title">Order Placed</div>
        <div class="alert-body-description">
            <p>ipsum dolor sit amet consectetur adipisicing elit. Aliquid pariatur, ipsum similique veniam.</p>
            <a href="">Download Invoice</a> <a href="" class="ml-3">Dismiss</a>
        </div>
    </div>
</div>
<div class="alert alert-info">
    <span class="alert-icon material-symbols-rounded">
        error
    </span><!-- Replace with your icon -->
    <div class="alert-body">
        <div class="alert-body-title">New Update Received</div>
        <div class="alert-body-description">
            <p>A new software update is available. See what’s new!</p>
            <a href="">Get Details →</a>
        </div>
    </div>
    <button class="alert-close">&times;</button>
</div>
<div class="alert alert-outline-info">
    <span class="alert-icon material-symbols-rounded">
        error
    </span><!-- Replace with your icon -->
    <div class="alert-body">
        <div class="alert-body-title">New Update Received</div>
        <div class="alert-body-description">
            <p>A new software update is available. See what’s new!</p>
            <a href="">Get Details →</a>
        </div>
    </div>
    <button class="alert-close">&times;</button>
</div>
</div>
