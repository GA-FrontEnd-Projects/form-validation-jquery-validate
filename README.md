# Form Validation with the jQuery Validation Plugin

Form validation is an essential part of any production application. Being clear with users about what information they are required to enter on a given form, and in what format, will help ensure that the form filling process is smooth and frustration-free. Typically form validation should be done both before the user submits the form (on the front end), as well as after the form has been submitted (on the back end) to ensure that the information really does meet all your requirements, but we'll just be looking at front end validation here.

For this exercise, we will use the [jQuery Validation](https://jqueryvalidation.org/) plugin to help make form validation easier to set up. This plugin allows us to set validation rules, error messages, and validation behavior for form elements in a simple, predictable way. Keep the plugin documentation open, and follow these steps to complete the exercise:

1. Open the index.html file under the `exercise` folder in your browser.

2. Open the index.html file in your code editor.

3. Include the jQuery Validation source in index file, either by linking to a CDN or by downloading it and including the local file.

4. In your js/script.js file, add the standard `$(document).ready()`	 statement.

5. Inside the `$(document).ready()` body, select the form using jQuery (`$('form')` will do) and initialize the validate plugin on it.

6. Look at the index.html file in your browser. For all fields marked with an asterisk, add `data-rule-required="true"` to each corresponding `input` element. Do not do this for `input[type="radio"]` elements. Adding this attribute tells the form validator that these fields should have values before the form can be submitted. Once you have done that, reload the page, submit the empty form, and see what happens. 

7. For each of the mandatory fields, create a custom error message by adding `data-msg-required="[your message, without brackets]"` to the input element. Reload the page, submit the empty form, and see your new messages in action.

8. The validation plugin offers [preset validation rules](https://jqueryvalidation.org/documentation/#link-list-of-built-in-validation-methods) for common types of form inputs. For the email address field, add a rule using the `data-rule-x` attribute format that we used earlier to ensure the field is formatted as an email address. Also add an error message for this rule that lets the user know they need to enter an email address.

9. Now add `data-rule-required="true"` to the radio button elements. Also add asterisks next to the field labels to indicate to the user that these fields are required. Watch what happens when the form is submitted without having selected an option for either field. Gross.

10. To fix the error message placement for these fields, inspect the error message in your browser and copy the element that contains the message. Copy and paste the markup below the closing tag for the last `<div class="radio">`, and remove the id attribute and message. Next time you try to submit the form, the error message should display nicely below the radio buttons.

11. Experiment with other validation rules -- try adding maximum or minimum length rules and corresponding custom error messages for different fields.

12. Look through the documentation for the [validate method](https://jqueryvalidation.org/validate/) and turn off validation checks on keyup.


There are many more options and settings to explore with this plugin, but this should give you a general idea of how validation works and how the jQuery Validation plugin makes our lives easier.
