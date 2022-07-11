# Chapter 10 Sparse Arrays, Cell Arrays, and Structures
___
## 10.1 Sparse Arrays
- When an ordinary array is declared, MATLAB creates a memory location for every element in the array
- A ==sparse matrix== is a large matrix in which the vast majority of the elements are zero
- Storing and working with large sparse matrices, most of whose elements are zero, is a serious waster of both computer memory and CPU time
### The `sparse` Attribute
- MATLAB has a special version of the double data type that is designed to work with sparse arrays
- In this type, only the non-zero elements of an array are allocated with memory locations, and the array is said to have the “sparse” attribute
- Three values are stored for each non-zero element: the value of the element itself, and the row and column numbers where the element is located
### Common Sparse Matrix Functions
![[58D7BE31-012C-4CC5-86A2-BE5684EC7CF7.jpeg]]
![[DC52F833-E5D7-496F-8076-00D0A143A74E.jpeg]]
## 10.2 Cell Arrays
- A ==cell array== is a special MATLAB array whose elements are cells, containers that can hold other MATLAB arrays
- Each element of a cell array is a ==pointer== to another data structure and those data structure can be of different types
- Cell arrays use braces {} instead of parentheses () for selecting  and displaying the contents of cells. The difference is due to the fat that **cell arrays contain data structures instead of data.**
### Cell Array (illustration)
![[2DBD5E1F-35F0-4544-93A9-8DE49AEF7604.jpeg]]
![[E0FE1016-1A87-4BF0-9C42-03C533EA1C80.jpeg]]
### cellplot function
![[B460705C-546F-49FE-A304-2D903240991C.jpeg]]
### Adding a Value to (3, 3)
![[00CDAD48-CAA7-4BC9-BFF8-54273C22C98B.jpeg]]
### Creating Cell Arrays
- Cell array can be created in two ways: by using assignment statements or by reallocating a cell array using the `cell` function (the using assignments statements).
![[E020ED57-D750-48E2-9D20-7F5200B9EEBB.jpeg]]
### The Significance of Cell Arrays
- Cell arrays are extremely flexible wince any amount of any type of data can be stored in each cell. As a result, cell arrays are used in any internal MATLAB data structures 
- We must understand them in order to use many features of Handle Graphics and the GUI
- In addition, the flexibility of cell arrays makes them regular features of functiosn with variable numbers of input arguments and output arguments
## 10.3 Structure Arrays
- A ==structure== is a data type in which each individual element has a name, as opposed to arrays in which elements are only known number
- The individual elements of a structure are known as ==firelds==m and each field in a structure may have a different type
- A ==structure array== is an array of structures. Each structure in the array will have identically the same fields, but the data stored in each field can differ.![[25684A47-5295-4B9C-AF24-F373A7E8FF19.jpeg]]
### Creating a Structure Array
- Structure arrays can be created in two ways:
	1. A field at a time using assignment statements, e.g.,
		- ```str_array.field1 = val1;```
		- ```str_array.field2 = val2;```
	2. All at once using the **struct** functions, e.g.
		 - str_array = struct(‘field1’ , val1, ‘field2’, val2, …)
### Common Structure Functions
![[87C0F2E9-0192-4B22-88F4-2B83F5C2804C.jpeg]]
### Dynamic Field Names
- Dynamic field name is a string enclosed in parentheses at the location where a field name is expected 
	- ```student.name``` = ```Student.(‘name’)```
### Structure Array
- The element of the array is a structure
- Syntax to access a field of a structure array element
	- ```Student(1).name```
## 10.4 Table Arrays
- Table arrays can be considered as a variant of cell array
- Each column of the table has the elements of the same data type
- The data types at different columns can be different
- Each column has a head that takes the name of the variable holding the values of the column. The variable names can be modified.
- Each row of the table can have an optional row name
### Creating a Table
- Create a table from a set of variables
	- ```t = table(var1, var2, …, varN);```
- Create an empty table with a specified size
	- ```t = table(‘Size’, so, ‘VariableTypes’, varTypes);```
### Table Properties
```
Description: ‘’
UserData: []
DimensionNames: (‘Row’ ‘Variables’)
VariableNames: {}
```