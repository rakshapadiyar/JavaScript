# JavaScript
Notes/Code Snippets

## [i] Basics
-> Case Sensitive  
-> Semicolons optional  
// single line comment  
/* multiline content comment*/

## [ii] Variables
 · ES5 - var  
 · JS is dynamically typed -> let, var, const need not declare datatype beforehand  

##### Strict Mode :- "use strict";
The purpose of "use strict" is to indicate that the code should be executed in "strict mode".
 With strict mode, you can not, for example, use undeclared variables.

> a = 5  
> console.log(a)

This would not give error in non-strict mode even though 'a' is not declared.

##### Hoisting :-
 · Hoisting of variables - in both strict and not strict mode  
 · Variable declarations done at the end of the code will be 'hoisted' to the top.

> "use strict";  
> a=5  
> console.log(a) //output 5

##### Let vs Var vs Const

##### a) Scope
> for ( var/let/const i=0;i<5;i++ )  
>  console.log(i);  
> //
> console.log(i);  

output :  
for var : 0 1 2 3 4 4  
for let : 0 1 2 3 4 i is undefined  
for const : Assignment to constant variable error  

var : function scoped  
let : block scoped  
const : block skoped

##### b) Redeclaring
var can be redeclared.  
let and const cannot be redeclared. If done, it gives error message "Identifier a has already been declared"  

##### c) Redefining
var can be redefined.  
> var a = 5  
> a= 6  
No error

let can be redefined  
> let a = 5  
> a = 7  
No error  

const cannot be redefined  
> const a = 6  
> a = 9  
Type error  : Assignment to a constant variable.

Suggestion :
Avoid usig var  
If value keeps changing, use let. Else, use const.

## [iii] Operators  
  
  #### 1) Relational Operators 
< , < , >= , <= , == , !=  

  #### 2) Arithmetic Operators
+, -, /, * , %  

  #### 3) Logical Operators
&&, ||, !

  #### 4) Bitwise Operators
&, | , ~, !, >> , << , >>>   
>>> '>>>' is Fill right shift' operator : op1 >>> op2.
This operator shifts the first operand the specified number of bits to the right. Excess bits shifted off to the right are discarded. Zero bits are shifted in from the left.  
Example : 101001 >>> 2 = 001010  
( There is no <<< operator )

  #### 5) Assignment Operators
= , +=, -= , *= , /=
 
  #### 6) Other Operators
  typeof, + , -  
  + => console.log("a" + x) //concatination
  - => let a=10, b=-a;

## [iv] Decision Making

#### 1) if else statement
#### 2) if else ladder
#### 3) switch statement
>switch( condition )  
{  
case "a" : {  
//code
break
}  
case "b" : {  
//code
break
}  
default :{  
}  
}
## [v] Looping Statements
#### 1) Definite looping
number of times the loop runs is pre defined
ex : for loop, for-in loop, for-of loop  

##### a) for loop
factorial of a number   
>for(let i=n ; i>=0 ; i--)  
{  
  factorial *= i;  
}  

##### b) for in loop
>var student = { "name" : "Anu" , "age" : 19 }  
for( let i in student )    
{  
 console.log(i) // prints name,age  
 console.log(student[i]) //prints Anu, 19  
 
##### c) for of loop


#### 2) Indefinite looping
loop runs as long as condition is true
ex : while loop, do while loop
  
  ->break stateement :to exit from further loop iterations.  
  -> continue :  to stop current iteration of loop and continue further iterations


