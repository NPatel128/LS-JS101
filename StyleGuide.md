# Style Guide

- Set the editor to use spaces (not tabs) for the indention. 
  - Use two spaces for the indention. 
- Limit the line break to 80 characters. 
- Use comments but don't over do it. 
  - Use // for single line comments under 80 characters
  - Use /* */ for multiline comments
- Use camelCase formatting for variable and function names.
- Use PascalCase for constructor functions. 
- Use SCREAMING_SNAKE_CASE for const values. 
- All names (variables, constants, and functions) should only use alphabetic and numberic characters.
  - The first character must be alphabetic.
  - Do not use consecutive underscores in a const name.
  - JS allows for $ in names, but this should only be used when working with a lib that uses $ names.
- Curly braces should be on the same line as the function name or conditional expression, and have a single space before it. 
    ```javascript 
    function test() { 
      //do something here
    } 
    ```
- Use spaces between operators and operands to make code less cluttered. 
    ```javascript
    let sum = x + 5;
    ```
- Use semicolons to terminte each logical line of code unless the line ends with {, }, or :.
