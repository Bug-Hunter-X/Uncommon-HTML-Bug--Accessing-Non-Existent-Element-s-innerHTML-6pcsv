# Uncommon HTML Bug: Accessing Non-Existent Element's innerHTML

This repository demonstrates a subtle bug in HTML/JavaScript where attempting to access and modify the `innerHTML` property of a non-existent element results in a runtime JavaScript error. The bug and its solution are explained in detail below.

## Bug Description
The bug lies in trying to set the `innerHTML` of an element that does not exist in the DOM. This often happens due to typos in the element's ID or because the element hasn't been rendered yet when the script attempts to access it. 

## Solution
The solution is to use error handling (try...catch) and ensure the element exists before attempting to modify its `innerHTML` property.  This prevents the script from crashing.  Alternatively, using more robust DOM manipulation methods can help prevent this type of error.