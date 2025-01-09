# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.  Specifically, the `/users/:id` route attempts to parse the `id` parameter as an integer without validating the input.  This can result in unexpected behavior or crashes if the ID is not a number.

## Bug

The `bug.js` file contains the problematic code. The route handler does not handle cases where the `userId` parameter is not a valid integer, leading to potential errors.

## Solution

The `bugSolution.js` file provides a corrected version of the code.  It includes input validation to prevent errors caused by non-numeric user IDs.  It also shows how to use a more robust method to find users by ID, and how to handle the case where a user is not found.