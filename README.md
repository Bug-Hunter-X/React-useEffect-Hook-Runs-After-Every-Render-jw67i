# React useEffect Hook Runs After Every Render

This repository demonstrates a common error when using the React useEffect hook: running the effect after every render instead of only when specific dependencies change. This can lead to performance issues, infinite loops, and unexpected behavior.

## Bug

The `bug.js` file contains a component that uses the useEffect hook without specifying a dependency array.  The console will log a message on every render, leading to unnecessary computations and potential performance problems.

## Solution

The `bugSolution.js` file shows the correct usage of the useEffect hook.  By specifying the dependency array `[count]`, the effect only runs when the `count` state variable changes.