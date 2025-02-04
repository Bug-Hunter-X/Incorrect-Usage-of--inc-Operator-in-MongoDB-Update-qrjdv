# MongoDB $inc Operator Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The error arises from providing a string value to the `$inc` operator instead of a numerical value.

## Bug Description
The provided code attempts to increment the `counter` field in a MongoDB document.  However, the value passed to `$inc` is a string ("1"), resulting in an error because `$inc` expects a numerical value.

## Solution
The solution involves correcting the `$inc` parameter to provide a number instead of a string. This ensures that the update operation works as expected, incrementing the counter field correctly.

## How to reproduce the error
1. Clone the repo
2. Run `bug.js`