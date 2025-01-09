# Uncommon HTML Error: Accessing Non-Existent Element

This repository demonstrates a common yet easily missed HTML error: attempting to access a DOM element that hasn't been fully parsed or added to the page yet.  This frequently results in a `null` value and a JavaScript error. 

The `bug.html` file illustrates the error, while `bugSolution.html` provides the correct approach using `document.createElement` to create the element and then append it to the DOM. This ensures the element exists before attempting to interact with it.

The error usually occurs because the script tag is in the `<head>` section or above the element it is trying to access.