# Off-by-One Error in TypeScript Array Iteration

This repository demonstrates a common off-by-one error in TypeScript when iterating over an array. The bug occurs in the `printArray` function, which uses a for loop that attempts to access an index beyond the valid range of the array. This leads to an error in the console.  The solution demonstrates a correct iteration technique.

## Bug
The original code causes a runtime error because the loop condition `i <= arr.length` allows the loop to run one iteration too many. The solution corrects this by changing the condition to `i < arr.length`.