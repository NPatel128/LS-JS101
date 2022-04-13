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
      console.log(findUniqueness("","")); //Expected Value:
      console.log(findUniqueness("","")); //Expected Value:
      console.log(findUniqueness("","")); //Expected Value:
      console.log(findUniqueness("","")); //Expected Value:
      console.log(findUniqueness("","")); //Expected Value:
      ```
  - D
    -   
