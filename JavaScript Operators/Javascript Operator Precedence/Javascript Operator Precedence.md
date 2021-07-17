## Javascript Operator Precedence:
Operators have precedence. Precedence defines the order in which the expression will be evaluated. Operators are used to building expression. Expressions are sequences of operators and operands that are evaluated to a single value.

# Operator Precedence from highest to lowest.
 
 `Precedence	Operators`
| Precedence        | Operators           
| ------------- |:-------------
| Highest       |( )
|               |++ — (postfix) new typeof 
|               |++ — (prefix) + – (unary) ! ~ 
|               |* / %
|               |<< >> 
|               |< > <= >= is as 
|               |== != 
|Lowest         |= *= /= %= += -= <<= >>= &= ^= |=
|Higher         |^ 
|               || 
|               |&&
|               ||| 
|               |?: 
|Lower          |&

# The Parenthesis operator always has the highest precedence.
Below is the arithmetic expression.

Example: var a = 100 + 50 * 3; By looking at this example it makes us think whether the result of the above example would be 150*3 or 100+150?
# Which operation will go to execute first? Whether the addition or  the multiplication done first?
As we have already learned in school mathematics rules, multiplication is done first. Multiplication (*) and division ( / ) have higher precedence than addition ( + ) and subtraction ( – ). As soon as we use the parenthesis the precedence gets changed.
# Below are the different types of operators JavaScript supports:
![Operator](https://dotnettutorials.net/wp-content/uploads/2020/02/JavaScript-Operators.png)

# JavaScript Arithmetic Operators with Examples:
Arithmetic operators +, -, *, / are the same as in math. The arithmetic operators are as follows:
# Addition (+) Operator:
This operator adds numbers (Operands). See the following example.

var a = 5;<br>
var b = 2;<br>
var c = a + b;<br>
alert(c);  //7
# Subtraction (-)  Operator:
This operator subtracts the second number (operand) from the first operand. Have a look at the following example.

var a = 5;<br>
var b = 2;<br>
var c = a – b;<br>
alert(c);  //3
# Multiplication (*) Operator:
This operator multiplies operands. Following is an example of Multiplication operator.

var a = 5;<br>
var b = 2;<br>
var c = a * b;<br>
alert(c);  //10
# Division (/) Operator:
This operator divide the numerator number by denominator number. Here is an example of Divison Operator.

var a = 5;<br>
var b = 2;<br>
var c = a / b;<br>
alert(c);  //2.5
# Modulus (%) Operator:
This operator returns the remainder from the division of numbers. The following is an example of modulus operator.

var a = 5;<br>
var b = 2;<br>
var c = a % b;<br>
alert(c);  //1
# Increment (++) Operator
This operator increments numbers by one. Example is given below.

var a = 5;<br>
a++;<br>
var c = a;<br>
alert(c); //6
# Decrement (–) Operator:
This operator decrements numbers by one. The following is an example of decrement operator:

var a = 5;<br>
a–;<br>
var c = a;<br>
alert(c); //4
# Exponentiation (**) Operator
This operator raises the first operand/number to the power of the second operand/number. Please have a look at the following code which is an example of an exponentiation operator.

var a = 5;<br>
var c = a ** 2;<br>
alert(c); //25 i.e. 5**2 =5*5 that is 25.
# JavaScript Comparison (Relational) Operators with Examples:
The comparison operators ==, ===, !=, !==, >, >=, < and <= are used in conditional statements to compare operands and to take the action on the output. The comparison operators are as follows:
## Is equal to (==) Operator
This operator is used to compare the values of two operands to check if both are equal or not. If yes then the condition becomes true else false. In order to understand this better, please have a look at the following example.

var a = 5, b = 4;<br>
alert(a == b); //false
## Identical –equal and of the same type (===) Operator:
This three-time equal sign is called strictly equal sign it checks both operands values as well as the data type. The following is an example of this operator.

var a = 5, b = 5, c = “5”;<br>
alert(a === b); //true<br>
alert(a === c); //false<br>
In the above example, a===b will return true, because the value of a and b is 5 and both are number data types, a===c will return false because the value of a and c is 5, but the data types are different.
## Not equal to (!=) Operator
This operator is called not equal to. It checks the value of both operands are equal or not. If the values are not equal then the condition becomes true else false. Following is the example.

var a = 5, b = 4;<br>
alert(a != b);//true
## Not equal value or not equal type (!== ) Operator:
This operator is used to check both the values as well as the data types. It checks the values of both operands whether equal or not. If both the operand values are not equal or data types are of the same type then the condition becomes true. Please have a look at the following example to understand this better.
var a = 5, b = 4, c = “5”;<br>
alert(a !== 5);//false<br>
alert(a !== b);//true<br>
alert(a !== c);//true 
## Greater than (>) Operator:
This operator is used to check if the left operand is greater than the right operand. When the left one is greater than the right one, the condition becomes true else false. Following is the example to understand this operator.
var a = 5, b = 4;<br>
alert(a > b); //true
## Greater than or Equal to (>= ) Operator:
This operator is used to check if the left operand is greater than or equal to the right operand. If yes then the condition becomes true else false. An example is given below. 
var a = 5, b = 8, c = 5;<br>
alert(a >= b);//false<br>
alert(a >= c)//true
## Less than (<) Operator:
This operator is used to check if the left operand is less than the right operand. When the left one is less than the right one, the condition is valid. Here is an example to understand this operator.
var a = 5, b = 4;<br>
alert(a < b);  //false
## Less than or Equal to (<=) Operator
This operator is used to check if the left operand is less than or equal to the right operand. If yes then the condition becomes true else false. Please have a look at the following code which is an example of less than or equal to operator.
var a = 5, b = 8, c = 5;<br>
alert(a <= b);//true<br>
alert(a <= c)//true
## JavaScript Bitwise Operators with Examples:
The bitwise operators are work for 32-bit integers in JavaScript. Bitwise operator ~ turns all 0 to 1 and all 1 to 0. Like ! for Boolean expressions but works bit by bit. The operators |, &, and ^ behave like bitwise ||, && and ^. The << and >> move the bits left or right.
The behavior of the operators &, | and ^:

| Operation	| &	| &	| &	| &	| |	| |	| |	| |	| ^	| ^	| ^	| ^
| ------------- |:-------------| ------------- |:-------------
| Operand1	| 0	| 0	| 1	| 1	| 0	| 0	| 1	| 1	| 0	| 0	| 1	| 1
| ------------- |:-------------| ------------- |:-------------
| Operand2	| 0	| 1	| 0	| 1	| 0	| 1	| 0	| 1	| 0	| 1	| 0	| 1
| ------------- |:-------------| ------------- |:-------------
| Result	| 0	| 0	| 0	| 1	| 0	| 1	| 1	| 1	| 0	| 1	| 1	| 0 