# Missing 'await' keyword in asynchronous function call in Dapp
This repo contains a simple example demonstrating a common error in Dapps when using asynchronous functions without the 'await' keyword. This can result in unexpected behavior and errors.

## Bug Description
The `getBalance` function is asynchronous.  However, the code calling it does not use `await`, causing the function to immediately return a promise instead of the actual balance. This leads to incorrect calculations and potential errors.

## Solution
The solution involves adding the 'await' keyword before calling the asynchronous function `getBalance`.  This ensures that the code waits for the promise to resolve before continuing. 
