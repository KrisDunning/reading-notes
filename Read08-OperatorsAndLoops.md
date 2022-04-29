[Return to main page](https://KrisDunning.github.io/reading-notes/)

# Operators and Loops 

*****

JavaScript uses special `operators` to express common behaviors between variables. There are standard math operators that work mostly as you expect, such as `x+y` , `x-y` ,`z*y` and `x/y`. There is also operators to express "to the power of " , `x^y`. Or even to find if there is a remainder leftover after division, `x%y`.  
One of the more common operators is the assignment operator, `=`. This is used to assign a value to a variable, `let x="theLetterX";`  
Though its not so important now here is a little factoid that just might explain odd operator behavior in the future.

>When chaining these expressions without parentheses or other grouping operators like array literals, the assignment expressions are grouped right to left (they are right-associative), but they are evaluated left to right. --MDN Expressions and Operators  

The next group of operators to familiarize yourself with are the comparison operators.

- Equal(`==`)- Returns `true` if operands are equal
- Not equal(`!=`)- Returns `true` if operands are not equal
- Strict equal(`===`)- Returns `true` if operands are equal and of same type
- Strict not equal(`!==`)- Returns `true` if the operands are of the same type but not equal, or are of differant type
- Greater than(`>`)- Returns `true` if the left operand is greater than the right operand
- Less than(`<`)- Returns `true` if the left operand is greater than the left operand

Arithmatic Operators 

- Remainder(`%`)- Binary operator. Returns the integer remainder of dividing two operands
- Increment(`++`)- Unary operator that adds one to its operand. If used as `++x` then returns the value of its operand after adding one. If used as `x++` then returns the value before incrementing by one. 
-Decrement(`--`)- Same as increments but subtracts 1
- Unary Negations(`-`)- Unary operator that returns the negation of its operand. (ex. x=3. -x=-3)
-Exponentiation(`**`)- calculate the bas to the exponent power. (base**power)  

*****

[Return to main page](https://KrisDunning.github.io/reading-notes/)