# React useEffect Infinite Loop Bug
This repository demonstrates a common React bug related to the `useEffect` hook.  The improper use of the `useEffect` hook without a dependency array causes the component to re-render infinitely, leading to performance issues and potential crashes. The solution demonstrates the correct usage of the dependency array to fix this issue. 

## Bug Description
The bug lies in how the `useEffect` hook is used in `bug.js`.  Without a dependency array (`[]`), the effect runs after every render. This leads to a continuous cycle of re-renders, resulting in the infinite loop. 

## Solution
The solution in `bugSolution.js` shows how to correctly use the dependency array to prevent the infinite loop. By including `count` in the dependency array, the effect only runs when the value of `count` changes.