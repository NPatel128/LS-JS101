# PEDAC
- The Two Layer Problem is when someone to trying to solve a problem while simutaneously memorizing the syntax of a particular language. 
- PEDAC helps solve this by breaking a problem down into parts.
  - P = Understand the ***P***roblem
  - E = Write ***E***xamples / Test Cases 
  - D = ***D***ata Structures
  - A = ***A***lgorithm
  - C = ***C***ode with intent
- Example Problem: Make a function that takes in two strings and returns the unique letters between the two strings. 
  - P
    - Input: 2 strings
    - Output: String
    - Rules:
      - Store any characters that appear in only one of the two strings
      - Return an empty string if both strings contain identical characters
      - If both strings are empty then return an empty string.
      - Uppercase and lowercase letters are different. 
      - The strings only contain alphabetic and numeric characters. 

  - E
      ```javascript
      console.log(findUniqueness("ABC","abc")); //Expected Value: "ABCabc"
      console.log(findUniqueness("","")); //Expected Value: ""
      console.log(findUniqueness("qwe","qweasd")); //Expected Value: "asd"
      console.log(findUniqueness("123","456")); //Expected Value: "123456"
      console.log(findUniqueness("asdf","fsda")); //Expected Value: ""
      ```
  - D
    - Using a string will suffice. 
  - A
    - Create a string that will hold the unique characters
    - Iterate through the first string's characters
      - While iterating check to see if the current character is included in the second string.
        - if it is not included in the second string then add it to the unique characters. 
    - Iterate thorugh the second strings's characters
      - While iterating check to see if the current characer is incuded in the first string.
        - If it is not included in the first string then add it to the unique characters
    - Return the unique characters
  - C
    ```javascript
    function findUniqueness(str1, str2) {
      let unique = ``;
      for (let i = 0; i < str1.length; i += 1) {
        if (!str2.includes(str1[i])) {
          unique = unique.concat(str1[i]);
        }
      }
      for (let i = 0; i < str2.length; i += 1) {
        if (!str1.includes(str2[i])) {
          unique = unique.concat(str2[i]);
        }
      }
      return unique;
    }
    ```
