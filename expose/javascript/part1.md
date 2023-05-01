# Lab 4 Part 1

1. values added: 20
2. final result: 20
3. values added: 20
4. the code returns a "ReferenceError" becuase `result` was not defined. This is becuase `result` was declared inside the `if` statement and the `console.log` call is outside of the `if` statement's block scope.
5. the code returns a "TypeError" becuase `result` was declared as a `const` variable which means that its assignment cannot be changed. Since line 9 tried changing the assignment/value of `result`, the code threw an error.
6. the code cannot reach line 13 becuase an error is thrown before the line can be ran.
