# Chapter 7 Advanced Features of User-Defined Functions
___
## 7.1 Function Functions
- “==Function function==” is the rather awkward name that MATLAB gives to a function whose input arguments include the *names or hands of other functions*
- For example, MATLAB contains a function function called `fzero`. This function locates a zero of the function that is passed to it . To locate a zero of `cos` between 0 and $\pi$, you would write:
```
fzero(‘cos’, [0 pi])
```
## 7.2 Function Handles
- A ==function handle== is a MATLAB data type that holds information to be used in referencing a function
- A function handle can be created in either two possible ways: the @ operator or the `str2func` function
### @ operator
- To create a function handle with the @ operator, just place it in front of the function name
```
function res = my_func(x);
res = x.^2 - 2*x + 1;
handle = @my_func
```
#### Use of Function Handle
![[8656BD4B-1388-437E-8D53-1CB02D9492D4.jpeg]]
### Function str2func
- To create a function handle with the `str2func` function, call the function name in a string
```
function res = my_func(x);
res = x.^2 - 2*x + 2;
hndl = str2func(‘my_func’);
```
#### Use of Function Handle
![[23615A85-A599-46F1-A02B-2A8769D74AB6.jpeg]]
### Significance of Function Handles
- Either function names or function handles can be used to execute most functions.
- However, function handles have certain advantages over function names, such as :
	1. Passing function information to other finctions
	2. Improved performance in repeated operations
	3.  Allow wider access to local functions (subfunctions) and private functions
	4. Include more functions per M-File for easier file management
## 7.3 Eval and Feval Functions
- The keys to the operation of function functions are two special MATLAB functions, `eval` and `feval`
- The function `eval` evaluates a character string as though it had been typed in the Command Window
```
x = eval(‘sin(pi/4)’)
```
- Function `feval` evaluates a named function at a specific input value
```
x = feval(‘sin’, pi/4)
```
### Common Function Functions
![[E94E28B9-8111-4EC7-9509-70BA124A61AA.jpeg]]
## 7.4 Local Functions, Private Functions, and Nested Functions
- The **scope** of a function is defined as the locations within MATLAB from which the function can be accessed
- It must be either in the current folder or on the MATLAB paths
### Local Functions and Private Functions
- There is usually one function in a single file
- If more than one function is present in a file,
	- The top function is a normal or **primary function**. The primary function name is also the m-file name
	- Other functions are **local functions** or **subfunctions**
	- Each functions must include keyword `end` as the last statement
- ==Private functions== are functions that reside in subdirectories with the special name `private`. They are only visita le to other functions in the *private directory*
 or to functions in the parent directory.
### Private Function and Private Folder
![[1EAD45FC-54F0-4C5A-AD17-1187C5BCF07D.jpeg]]
![[8F4150B1-D104-4A1F-B199-47D582793E30.jpeg]]
### Example of Local and Private Functions
![[6CB932E3-960B-4555-B26C-B7F6F2FC0954.jpeg]]
### Nested Functions
- ==Nested functions== are functions that are defined entirely within the body of another function, called the **host function.**
- ==Nested functions== are only visible to the host function and other nested functions embedded at the same level within the same host function.
- A nested function can access to any variables defined with it, plus any variables defined within the host function
![[FB840F93-9060-41CC-8B78-362B03A08EA9.jpeg]]
### Order of Function Evaluation
1. Execute the specified function if it is an nested function. If not,
2. Execute the specified function if it is a local function. If not,
3. Execute the specified function if it is a private function. If not,
4. Execute the specified function if it is in current folder. If not,
5. Execute the specified function if it is on the MATLAB path. If not,
6. Error occurs because no function is found
## 7.6 Anonymous Functions
- An anonymous function is a function “without a name”
- It is a function that is declared in a single MATLAB statement that returns a function handle, which can then be used to execute the function. The general form is:
```
fhandle = @ (arglist) expr
```
- For example,
```
myfunc = @ (x) x.~2 - 2*x - 2
>>myfunc(2)
>>ans = -2
```
## 7.7 Recursive Functions
- A function is said to be ==recursive== if it calls itself. A typical example of a recursive function is the factorial function. It can be written explicitly and recursively as follows:
![[0AABFE17-CC55-4FAA-AD0C-F9C123D7D8E3.jpeg]]
## 7.8 Plotting Functions
- MATLAB also includes two functions, `explot` and `fplot`, that will plot a function directly
- Function `fplot` has the following advantages over `explot`
	1. It is adaptive- -  it calculates and displays more data pints in the regions where the function being plotted is changing most 
	2. It supports user-defined line specifications (color, line style, and marker style)
### fplot
![[49C1D7CD-684D-4D0F-901D-01F6B39670D4.jpeg]]
## 7.7 Histograms (incomplete)
- A **histogram** is a plot showing the distribution of values within a data