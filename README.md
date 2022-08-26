# Coding Dojo 2022 

## Task

You need to create a function, which "translates" a string following some specific rules:
 - You need to convert the string to character codes (C => 67, c => 99, etc...) (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charCodeAt)
 - You need to convert the number to binary (67 => 1000011, 99 => 1100011)
 - You need to convert the binary number to "unary" syntax
   - unary only contains zeroes and spaces
   - consist of blocks of two separated by a space
     - first block representing the number 0 or 1 (1 => 0 // 0 => 00)
     - second block is how many times that number repeat
    
    Ex:
   - decimal 1 =>  binary 1 => 0 0  (first zero means 1, second zero count means that it appears 1 times)
   - decimal 3 => binary 11 => 0 00 (first zero means 1, second zero count means that it appears 2 times)
   - decimal 0 => binary 0 => 00 0 (first double zero means 0, second zero count means that it appears 2 times)
   - decimal 99 => binary 1100011 => 0 00 00 000 0 00 
     - 3 groups (0 00 // 00 000 / 0 00)
     - 0 00 => means 1 x2
     - 00 000 => means 0 x3
     - 0 00 => means 1 x2
 - When you're given a character string and not a single character, you need to convert every character individually and put two spaces between the codes representing a single character
   - Ex: 
     - a => 0 00 00 0000 0 0
     - aa => 0 00 00 0000 0 0  0 00 00 0000 0 0
     
## Expectations
- You can't change anything in the test file, but you can completely re-write the implementation file.
- You need to fulfill the tests, but you can decide on the algorithm (you can change / skip parts if you find a better one)
- You can't use external libraries only built-in features of Node
- Tests need to run in random order as well (so burning in the correct values to return is not a solution)
     
## To win, you need to write the shortest implementation 
You can check the length of your implementation by typing `wc -c index.js`

