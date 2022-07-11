# Programming
---
- Arduino programming language is based on [[C Programming Language|C]].
- Example
	- `digitalWrite(13, HIGH);`
	- `delay(500;`
	- `digitalWrite(13, LOW);`
- **Avoid spaces** in names, *names are case sensitive*.
- The [[Functions|function]] `digitalWrite` defines which pin to set and whether to set that pin *HIGH or LOW*.
	- **Arguments** are passed to a function when it is called.
	- The [[Parameters|parameters]] for a function must be *enclosed in parentheses* and *separated by commas*.
	- Each line ends with a **semicolon**.
- `void setup()` means that you are defining a function called **setup**.
- Some functions are already defined: e.g., `digitalWrite` and `delay`.
- `setup`and `loop` are two functions **you must define**.
	- They *do not return a value* as some functions do, so you have to say that they are **void**, using `void` keyword.
- After `void` comes **the name of the function** and **the parentheses to contain any argument**
	- *No semicolon after the closing parenthesis* because we are defining the function, but **not calling it**.
	- A **block of code** goes in between *curly brace* - define what are to happen when the function is called.
	
## Numeric [[Variables]] and Arithmetic
---
- **Assignment** — `=`
	- Alternative:
		`int degC;`
		`degC = 20;`
- Same arithmetic operations:
	- `+,-,*,/,parenthesis...`
---
## `#define` Directive
---
- `#define` allows you to *associate a value with a name*. 
- Everywhere the name appears in the sketch, **the value will be substituted before the sketch is complied **
	- `#define ledPin 13`
- `#define` *does not use “="*, *does not need a “;”* on the end
- `#define` is a **pre‐complier directive** that is *run before compilation*
- Not the most convenient, but it *does not use any memory to store it*
---
## Return Values
---
- If a [[Function|function]] *returns a value*, you need to specify a **return type**.
- Any *non‐void function* has to have a **return statement** in it.
- The value after return *can be an expression*, instead of the **name of a variable**.
---