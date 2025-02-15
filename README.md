# Unhandled Asynchronous Error in Node.js

This repository demonstrates a common error in Node.js applications: unhandled errors within asynchronous operations.  The `bug.js` file contains code that simulates an asynchronous request that may fail.  The error isn't properly caught, leading to a crash. The `bugSolution.js` provides a solution using error handling techniques to prevent this crash. 

## How to reproduce
1. Clone this repository.
2. Navigate to the directory.
3. Run `node bug.js`.
4. Observe the error or crash. (50% chance)
5. Run `node bugSolution.js`. (Should always work.)

## Solution
The solution utilizes `try...catch` blocks within asynchronous callbacks, or promise rejection handling, to gracefully handle potential errors and prevent crashes.