# Unhandled Error in Express.js Route Handler

This repository demonstrates a common error in Express.js route handlers:  failure to handle cases where input data is invalid or missing.  Specifically, this example shows a route that fetches a user by ID but lacks proper error handling if the ID is not a number or if the user doesn't exist.

The `bug.js` file contains the erroneous code. The `bugSolution.js` file provides the corrected code with proper error handling.

## Bug

The original code attempts to parse the user ID as an integer without checking if it's actually a number. This can lead to runtime errors if the ID is not numeric.

## Solution

The corrected code includes checks to validate the user ID and handles the case where a user is not found, returning a 404 status code.