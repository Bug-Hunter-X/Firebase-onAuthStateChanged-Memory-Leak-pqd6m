# Firebase onAuthStateChanged Memory Leak Bug

This repository demonstrates a common error when using Firebase's `onAuthStateChanged` function: forgetting to unsubscribe.  The `onAuthStateChanged` listener continues to run even after the component that uses it is unmounted, leading to memory leaks and potential performance issues.

The `firebaseBug.js` file shows the problematic code, and `firebaseBugSolution.js` demonstrates the correct implementation with unsubscribe function call.