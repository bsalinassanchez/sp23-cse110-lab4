# Lab 4 Part 2

1. At line 12, the for loop will have finished running through prices.length times. It will have found the discounted prices and pushed it to discounted array. However, the variable it uses `i` is not yet garbage collected and, as a result, when it was console logged, it prints out `3`.
2. At line 13, the for-loop will have finished running through prices.length times. At the end, it calculates the discounted price of the ith element in the prices array. This value will still exist outside of the for-loops block becuase it was declared as a `var`. As a result, when console logged, it prints `150` to the console.
3. At line 14, the for-loop will have finished running through prices.length number of times. At the end, it calculates the "finalPrice" of the ith element in the prices array. Since `finalPrice` was declared with `var` type, it is accessible throughout the function. As a result, after the last iteration of the for-loop is ran, and the final price of the ith element is calculated, when `finalPrice` is console logged it prints `150` to the console.
4. The function will return an array, `discounted`, which holds the discounted-price values of the elements in the `prices` array. The for-loop accesses the ith element of `prices`, calculates the new price, and pushes it to the `discounted` array. `[ 50, 100, 150 ]`
5. At line 12 a `ReferenceError` will be thrown. This happens becuase `i` is declared using `let` type. Since `let` type is a block-scope type, after the for-loop is done running, `i` cannot be accessed outside of the for-loop. As a result, when it is console.logged, an error is thrown.
6. At linen 13 a `ReferenceError` will be thrown. This happens becuase `discountedPrice` is declared using `let` type. Since `let` type is a block-scope type, after the for-loop is done running, `discountedPrice` cannot be accessed outside of the for-loop. As a result, when it is console.logged, an error is thrown.
7. At line 14, the value of `finalPrice` will be console.logged. Since finalPrice is declared with `let` and is in the same block as the console.log, the latest value of `finalPrice` will be logged to the console.
8. The function will return an array, `discounted`, which holds the discounted-price values of the elements in the `prices` arra. The for-loop accesses the ith element of `prices`, calculates the new price, and pushes it to the `discounted` array. `[ 50, 100, 150 ]`
9. A `ReferenceError` is thrown at line 11. This happens becuase `i` is declared using `let` type. Since `let` type is a block-scope type, after the for-loop is done running, `i` cannot be accssed outside of the for-loop. As a result, when it is console.logged, an error is thrown.
10. At line 12, the value of `length` will be printed to the console. This happens becuase `length` is declared at line 4 with the length of the `prices` array. Since it is declared with `const` type, and it isn't reassigned throughout the code, the initial value of the variable will be printed to the console, `3`.
11. The function will return an array, `discounted`, which holds the discounted-price values of the elements in the `prices` arra. The for-loop accesses the ith element of `prices`, calculates the new price, and pushes it to the `discounted` array. `[ 50, 100, 150 ]`. Even though `discounted` is declared as a `contst` type, the elements of the array can be changed but the variable cannot point to a different array.
12. object access
    1. `student.name`
    2. `student["Grad Year"]`
    3. `student.greeting();`
    4. `student["Favorite Teacher"].name`
    5. `student.courseLoad[0]`
13. Arithmetic
    1. "32", since addition was used, it concatenated the 2 to the "3"
    2. `1`, since subtraction was used, it converted "3" to `3' and subtracted 2
    3. `3`, since it added `null`, nothing was added to 3, remained the same
    4. "3null", since we added `null` to a string, it was converted to string and concatenated to the "3"
    5. `4`, since `true` is also `1`, `1` was simply added to 3
    6. `0`, since it added `null` to false, nothing was added to false, remained `0`
    7. "3undefined", since we added `undefined` to a string, it simply concatenated
    8. `NaN`, since we are subtracting, it attempts to subtract something undefined from `3` which results in `NaN`
14. comparison
    1. true, since "2" becomes a number and 2 is greater than 1
    2. false, since the first character of the first string is not less than the first character of the second string
    3. true, since "2" becomes a number and 2 is equal to 2
    4. false, since "2" remains a string and the types are different
    5. false, since true becomes 1 and 1 is not equal to 2
    6. true, since Boolean(2) is true which is equal to true
15. The `==` operator attempts to convert types to a common type by converting to numbers. The `===` operator compares the values strinctly by type AND value.
16. [part2-16](./part2-question16.js)
17. After running the function, the result of the modifyArray function will be the array where for each ith element, the element is multiplied by 2, and a new array is returned with the new values. `modifyArray` simply creates a new array and pushes values based on the return value of `callback`. Since `callback` can be a function, if a function such as `doSomething` is passed, then the value pushed to the new array will be the value of `doSomething(array[i])`
18. [part2-18](./part2-question18.js)
19. the output of the code above is 1,4,3,2
