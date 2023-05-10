# DOM-Intro Exercise

# How the DOM loads
This exercise demonstrates the importance of the order in which scripts are loaded on an HTML page, particularly when manipulating the DOM with JavaScript.

The index.html file in the exercise has all the script tags at the bottom of the page to ensure that the DOM elements are fully loaded before the JavaScript references them. A sample HTML file named dom-loading.html is provided to show what happens if the script tags are at the top of the page. In this case, the browser throws an error since the DOM elements have not yet loaded fully, and the JavaScript reference to them returns null.

The solution is to move the script tags to the bottom of the page or better yet use the DOMContentLoaded event to execute JavaScript code only after the DOM elements have loaded. The DOMContentLoaded event is demonstrated in the content-loaded.html file, which shows how to safely execute JavaScript code that references the DOM without needing to move the script tags to the bottom of the page.

The final version of dom-loading.html shows how to use the DOMContentLoaded event to move the JavaScript code to the top of the page and still have it work correctly. The button on the HTML page responds correctly to the click event in this final version.

In summary, this exercise shows that it is essential to place script tags carefully when manipulating the DOM with JavaScript. Using the DOMContentLoaded event is a safer and more reliable way to execute JavaScript code that references the DOM, even if the script tags are placed at the top of the page.
