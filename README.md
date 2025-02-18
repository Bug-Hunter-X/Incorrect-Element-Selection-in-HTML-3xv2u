# Uncommon HTML Bug: Incorrect Element Selection

This repository demonstrates a common yet easily overlooked error in HTML when using JavaScript to manipulate the DOM. The bug lies in using `document.querySelector('div')` to select a specific div element with a known ID.  Using `getElementById` is a more precise and efficient solution.

## Bug Description

The provided HTML code uses `document.querySelector('div')` to hide all divs, instead of hiding only the one with the specific ID `myDiv`.  This is because `querySelector` selects the first element that matches the selector, and in this case, any div element will be selected.

## Solution

The solution uses `document.getElementById('myDiv')` to accurately select the element with the ID "myDiv" and hide it.