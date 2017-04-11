# form-validation-jquery-validate
Learn about form validation using the jQuery Validate plugin

Form validation is an essential part of any production application. Being clear with users about what information they are required to enter on a given form, and in what format, will help ensure that the form filling process is smooth and frustration-free. Typically form validation should be done both before the user submits the form (on the front end), as well as after the form has been submitted (on the back end) to ensure that the information really does meet all your requirements, but we'll just be looking at front end validation here.

For this exercise, we will use the [jQuery Validate](https://jqueryvalidation.org/) plugin to help make form validation easier to set up. Follow these steps to complete the exercise:

1. Open the index.html file under the `exercise` folder in your browser
2. Open the index.html file in your code editor
3. Include the jQuery Validate source, either by linking to a CDN or by downloading it and including the local file
4. In your js/script.js file, add the standard `$(document).ready()` statement
5. Inside the `$(document).ready()' body, select the form using jQuery ($('form') will do) and initialize the validate plugin on it
6. Look at the index.html file in your browser. For all fields marked with an asterisk, add 'data-rule-required="true" to each corresponding `input` element