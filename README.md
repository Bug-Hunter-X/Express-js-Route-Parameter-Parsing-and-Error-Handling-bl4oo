# Express.js Route Parameter Parsing and Error Handling

This repository demonstrates a common error in Express.js applications: improper handling of route parameters. The provided code lacks input validation, which may result in unexpected behavior or crashes when non-numeric user IDs are used.

The `bug.js` file shows the problematic code, while `bugSolution.js` provides a corrected version.

## Bug

The primary issue is the absence of error handling and input validation for the `userId` parameter.  If the user inputs a non-numeric value, `parseInt(userId)` will return `NaN`, leading to a potential crash or incorrect results. The improved version handles this to prevent unexpected behavior and enhance security.