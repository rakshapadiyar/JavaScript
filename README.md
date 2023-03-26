# JavaScript
Notes/Code Snippets

## Basics
-> Case Sensitive  
-> Semicolons optional  
// single line comment  
/* multiline content comment*/

## Variables
ES5 - var  
JS is dynamically typed -> let, var, const need not declare datatype beforehand  

##### Strict Mode :- "use strict";
The purpose of "use strict" is to indicate that the code should be executed in "strict mode". With strict mode, you can not, for example, use undeclared variables.

> a = 5  
> console.log(a)

This would give error in strict mode as a is not declared.

##### Hoisting :-
Hoisting of variables - in both strict and not strict mode
Variable declarations done at the end of the code will be 'hoisted' to the top.

> "use strict";
> a=5  
> console.log(a) //output 5
