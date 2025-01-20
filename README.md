# React useEffect Performance Issue

This repository demonstrates a common performance issue in React applications related to the `useEffect` hook.  The initial implementation of `MyComponent` causes unnecessary re-renders due to the `useEffect` hook being called on every render.

The `bug.js` file shows the problematic code. The `bugSolution.js` file provides the corrected implementation.

## Problem
The `useEffect` hook in the original component runs on every render because the dependency array `[]` is missing. This leads to excessive logging and unnecessary re-renders, impacting performance, especially with more complex components.