# MongoDB $inc operator error
This example demonstrates an incorrect usage of MongoDB's `$inc` operator, specifically when providing a string value instead of a number.  The `$inc` operator is used to increment a numerical field in a document.  Providing a string will lead to an error because the operation is not valid.

## Bug
The bug lies in the use of the string "10" instead of the number 10 when incrementing the `count` field.  MongoDB will throw an error indicating that the update operation is invalid.

## Solution
The solution is to use a numerical value with the `$inc` operator. This ensures that the update operation correctly increments the `count` field.