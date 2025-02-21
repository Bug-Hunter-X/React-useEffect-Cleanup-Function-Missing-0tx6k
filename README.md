# React useEffect Cleanup Function Bug

This repository demonstrates a common React bug: forgetting to include a cleanup function in the `useEffect` hook.  This leads to memory leaks and potential unexpected behavior.

## Bug

The `bug.js` file contains a React component that adds an event listener using `useEffect` but fails to remove it when the component unmounts.

## Solution

The `bugSolution.js` file provides the corrected version of the component.  It includes a cleanup function that removes the event listener, preventing memory leaks.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server. You will notice that in the original example, memory will leak as the event listener is not removed.