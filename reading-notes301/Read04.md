# The Conditional (Ternary) Operator Explained

## The if statement
Using a conditional, like an if statement, allows us to specify that a certain block of code should be executed if a certain condition is met.

## The Conditional (Ternary) Operator

**what we need to know:**

1. The condition is what you’re actually testing. The result of your condition should be true or false or at least coerce to either boolean value.
2. A ? separates our conditional from our true value. Anything between the ? and the : is what is executed if the condition evaluates to true.
3. Finally a : colon. If your condition evaluates to false, any code after the colon is executed.

Example — Student Pricing
In this example, we’re coding for a movie theater. The movie theatre offers two ticket prices: $12 for the general public, and $8 for students.
Lets create a variable to keep track of whether a patron is a student or not:

        let isStudent = true;

With this variable we can now use a ternary operator to change the price accordingly:

        let price = isStudent ? 8 : 12
        console.log(price);
        // 8

Since our isStudent boolean is true, the value of 8 is returned from the ternary to the price variable.


# Forms
The < FormControl> component renders a form control with Bootstrap styling. The < FormGroup> component wraps a form control with proper spacing, along with support for a label, help text, and validation state. To ensure accessibility, set controlId on < FormGroup>, and use < FormLabel> for the label.
The < FormControl> component directly renders the < input> or other specified component. If you need to access the value of an uncontrolled < FormControl>, attach a ref to it as you would with an uncontrolled input, then call ReactDOM.findDOMNode(ref) to get the DOM node. You can then interact with that node as you would with any other uncontrolled input.

If your application contains a large number of form groups, we recommend building a higher-level component encapsulating a complete field group that renders the label, the control, and any other necessary components. We don't provide this out-of-the-box, because the composition of those field groups is too specific to an individual application to admit a good one-size-fits-all solution.

## Form controls
For textual form controls—like inputs and textareas—use the FormControl component. FormControl adds some additional styles for general appearance, focus state, sizing, and more.
## Sizing#
Use size on < FormControl> and < FormLabel> to change the size of inputs and labels respectively.
## Readonly
Add the readOnly prop on an input to prevent modification of the input's value. Read-only inputs appear lighter (just like disabled inputs), but retain the standard cursor.
## Readonly plain text
If you want to have readonly elements in your form styled as plain text, use the plaintext prop on FormControls to remove the default form field styling and preserve the correct margin and padding.

## Checkboxes and Radios
For the non-textual checkbox and radio controls, FormCheck provides a single component for both types that adds some additional styling and improved layout.

## Default (stacked)#
By default, any number of checkboxes and radios that are immediate sibling will be vertically stacked and appropriately spaced with FormCheck.
## Customizing FormCheck rendering
When you need tighter control, or want to customize how the FormCheck component renders, it may better to use it's constituent parts directly.

By provided children to the FormCheck you can forgo the default rendering and handle it yourself. (You can still provide an id to the FormCheck or FormGroup and have it propagate to the label and input).
## Floating labels
Wrap a <Form.Control> element in <FloatingLabel> to enable floating labels with Bootstrap’s textual form fields. A placeholder is required on each < Form.Control> as our method of CSS-only floating labels uses the :placeholder-shown pseudo-element.

