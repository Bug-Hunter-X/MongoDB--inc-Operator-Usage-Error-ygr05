# MongoDB $inc Operator Usage Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical field in a document. However, if you provide a string value instead of a number, the operation may fail or produce unexpected results.
The `bug.js` file illustrates the incorrect usage, while `bugSolution.js` shows the correct implementation.
## Bug
The bug lies in the incorrect usage of the `$inc` operator within the `updateOne` method. The value being incremented ('1') is enclosed in quotes, making it a string rather than a number. This will cause MongoDB to interpret the operation incorrectly.
## Solution
The solution is to use a numerical value for the increment operation. The `bugSolution.js` file demonstrates the correct usage.
