# Unhandled Exception in Asynchronous Node.js Server

This repository demonstrates a common error in Node.js where an unhandled exception within an asynchronous operation causes the server to crash.  The provided solution showcases how to gracefully handle such errors using proper error handling techniques.

## Bug

The `bug.js` file contains a Node.js HTTP server that simulates an asynchronous operation.  In 50% of cases, it throws an error. This unhandled exception results in the server crashing without any informative error message.

## Solution

The `bugSolution.js` file presents a corrected version of the server. It uses a `try...catch` block to handle potential errors, ensuring that the server continues to operate even if an error occurs within the asynchronous operation.  The error is then logged to the console for debugging purposes.

This approach prevents server crashes and promotes robust error handling within asynchronous Node.js applications.