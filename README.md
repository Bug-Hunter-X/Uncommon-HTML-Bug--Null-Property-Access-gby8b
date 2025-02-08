# Uncommon HTML Bug: Null Property Access

This repository demonstrates a subtle bug that can occur in HTML when attempting to access properties of elements that may not exist.  The bug occurs because of accessing properties on a null value, which can lead to a runtime error.

## Bug Description
The bug involves accessing a non-existent property ("nonExistentProperty") of an element after retrieving it using `document.getElementById()`. If the element with the given ID doesn't exist,  `document.getElementById()` returns null which then causes an error when attempting to access a property of the null object.

## Solution
The solution involves explicitly checking for null before accessing any properties of the element.  This prevents the runtime error caused by trying to access a property of a null object.