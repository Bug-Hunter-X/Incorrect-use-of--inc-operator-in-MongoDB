# Incorrect use of $inc operator in MongoDB
This example demonstrates an uncommon error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical field.  However, if a string value is provided instead of a number, the operation will not perform as expected. This can lead to subtle and difficult-to-detect bugs.

## Bug
The bug lies in the incorrect use of the `$inc` operator.  The value being incremented should be a number, but a string is used instead.

## Solution
The solution is simple: provide a numerical value to the `$inc` operator.
