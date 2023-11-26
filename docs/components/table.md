# Table

The Table component is an essential element for displaying data in a structured and readable format. It's ideal for representing information in rows and columns, making it easier for users to scan, compare, and understand data. This particular table component is designed with responsiveness and interactivity in mind, featuring striped rows, hover effects, and bordered styling.

## Usage

The Table component is created using HTML and is enhanced with CSS classes for styling. Below is an in-depth look at its structure and the classes used.

### HTML Structure

```html
<div class="table-responsive rounded-2">
  <table class="table table-striped table-hover table-bordered">
    <thead>
      <tr>
        <th scope="col">#</th>
        <th scope="col">First Name</th>
        <th scope="col">Last Name</th>
        <th scope="col">Username</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">1</th>
        <td>Mark</td>
        <td>Otto</td>
        <td>@mdo</td>
      </tr>
      <tr>
        <th scope="row">2</th>
        <td>Jacob</td>
        <td>Thornton</td>
        <td>@fat</td>
      </tr>
      <tr>
        <th scope="row">3</th>
        <td>Larry</td>
        <td>the Bird</td>
        <td>@twitter</td>
      </tr>
    </tbody>
  </table>
</div>
```

### CSS Classes

- `table-responsive`: Ensures table responsiveness, especially on smaller screens.
- `rounded-2`: Applies a specific border-radius to the table container.
- `table`: Base class for styling the table.
- `table-striped`: Adds zebra-striping to any table row.
- `table-hover`: Enables a hover state on table rows.
- `table-bordered`: Adds borders on all sides of the table and cells.

<div class="component-preview d-block">
<div class="table-responsive rounded-2">
    <table class="table table-striped table-hover table-bordered">
        <thead>
            <tr>
                <th scope="col">#</th>
                <th scope="col">First Name</th>
                <th scope="col">Last Name</th>
                <th scope="col">Username</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th scope="row">1</th>
                <td>Mark</td>
                <td>Otto</td>
                <td>@mdo</td>
            </tr>
            <tr>
                <th scope="row">2</th>
                <td>Jacob</td>
                <td>Thornton</td>
                <td>@fat</td>
            </tr>
            <tr>
                <th scope="row">3</th>
                <td>Larry</td>
                <td>the Bird</td>
                <td>@twitter</td>
            </tr>
        </tbody>
    </table>
</div>
</div>
