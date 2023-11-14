# Forms

Inputs are essential elements in any form to allow users to enter data. MinimaCSS provides a range of input styles that are easily customizable and adaptable to your design needs.

## Base Input

The base input is a simple input field without any additional styling.

```html
<div class="input-group">
    <label for="inputExample">Input Label</label>
    <input type="text" class="input" id="inputExample" placeholder="Input text here">
    <div class="helper-text">
        This is Helper text
    </div>
</div>
```

<div class="component-preview d-block">
<div class="input-group ">
    <label for="inputExample">Input Label</label>
    <input type="text" class="input" id="inputExample" placeholder="Input text here">
    <div class="helper-text">
        This is Helper text
    </div>
</div>
</div>

## Small Input

You can also use a smaller version of the input field by adding the `.input-small` class

```html
<div class="input-group ">
    <label for="SmallInput">Input Small Label</label>
    <input type="text" class="input input-small" id="SmallInput" placeholder="Input text here">
    <div class="helper-text">
        This is Helper text
    </div>
</div>
```

<div class="component-preview d-block">
<div class="input-group">
    <label for="SmallInput">Input Small Label</label>
    <input type="text" class="input input-small" id="SmallInput" placeholder="Input text here">
    <div class="helper-text">
        This is Helper text
    </div>
</div>
</div>

## Input Addons - Icon and Button

You can add icons or buttons to the input field by using the `.input-addon` class. Here are examples of input addons with icons and buttons:

```html
<div class="input-group">
    <label for="inputAddon">Input Addon</label>
    <div class="input-addon">
        <span class="pl-2 leading-addon material-symbols-rounded text-secondary">
            search
        </span>
        <input type="text" class="input pl-6 py-2" id="inputAddon" placeholder="Input text here">
        <button class="trailing-addon btn btn-primary btn-sm">Search</button>
    </div>
    <div class="helper-text">
        This is Helper text
    </div>
</div>
<div class="input-group">
    <label for="inputAddon">Input Addon</label>
    <div class="input-addon">
        <span class="pl-2 text-secondary leading-addon material-symbols-rounded">
            search
        </span>
        <input type="text" class="input pl-6 py-2" id="inputAddon" placeholder="Input text here">
        <span class="trailing-addon pr-3 text-secondary">$</span>
    </div>
    <div class="helper-text">
        This is Helper text:
    </div>
</div>
```

<div class="component-preview d-block">
<div class="input-group">
    <label for="inputAddon">Input Addon</label>
    <div class="input-addon">
        <span class="pl-2 leading-addon material-symbols-rounded text-secondary">
            search
        </span>
        <input type="text" class="input pl-6 py-2" id="inputAddon" placeholder="Input text here">
        <button class="trailing-addon btn btn-primary btn-sm">Search</button>
    </div>
    <div class="helper-text">
        This is Helper text
    </div>
</div>
<div class="input-group">
    <label for="inputAddon">Input Addon</label>
    <div class="input-addon">
        <span class="pl-2 text-secondary leading-addon material-symbols-rounded">
            search
        </span>
        <input type="text" class="input pl-6 py-2" id="inputAddon" placeholder="Input text here">
        <span class="trailing-addon pr-3 text-secondary">$</span>
    </div>
    <div class="helper-text">
        This is Helper text:
    </div>
</div>
</div>

## Input Addon with Loader

The input addon can also include a loading spinner.

```html
<div class="input-group">
    <label for="inputAddon">Input Addon</label>
    <div class="input-addon">
        <span class="pl-2 text-secondary leading-addon material-symbols-rounded">
            search
        </span>
        <input type="text" class="input pl-6 py-2" id="inputAddon" placeholder="Input text here">
        <div class="trailing-addon pr-2"><span class="circular-loader-sm dark"></span></div>
    </div>
    <div class="helper-text">
        This is Helper text:
    </div>
</div>
```

<div class="component-preview d-block">
<div class="input-group">
    <label for="inputAddon">Input Addon</label>
    <div class="input-addon">
        <span class="pl-2 text-secondary leading-addon material-symbols-rounded">
            search
        </span>
        <input type="text" class="input pl-6 py-2" id="inputAddon" placeholder="Input text here">
        <div class="trailing-addon pr-2"><span class="circular-loader-sm dark"></span></div>
    </div>
    <div class="helper-text">
        This is Helper text:
    </div>
