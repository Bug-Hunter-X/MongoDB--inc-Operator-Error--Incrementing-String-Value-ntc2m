# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numerical value in a document.  However, attempting to increment a string value will result in an error.

## Bug
The `bug.js` file contains the incorrect usage of the `$inc` operator, where a string value ('1') is provided instead of a number (1). This will cause a MongoDB error.

## Solution
The `bugSolution.js` file provides the corrected code, which uses a numerical value (1) to properly increment the field using `$inc`.

## How to reproduce the bug
1. Install MongoDB.
2. Create a MongoDB database and collection.
3. Insert a document with a numerical field
4. Run `bug.js`. The update will fail. 
5. Run `bugSolution.js`. The update will work.