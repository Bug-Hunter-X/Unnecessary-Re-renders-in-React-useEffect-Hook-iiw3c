# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common React bug involving the `useEffect` hook. The `useEffect` hook runs more frequently than expected due to missing dependency array.

## Bug Description
The `useEffect` hook in the `MyComponent` function is designed to log the current `count` value to the console.  However, without a proper dependency array, it re-runs on every render, causing excessive logging and potential performance problems. 

## Solution
The solution involves specifying the `count` variable in the dependency array to ensure that the `useEffect` hook runs only when the `count` value changes.