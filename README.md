# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug: an infinite loop caused by an incorrectly used `useEffect` hook.

## The Bug
The `bug.js` file contains a component with a `useEffect` hook. The empty dependency array `[]` is intended to make the effect run only once after the initial render. However, due to a logical error, the effect indirectly triggers a re-render, leading to an infinite loop.

## The Solution
The `bugSolution.js` file provides a corrected version. The issue is resolved by identifying and rectifying the logic that triggers unwanted re-renders.