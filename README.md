# JavaScript
Notes/Code Snippets

## Basics
-> Case Sensitive  
-> Semicolons optional  
// single line comment  
/* multiline content comment*/

## Variables
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
