# React 18+ useEffect Cleanup Issue with setInterval

This repository demonstrates a common error in React 18+ related to the useEffect hook and the use of setInterval. Forgetting to include a cleanup function in useEffect when using setInterval or setTimeout can lead to memory leaks and unexpected behavior.

## Bug
The `bug.js` file shows the incorrect implementation, where the setInterval function is not properly cleaned up. This will cause the counter to continue incrementing even after the component unmounts, leading to a memory leak.

## Solution
The `bugSolution.js` file demonstrates the corrected implementation, including a cleanup function that uses `clearInterval` to stop the interval when the component unmounts. This prevents memory leaks and ensures the component behaves correctly.
