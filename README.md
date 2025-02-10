# Uncommon HTML/JavaScript DOM Error
This repository demonstrates a subtle error that can occur when interacting with the Document Object Model (DOM) in JavaScript.  The problem arises from attempting to access and modify a DOM element before the browser has completed parsing the HTML and adding the element to the DOM. 

**bug.html:** Shows the incorrect code that causes the error.
**bugSolution.html:** Provides the corrected code using the DOMContentLoaded event.

The key takeaway is the importance of ensuring that DOM elements are available before attempting to manipulate them. Using event listeners (like `DOMContentLoaded`) ensures your JavaScript code executes after the page's HTML is fully loaded.