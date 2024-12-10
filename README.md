# React useEffect Hook Bug

This repository demonstrates a common bug related to the `useEffect` hook in React. The bug occurs when the dependency array is either missing or incorrect, leading to unexpected re-renders and potential performance issues. 

## Bug Description

The provided `MyComponent` uses the `useEffect` hook to log the current count to the console. However, the dependency array is empty, causing the effect to run on every render of the component, regardless of whether the `count` state variable has changed.

## Solution

The solution involves adding `count` to the dependency array of `useEffect`. This ensures that the effect only runs when the `count` value changes.

## How to Reproduce

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs; notice how many times the log message is printed for each click. This should be corrected after applying the solution. 
