# MongoDB Aggregation Pipeline Error: Incorrect $inc Usage
This repository demonstrates a common error when using the `$inc` operator within the `$project` stage of a MongoDB aggregation pipeline.  The `$inc` operator is designed to increment a numeric field by a specified value.  However, attempting to use it with an array results in an error.

## Bug Description
The provided code attempts to increment the `count` field using `$inc` with an array argument, which is invalid.  This leads to a pipeline failure.

## Solution
The solution involves correcting the `$inc` operator to directly use the `count` field.

## How to Reproduce
1.  Ensure you have a MongoDB instance running and a collection with sample data.
2.  Run the code in `bug.js`.  It will produce an error.
3.  Run the code in `bugSolution.js`. This will correctly increment the count field.
