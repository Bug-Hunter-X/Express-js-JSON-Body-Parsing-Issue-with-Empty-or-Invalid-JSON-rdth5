This repository contains a demonstration of a common issue in Express.js applications related to JSON body parsing.  When an empty request body or an invalid JSON is sent to an endpoint expecting JSON data, the server might behave unexpectedly.  The `bug.js` file showcases the problem, while `bugSolution.js` provides a solution to handle these cases gracefully.

## Problem

The provided code uses `express.json()` middleware to parse JSON request bodies. However, it doesn't handle cases where the request body is empty or contains invalid JSON. This can result in unexpected behavior, such as the server logging an empty object or throwing errors.

## Solution

The solution involves adding error handling to gracefully handle both empty and invalid JSON requests.  This ensures that the server responds appropriately, preventing unexpected crashes or behavior.