</div>
</div>

## Input States - Valid and Invalid

You can style input fields to indicate their validity or invalidity. Here are examples of input fields with valid and invalid states:

```html
 <div class="input-group">
     <label for="inputstates">Input Label</label>
     <input type="text" class="input is-valid" id="inputstates" placeholder="Input text here" value="Valid Entry">
     <div class="helper-text-valid">
         This is Helper text:
     </div>
 </div>
 <div class="input-group">
     <label for="inputstates">Input Label</label>
     <input type="text" class="input is-invalid" id="inputstates" placeholder="Input text here" value="Invalid Entry">
     <div class="helper-text-invalid">
         This is Helper text:
     </div>
 </div>
```

<div class="component-preview d-block">
<div>
    <div class="input-group">
     <label for="inputstates">Input Label</label>
     <input type="text" class="input is-valid" id="inputstates" placeholder="Input text here" value="Valid Entry">
     <div class="helper-text-valid">
         This is Helper text:
     </div>
 </div>
 <div class="input-group">
     <label for="inputstates">Input Label</label>
     <input type="text" class="input is-invalid" id="inputstates" placeholder="Input text here" value="Invalid Entry">
     <div class="helper-text-invalid">
         This is Helper text:
     </div>
 </div>
</div>
</div>

## Select Input - Styled Browser Based

The select input is a styled version of the default browser-based select input.

```html
<div class="input-group">
<label for="selectInput" class="mt-3">Select</label>
<select class="select" id="selectInput">
    <option>Option 1</option>
    <option>Option 2</option>
</select>
</div>
```

<div class="component-preview d-block">
<div class="input-group">
<label for="selectInput" class="mt-3">Select</label>
<select class="select" id="selectInput">
    <option>Option 1</option>
    <option>Option 2</option>
</select>
</div>
</div>

## Custom Select Input

The custom select input uses a dropdown toggle to display a list of options.

```html
<details class="dropdown w-full">
    <summary class="dropdown-toggle input">Select using Dropdown
    </summary>
    <div class="dropdown-menu w-full">
        <a class="dropdown-item" href="#">Action</a>
        <a class="dropdown-item" href="#">Another action</a>
    </div>
</details>
```

<div class="component-preview d-block">
<details class="dropdown w-full">
    <summary class="dropdown-toggle input">Select using Dropdown
    </summary>
    <div class="dropdown-menu w-full">
        <a class="dropdown-item" href="#">Action</a>
        <a class="dropdown-item" href="#">Another action</a>
    </div>
</details>
</div>

## Textarea with Disabled State

The textarea can be disabled to prevent user input.

```html
<div class="input-group">
    <label for="textareaExample" class="mt-3">Textarea disabled</label>
    <textarea class="textarea" id="textareaExample" rows="3" placeholder="Enter text here" disabled=""></textarea>
</div>
```

<div class="component-preview d-block">
<div class="input-group">
    <label for="textareaExample" class="mt-3">Textarea disabled</label>
    <textarea class="textarea" id="textareaExample" rows="3" placeholder="Enter text here" disabled=""></textarea>
</div>
</div>

## File Input

The file input allows users to select and upload files.

```html
<div class="file-input mt-3">
    <input type="file" id="fileExample">
</div>
```

<div class="component-preview d-block">
<div class="file-input mt-3">
    <input type="file" id="fileExample">
</div>
</div>

## Switch Input

The switch input can be used for binary choices. You can use the `.switch` class to style checkbox inputs as switches. Here is an example:

```html
<label class="switch">
    <input type="checkbox" checked="true">
    <span class="label-text">Switch Label</span>
</label>
```

<div class="component-preview">
<label class="switch">
    <input type="checkbox" checked="true">
    <span class="label-text">Switch Label</span>
</label>
</div>

## Checkbox Input with all the States

The checkbox input can have different states, such as checked and disabled. You can use the `.checkbox` class to style checkbox inputs. Here are examples with different states:

