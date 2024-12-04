# React Memory Leak: setInterval without Cleanup

This repository demonstrates a common React memory leak caused by using `setInterval` without properly clearing the interval in `componentWillUnmount`. The `bug.js` file shows the problematic code, while `bugSolution.js` provides the corrected version.

## Problem

The `setInterval` method in the original component continues to run even after the component is unmounted, leading to unnecessary resource consumption and potential memory leaks.

## Solution

The solution involves clearing the interval using `clearInterval` within the `componentWillUnmount` lifecycle method. This ensures that the interval is stopped when the component is removed from the DOM.

## How to Run

1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install` to install necessary dependencies (if any).
4. Run the code using your preferred React development environment.