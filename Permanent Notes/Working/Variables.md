# Variables
---
- When *defining a variable* in [[C Programming Language|C]], you need to specify the **type of the variable**.
	- The type of variable is a feature of the variable called [[Data Types|data type]].
- Syntax
	- `(data type) (name of variable) = (value that matches data type)`
## Global, Local, and Static Variables
---
- **Global variables** are variables defined outside of all the functions and can be called from each one.
- **Local variables** are the ones defined within functions, whether are as a [[Parameters|parameter]] or not.
	- These can *override global variables*.
	- This overriding only happens within the function.
- **Static variables** are only initialized once within a function, specifically the loop function, which means its value does not reset when the loop function is ran again.