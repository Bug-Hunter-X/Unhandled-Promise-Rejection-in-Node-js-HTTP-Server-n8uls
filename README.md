# Unhandled Promise Rejection in Node.js HTTP Server

This repository demonstrates a common error in Node.js applications: unhandled promise rejections in asynchronous operations within an HTTP server.  The `bug.js` file contains a server that lacks proper error handling, leading to potential crashes or silent failures.  The `bugSolution.js` file provides a corrected version with robust error handling.

## Bug Description

The server simulates an asynchronous operation that may throw an error.  Without proper error handling, a promise rejection is not caught, resulting in an unhandled promise rejection and a potential server crash.

## Solution

The solution demonstrates how to use `.catch()` to handle potential errors in the asynchronous operation, providing more robust error handling and preventing unhandled promise rejections.