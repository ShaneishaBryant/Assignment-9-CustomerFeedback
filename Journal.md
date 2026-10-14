Phase 1 Question 
What did you accomplish in this phase? What happens if you forget to include event.preventDefault() when handling a form submission in client-side JavaScript, and why is preventing the default behavior necessary when you do not have a backend server endpoint?

Forgetting to include event.preventDefault() causes the browser to trigger its default submission behavior, which reloads the page instantly. As a result, any entered input data, DOM updates, or console logs disappear before they can be processed. Without a backend server endpoint, submitting the form simply reloads the static HTML page or triggers a 404 error if an invalid action URL is specified.



Phase 2 Question
What validation approach did you take to collect and display errors? Did you display errors all at once or one at a time, and what are the user experience pros and cons of your chosen approach?

I used an array with conditional statements to collect error messages and display them inside the #error-box container.

I chose to display all error messages all at once upon submission.

Pros: This approach allows users to fix all missing or invalid fields in a single pass rather than making them play a frustrating "guess-and-check" game. It also provides a clear, summary at the top of the form highlighting everything that requires attention.

Cons: Because the errors are grouped together at the top rather than placed directly next to their respective input fields, users have to scan the form to match each message to its field. Additionally, if the form had severalbinputs, seeing a long list of error messages can feel overwhelming to the user.


Phase 3 Question
What did you accomplish in this phase? Compare using localStorage to cookies: why is localStorage often simpler to use for client-only state, and when might a website prefer cookies over localStorage?

I was able to retrieve information from localStorage to display for a returning user.

localStorage is simpler for client-only state because it offers a clean JavaScript API, provides a higher storage capacity, and keeps data strictly inside the browser without transmitting it over the network.

In contrast, a website would prefer cookies when handling sensitive session tokens that require protection, when the server needs to read user state before returning the initial HTML, or when managing automatic data expiration attributes.



Phase 4 Question
What edge cases or unexpected behaviors did you encounter while testing your form validation and local storage? If you asked an AI tutor to review your code, what suggestions did it make, and how did you decide whether to adopt them.

I did not encounter any unexpected behavior while testing, as the program worked correctly and met my expectations.

When I ran the code through Gemini, it suggested replacing the inline styles in JavaScript with a dedicated CSS class, adding accessibility improvements, and fixing a few missing semicolons.

I adopted the accessibility recommendations and added the missing semicolons to keep the code clean and accessible. However, I chose not to separate the inline JavaScript styles into CSS classes for this iteration. Because the current setup is functioning properly, I did not see an immediate need to alter the working code, though I do recognize the long-term maintainability benefits of separating style definitions from script logic in larger applications.