```html
<div>
    <label class="checkbox">
        <input type="checkbox" name="checkbox"> checkbox 1
    </label>
    <label class="checkbox ml-2">
        <input type="checkbox" name="checkbox" id="myCheckbox"> checkbox 2
    </label>
    <label class="checkbox ml-2">
        <input type="checkbox" name="checkbox" disabled="" checked="true"> checkbox 2
    </label>
</div>
```

<div class="component-preview">
<div>
    <label class="checkbox">
        <input type="checkbox" name="checkbox"> checkbox 1
    </label>
    <label class="checkbox ml-2">
        <input type="checkbox" name="checkbox" id="myCheckbox"> checkbox 2
    </label>
    <label class="checkbox ml-2">
        <input type="checkbox" name="checkbox" disabled="" checked="true"> checkbox 2
    </label>
</div>
</div>

## Radio Input with all the States

The radio input can have different states, such as checked and disabled. You can use the `.radio` class to style radio inputs. Here are examples with different states:

```html
<div>
    <label class="radio ">
        <input type="radio" name="Radio"> Radio 1
    </label>
    <label class="radio ml-2">
        <input type="radio" name="Radio"> Radio 2
    </label>
    <label class="radio ml-2">
        <input type="radio" name="Radio" disabled=""> Radio 2
    </label>
</div>
```

<div class="component-preview">
<div>
    <label class="radio ">
        <input type="radio" name="Radio"> Radio 1
    </label>
    <label class="radio ml-2">
        <input type="radio" name="Radio"> Radio 2
    </label>
    <label class="radio ml-2">
        <input type="radio" name="Radio" disabled=""> Radio 2
    </label>
</div>
</div>

## Range Slider

The range slider allows users to choose a value within a specified range. You can use the `.range` class to style range input sliders. Here is an example:

```html
<label for="rangeSlider">Range Slider:</label>
<input type="range" class="range" id="rangeSlider" min="0" />
```

<div class="component-preview">
<div class="">
    <label for="rangeSlider">Range Slider:</label>
    <input type="range" class="range" id="rangeSlider" min="0"/>
    </div>
</div>


## Form Layout - Contact form
here is sample of various form layouts you can do
```html
<form class="card max-w-sm w-full">
<div class="card-body">
    <div class="input-group">
        <label for="name">Name:</label>
        <input type="text" id="name" class="input" placeholder="Enter your name">
        <span class="helper-text">Please enter your full name</span>
    </div>
    <div class="input-group">
        <label for="email">Email:</label>
        <input type="email" id="email" class="input" placeholder="Enter your email">
        <span class="helper-text">We'll never share your email with anyone else</span>
    </div>
    <div class="input-group">
        <label for="message">Message:</label>
        <textarea id="message" class="textarea" placeholder="Your message"></textarea>
    </div>
    <button type="submit" class="btn btn-primary btn-block">Submit</button>
</div>
</form>
```

<div class="component-preview">
<form class="card max-w-sm w-full">
<div class="card-body">
    <div class="input-group">
        <label for="name">Name:</label>
        <input type="text" id="name" class="input" placeholder="Enter your name">
        <span class="helper-text">Please enter your full name</span>
    </div>
    <div class="input-group">
        <label for="email">Email:</label>
        <input type="email" id="email" class="input" placeholder="Enter your email">
        <span class="helper-text">We'll never share your email with anyone else</span>
    </div>
    <div class="input-group">
        <label for="message">Message:</label>
        <textarea id="message" class="textarea" placeholder="Your message"></textarea>
    </div>
    <button type="submit" class="btn btn-primary btn-block">Submit</button>
</div>
</form>
</div>


## Form Layout - Registration Form with Validation
here is sample of various form layouts you can do

