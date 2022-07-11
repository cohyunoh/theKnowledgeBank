# Other Functions
---
`x=linspace(-2*pi,2*pi,1000);`
`y=sin(x);`
`plot(x,y)`
- This whole block of code creates a graph of a sine wave from -2pi to 2pi.
- The first line defines *x* as an array of values from **-2pi to 2pi** in increments of **4pi/1000**. 
	- Without the 1000, the default number will be 100
	- There are exactly 1000 values in that array
- The second line defines *y* as the sine of all the values in the array of x
- The third line plots y against x to create the sine wave

---
- Just typing the name of a script (ends in .m) in the command window will **run that script**
- `clear` gets *rid of the variables in the workspace window*
- `clc` *clears command window*
	- Command history is still there though when pressing **up arrow**
- `help sin` tells you what the function does, in this case `sin`
- `lookfor inverse` will find all functions that have the word *inverse* in there description
- ==ctrl + c== stops code
---