# Chapter 5: Loops and Vectorization
___
## Introduction
- **Loops** are MATLAB statements that *execute a sequence of statements more than once*
- There are two basic forms of loop constructs:
	- ==while== loop and ==for== loop
- **Vectorization** is an alternate and faster way to perform the same function as many MATLAB **for** loops
![[Recording 20220222080918.m4a]]
## 5.1 The while loop
- A **while** loop is a *block of statements that are repeated until a certain condition is satisfied.*

___
![[C078C5A2-4F77-43D4-BEAE-8B0409A97328.jpeg]]

___
- **while** loop evaluates the condition first
- The code block could never be executed if the condition is NOT true at the first iteration
- **while** loop may not be able to exit if the condition is always true
- The code block in the **while** loop is a block of statements that are repeated until the condition is false.
![[Recording 20220222081746.m4a]]
### First Live Script
![[Recording 20220222082425.m4a]]
### Example 5.1 - Statistical Analysis
- What is the problem?
	- *Calculate the average and the standard deviation of a set of measurements which are either positive or zero. There is no prior knowledge of the number of measurements*
- What are the inputs?
	- *Unknown number of measurement values*
- What are the outputs?
	- *Mean and standard deviation*
- Design the algorithm: **Pseudocode**
- Procedure
	1. **Initialize** n, sum_x and sum_x2 to 0
	2. **Prompt** user for the measurement data
	3. **Read** the data and store it in x
	4. **Repeat** step 5 if non-negative value is entered
	5. **Calculate** sum and the square sum of the entered measurements and count the number measurements entered
	6. **Output** results
*Live script section at the end*

![[Recording 20220222084444.m4a]]
## 5.2 The for Loop
- The **for** loop is to execute block of statements for a specified number of times

___
![[5E4FDCAB-5158-40F4-AEEF-852A0EDFA8DF.jpeg]]

___
- The **expr** in the for loop should be a vector
- The **index** will pack each element in the vector in every loop.
	- i.e. Index picks the first element in the vector in the first iteration, the second element in the second interation
	- The number of iterations of a **for** loop is determined by the number of elements in the vector
![[Recording 20220222084900.m4a]]
### Specials on **FOR** loop
1. ==Don’t modify the loop index within the body of a loop==, otherwise may cause hard-to-find errors
2. ==Pre-allocate arrays== - if you are going to modify an array in a loop, *allocate it beforehand so the loop is not creating a new array with each pass*
![[Recording 20220222085325.m4a]]
### Break and Continue Commands
- The **break** statement *terminates the execution of a loop and passes control to the next statement after the end of the loop*
- The **continue** statement *terminates the current pass through the loop and returns control to the top of the loop*
![[Recording 20220222085700.m4a]]
### Use of Loops
- Select the correct type of loop structure
	- Use **FOR loop** for a fixed number of iterations. It is common when the code processes the data in a vector
	- Use **WHILE loop** if the number of iterations is unknown. Make sure that the code in the WHILE loop will change the loop condition
- Use initialization code before entering the loop
	- All variables that carry data between iterations should be initialized
	- The variable on the left side of the “=“ operator after the FOR keyword does not need initialization because it will get values from the vector on the right side of the “=“ operator in every iteration.
- The code block inside the loop usually has a **branch statement** to process data according to certain conditions. Examples are:
	- *Check if temporary maximum value is smaller than the current value from the vector*
	- *Check if the current value from the vector is an even number*
	- *Check if the current value from the vector is an odd number*
	- *Check if the current value from the vector is divisible by an integer*
- The code block inside the loop **should update the initialized value**

![[Recording 20220222091410.m4a]]
### Example
- Find the day of year corresponding to a specific date
- The day of year is the number of days (including the current day) that have elapsed since the beginning of a given year. It is a number in the range 1 to 365 for ordinary years and 1 to 366 for leap years
#### Pseudo Code
- Get day, month, and year to convert
- Check for leap year, and add extra day if necessary
	- Years divisible by 400 are leap years
	- Other centuries are not leap years
	- Every 4th year is a leap year
	- Other years are not leap years
- Calculate day of year by adding current day to the days in the previous months
- Add days in months from January to month before current month
	- For January, March, May, July, October, December, add 31
	- For April, June, September, November, add 30
	- For February, add 28 plus 1 if it is a leap year
- Output the day of the year
## 5.3 Logical Arrays and Vectorization
- Logical arrays can serve as a **mask** for arithmetic operations
- A **mask** is an *array that selects the elements of another array for use in an operation*. The specified operation will then be applied to the selected elements, and not to the remaining elements
![[FB098F41-7D05-4B4F-8436-086F26D681CA.jpeg]]
### Vectorization
- **Vectorization** is the process of replacing loops with vectorized statements and allows users to do the calculation for all elements in a single statement rather than looping to perform the calculation for each element, which speeds up your code
![[9F227BE4-74B1-4AB3-A6C1-640D01788EA3.jpeg]]
## 5.4 The MATLAB Profiler
- MATLAP includes a profiler, which can be used to identify the parts of a program that consume the most execution time
- You can start the MATLAB profiler by selecting the Run and Time tool from the Code section of the Home Tab
- After the profiler runs, a Profiler summary is displayed, showing how much time is spent in each function being profiled. You can then use that information to identify the slow portions of the code and work to speed them up with vectorization and similar techniques
## 5.5 The textread Function
- The **textread** function reads text files that are formatted into columns of data, where each column can be of a different type, and stores the contents of each column in a separate output array
>[a,b,c,…] = textread(filename,format,n);
- The **textread** function is much more useful and flexible than the **load** command because **load** only reads the data saved in a workspace file
## 5.7 Summary (incomplete)
- The **while** loop us used to repeat a section of code in cases where