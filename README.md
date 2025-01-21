# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The bug occurs when a dependency is omitted from the `useEffect` hook's dependency array, leading to an infinite render loop.

## Bug Description
The `MyComponent` component uses `useEffect` to log the current value of the `count` state variable to the console.  However, the `count` variable is missing from the dependency array. This causes the effect to run after every render, leading to an infinite loop as the `count` state continuously updates.