```html
<form class="card max-w-sm w-full">
    <div class="card-body">
    <div class="input-group">
            <label for="username">Username:</label>
            <input type="text" id="username" class="input is-valid" placeholder="Username">
            <span class="helper-text-valid">Looks good!</span>
        </div>
        <div class="input-group">
            <label for="password">Password:</label>
            <input type="password" id="password" class="input is-invalid" placeholder="Password">
            <span class="helper-text-invalid">Password must be 8 characters long</span>
        </div>
        <div class="input-group">
            <label for="confirm-password">Confirm Password:</label>
            <input type="password" id="confirm-password" class="input" placeholder="Confirm Password">
        </div>
        <div class="input-group">
        <label class="checkbox">
            <input type="checkbox" name="checkbox"> I Accept anything you tell me. Read <a href="#" class="ml-1"> Anything here</a>
        </label>
        </div>
        <div class="input-group">
        <button type="submit" class="btn btn-primary btn-block mt-2">Register</button>
        </div>
    </div>
</form>
```

<div class="component-preview">
<form class="card max-w-sm w-full">
    <div class="card-body">
    <div class="input-group">
            <label for="username">Username:</label>
            <input type="text" id="username" class="input is-valid" placeholder="Username">
            <span class="helper-text-valid">Looks good!</span>
        </div>
        <div class="input-group">
            <label for="password">Password:</label>
            <input type="password" id="password" class="input is-invalid" placeholder="Password">
            <span class="helper-text-invalid">Password must be 8 characters long</span>
        </div>
        <div class="input-group">
            <label for="confirm-password">Confirm Password:</label>
            <input type="password" id="confirm-password" class="input" placeholder="Confirm Password">
        </div>
        <div class="input-group">
        <label class="checkbox">
            <input type="checkbox" name="checkbox"> I Accept anything you tell me. Read <a href="#" class="ml-1"> Anything here</a>
        </label>
        </div>
        <div class="input-group">
        <button type="submit" class="btn btn-primary btn-block mt-2">Register</button>
        </div>
    </div>
</form>
</div>


## Form Layout - Feedback Form with Interactive Elements
here is sample of various form layouts you can do

```html
<form class="card max-w-sm w-full">
    <div class="card-body">
        <div class="input-group">
            <label for="feedback">Your Feedback:</label>
            <textarea id="feedback" class="textarea" placeholder="Enter your feedback"></textarea>
        </div>
        <div class="input-group">
            <label class="checkbox">
                <input type="checkbox" > Subscribe to newsletter
            </label>
        </div>
        <div class="input-group">
            <label class="radio ">
                <input type="radio" name="rating" > Satisfied
            </label>
            <label class="radio ml-2">
                <input type="radio" name="rating" > Unsatisfied
            </label>
        </div>
        <button type="submit" class="btn btn-outline-primary btn-block mt-2">Send Feedback</button>
    </div>
</form>
```

<div class="component-preview">
<form class="card max-w-sm w-full">
    <div class="card-body">
        <div class="input-group">
            <label for="feedback">Your Feedback:</label>
            <textarea id="feedback" class="textarea" placeholder="Enter your feedback"></textarea>
        </div>
        <div class="input-group">
            <label class="checkbox">
                <input type="checkbox" > Subscribe to newsletter
            </label>
        </div>
        <div class="input-group">
            <label class="radio ">
                <input type="radio" name="rating" > Satisfied
            </label>
            <label class="radio ml-2">
                <input type="radio" name="rating" > Unsatisfied
            </label>
        </div>
        <button type="submit" class="btn btn-outline-primary btn-block mt-2">Send Feedback</button>
    </div>
</form>
</div>

## Form Layout - Settings Form with Range Slider
here is sample of various form layouts you can do

```html
<form class="card max-w-sm w-full">
    <div class="card-body">
        <div class="input-group">
            <label for="volume">Volume Control:</label>
            <input type="range" id="volume" class="range">
        </div>
        <div class="input-group">
            <label>
                <input type="checkbox" class="checkbox"> Enable notifications
            </label>
        </div>
        <button type="submit" class="btn btn-outline-primary btn-block mt-2">Send Feedback</button>
    </div>
</form>
```

<div class="component-preview">
<form class="card max-w-sm w-full">
    <div class="card-body">
        <div class="input-group">
            <label for="volume">Volume Control:</label>
            <input type="range" id="volume" class="range">
        </div>
        <div class="input-group">
            <label  class="checkbox">
                <input type="checkbox"> Enable notifications
            </label>
        </div>
        <button type="submit" class="btn btn-outline-primary btn-block">Save Settings</button>
    </div>
</form>
</div>
