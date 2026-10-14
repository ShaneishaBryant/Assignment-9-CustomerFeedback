Phase 1 Question 
What did you accomplish in this phase? What happens if you forget to include event.preventDefault() when handling a form submission in client-side JavaScript, and why is preventing the default behavior necessary when you do not have a backend server endpoint?

Forgetting to include event.preventDefault() causes the browser to trigger its default submission behavior, which reloads the page instantly. As a result, any entered input data, DOM updates, or console logs disappear before they can be processed. Without a backend server endpoint, submitting the form simply reloads the static HTML page or triggers a 404 error if an invalid action URL is specified.



Phase 2 Question
What validation approach did you take to collect and display errors? Did you display errors all at once or one at a time, and what are the user experience pros and cons of your chosen approach?

I used an array with conditional statements to collect error messages and display them inside the #error-box container.

I chose to display all error messages all at once upon submission.

Pros: This approach allows users to fix all missing or invalid fields in a single pass rather than making them play a frustrating "guess-and-check" game. It also provides a clear, summary at the top of the form highlighting everything that requires attention.

Cons: Because the errors are grouped together at the top rather than placed directly next to their respective input fields, users have to scan the form to match each message to its field. Additionally, if the form had severalbinputs, seeing a long list of error messages can feel overwhelming to the user.