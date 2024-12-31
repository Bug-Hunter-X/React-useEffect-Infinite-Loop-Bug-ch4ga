# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug arises from an incorrect dependency array, leading to an infinite loop and performance issues.

The `bug.js` file contains the erroneous code, while `bugSolution.js` provides the corrected version.

## Bug Description
The `useEffect` hook is used to update the count every second. However, the dependency array is empty (`[]`), causing the effect to run after every render, triggering a continuous update cycle.

## Solution
The corrected version in `bugSolution.js` includes `count` in the dependency array.  This ensures the effect only runs when the `count` value changes, resolving the infinite loop.