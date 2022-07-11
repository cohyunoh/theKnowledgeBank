# Chapter 4: Branching Statements and Program Design
___
## Introduction to Top—Down Design Techniques
- ==[[Top-down design]]== is the process of starting with a large task and breaking it down into *smaller, more easily understandable pieces (sub-tasks).* It also called **modular programming** ^2c7e5e
	1. Clearly ==state the problem== that you are trying to solve
	2. ==Define the inputs== required by the program and the ==outputs== to be produced by the program
	3. Design the ==algorithm== that you intend to implement in the program
	4. Turn the algorithm into MATLAB script
	5. Test the MATLAB script
___
![[6383E991-5603-4D36-AD4A-F6B08C19088F.jpeg]]
___
## Use of Psuedocode
- Describe the algorithm that you intend to implement in a way that is *easy for both you and other people to understand*
- Use [[pseudocode]], a hybrid mixture of MATLAB and English ^5cade7
- Use a **separate line for each distinct idea or segment of code**, but the descriptions on each line are in English
## The Logical Data Type
- The ==logical== data type is a special type of data that can have one of only *two possible values*: **true or false**
- Logical values are **stored in a single byte of memory**. These values are produced by the two special functions ***true*** and ***false***, e.g.,
	- `a1 = true;`
- These are also produced by two types of MATLAB operators: **relational** operators and **logic** operators. MATLAB displays the logic values as *1 for true and 0 for false*
### Relational Operator
![[8C7292CB-CAF9-4A2A-95FE-EEA2D46CB5E6.jpeg]]
### Note on the equality test
- If you are going to test if **two floating numerical values** (number with decimals), the equality test may *fail* because of the ==round off error==. 
	- i.e. two values which appear to be the same on the screen (value displayed after round off) but are not equal.
- For example, two numbers 1.23453 and 1.23454 are not the same. They will look the same if only 5-digit precision is used for display. They all look like 1.2345 which give you the illusion they are the same.
- Always test if the two floating numbers are nearly equal within the round off error
	- i.e. if the difference is less than a preset value
### Logic Operators
![[57774C5C-191A-4A7E-8872-F92EC89C2388.jpeg]]
### True Tables for Logic Operators
![[D6696B10-81FA-44F8-B10F-3E1DF7C28682.jpeg]]
### Function `all`
- Function `all` will return true if all its elements of the input array are `true`
### Hierarchy of Operations
- Arithmetic operations
- Relational operations
- ~ operator
- &, && operators
- |, || operators
- Parentheses can change hierarchy
### Logic Functions
![[91AA0CC8-2B51-4B11-A8C6-650EA854A5B6.jpeg]]
![[4B4F0FA0-2C7E-45F3-84FA-CD3C57B898D0.jpeg]]
## Branches
- [[Branches]] are conditional statements that permit the program to select and execute specific sections of code (called *blocks*) while skipping other sections of code
- There are variations of the **if** statement, the **switch** statement, and the **try/catch** statement
### The if Statement
![[E673141C-D539-453E-9B0E-9D091491740B.jpeg]]
- Always indent the code block within the if statement
### Control Expression in if Statment
- If the expression returns a logic array, the `all` function is applied to implicitly to generate a scalar logic value
`A=[1 2 3];`
`if A>1`
	`fprintf(‘The condition is true’);`
`else`
	`fprintf(‘The condition is false’);`
`end`
### Nested if Statement
- You may use the if statement inside the code block of another if statement
- This will add complexity to the code structure and cause problem during debugging
- Avoid using nested if statement if possible
### Nested vs. Non-Nested if Statement
![[DCB24228-D50E-4427-AA6A-E625E8E1D89F.jpeg]]
### The switch Statement
![[2B4A657A-DB7E-47E9-BC86-A546F70F59E0.jpeg]]
### The try/catch Construct
![[A33B27C9-FA2F-4278-AE8F-AB831D1152AB.jpeg]]
## Debugging MATLAB Programs
- Debug is the process to fund run-time errors and logic errors
- Symbolic debugger can execute, pause, or stop the program so that the programmer can check the intermediate data for errors
- You can find those tools when you open the MATLAB script editor
![[133F52E8-7534-4ABD-889A-BF5C5E8B4CB8.jpeg]]
### Debug Tools
#### Breakpoints
 - Breakpoints: The script will paise at breakpoints. To set up a break point, click the gray area to the right of the statement where you want to set the breakpoint. Click the red dot again will remove it.
