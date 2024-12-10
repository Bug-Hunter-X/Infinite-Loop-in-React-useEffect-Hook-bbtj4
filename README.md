# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: an infinite loop caused by a missing dependency in the `useEffect` hook. 

The `bug.js` file contains the erroneous code. The `useEffect` hook logs a message to the console on every render.  Because the function is not correctly referencing `count`, the component continuously re-renders. 

The `bugSolution.js` file provides the corrected code, demonstrating the proper use of the dependency array to prevent the infinite loop.