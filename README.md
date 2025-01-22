# Uncommon HTML Bug: Incorrect Event Listener

This repository demonstrates a subtle bug related to event listeners in HTML.  Improperly attaching event listeners using the assignment operator (=) can lead to unexpected behavior, especially when multiple listeners are needed.

The `bug.html` file shows the incorrect implementation, while `bugSolution.html` demonstrates the correct way to handle event listeners using `addEventListener`.

## Bug Description

The incorrect approach overwrites any previously attached listeners, resulting in only the last listener being executed. This can be especially problematic in larger, more complex applications.

## Solution

Using `addEventListener` allows you to attach multiple listeners to the same element without overwriting previous ones, ensuring all intended actions are triggered.