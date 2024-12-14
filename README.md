# MongoDB $inc Operator Error with String Values

This repository demonstrates a common error when using the `$inc` operator in MongoDB: providing a string value instead of a number.  The `$inc` operator is used to increment a numeric field by a specified amount.  Attempting to increment a field using a string results in an error.

## Bug

The `bug.js` file shows the incorrect usage of the `$inc` operator with a string value.  This will result in an error when executing the update operation.

## Solution

The `bugSolution.js` file provides the correct way to use the `$inc` operator with a numeric value, resolving the error.

## How to Reproduce

1.  Make sure you have MongoDB installed and running.
2. Create a MongoDB collection named `myCollection` with a document containing a field named `count` (e.g., `{ _id: ObjectId(...), count: 0 }`).
3. Run the `bug.js` script. This will result in an error.
4. Run the `bugSolution.js` script. This will increment the `count` field correctly.