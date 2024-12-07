# Uncommon HTML Error: Accessing Non-Existent Element

This repository demonstrates a common yet often overlooked error in HTML: attempting to access a DOM element that does not exist.  The error occurs when JavaScript code tries to manipulate an element using `getElementById` or similar methods, but the specified element is not found in the HTML document.

The `bug.html` file contains the erroneous code.  The `bugSolution.html` shows the corrected version.

This type of error often manifests as an `Uncaught TypeError` in the browser's developer console, specifically mentioning that you are trying to set a property of null.  This is because `getElementById` returns `null` if no element with the specified ID is found.