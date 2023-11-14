
# Steps

The `Progress Stepper` component in MinimaCSS is designed to provide a clear and visually engaging representation of progression through multiple steps or stages. It's typically used in multi-step forms, wizards, or processes where users need to complete a sequence of actions. The design adheres to simplicity and clarity, ensuring users can easily track their current position and the steps ahead or behind them.

Usage
-----

The `Progress Stepper` is implemented using an ordered list (`<ol>`) with list items (`<li>`) representing each step. The component utilizes several classes to define the states of each step:

*   `.progress-stepper`: The container class applied to the `<ol>` element.
*   `.progress-step`: Applied to each `<li>` element, representing an individual step.
*   `.completed`: A modifier class indicating a step that has been completed.
*   `.current`: A modifier class for the step that is currently active.
*   `.upcoming`: A class for steps that are yet to be completed.

### Example

Here's an example of how the `Progress Stepper` can be implemented:


```html
<nav aria-label="Progress">
    <ol class="progress-stepper">
        <li class="progress-step completed">
            <a href="#" class="group">
                <span class="step-title">Step 1</span>
                <span class="step-description">Basic Details</span>
            </a>
        </li>
        <li class="progress-step current">
            <a href="#" aria-current="step">
                <span class="step-title">Step 2</span>
                <span class="step-description">Company Details</span>
            </a>
        </li>
        <li class="progress-step upcoming">
            <a href="#" class="group">
                <span class="step-title">Step 3</span>
                <span class="step-description">Location Details</span>
            </a>
        </li>
        <li class="progress-step upcoming">
            <a href="#" class="group">
                <span class="step-title">Step 4</span>
                <span class="step-description">Last Submission</span>
            </a>
        </li>
    </ol>
</nav>

```

<div class="component-preview d-block">
<nav aria-label="Progress">
    <ol class="progress-stepper">
        <li class="progress-step completed">
            <a href="#" class="group">
                <span class="step-title">Step 1</span>
                <span class="step-description">Basic Details</span>
            </a>
        </li>
        <li class="progress-step current">
            <a href="#" aria-current="step">
                <span class="step-title">Step 2</span>
                <span class="step-description">Company Details</span>
            </a>
        </li>
        <li class="progress-step upcoming">
            <a href="#" class="group">
                <span class="step-title">Step 3</span>
                <span class="step-description">Location Details</span>
            </a>
        </li>
        <li class="progress-step upcoming">
            <a href="#" class="group">
                <span class="step-title">Step 4</span>
                <span class="step-description">Last Submission</span>
            </a>
        </li>
    </ol>
</nav>

</div>