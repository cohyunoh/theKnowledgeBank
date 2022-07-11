# Chapter 11 Input/Output Functions
___
## 11.1 The `textread` Function
- The ==textread== function reads text files that are formatted into columns of data, where each column can be of a different type, and stores the contents of each column in a separate output array of cell array.
```
[a,b,c,...] = textread(filename, format, n);
```
## 11.2 More about `load` and `save` Commands
- The ==save== command saves MATLAB workspace data to disk, and the ==load== command loads data from disk into the workspace
- The ==save== command can save data either in a special binary format called a MAT file or in an ordinary text file
- The form of the ==save== command is:
```
save filename [content] [optioms]
```
### Table 11.1 Content
![[BA72C061-FED5-49A7-B284-8194556DF8D4.jpeg]]
### Table 11.2 Options
![[0695843E-2EE6-47F2-BC45-588ADE8A5022.jpeg]]
### Examples of save command
- Save entire workspace to a mat file (binary file)
	```
	save ‘test.mat’
	```
- Save selected variables to a mat file (binary file)
```
	save ‘test.txt’ a b c
```
- Save selected variables to a text file
```
	save ‘test.mat’ a b c ‘-ascii’
```
### More about `load` and `save` Commands (continued)
- The ==load== command can load data from MAT files or from ordinary text files. The form of the ==load== command is:
```
load filename [options] [content]
```
- The ==load== all by itself loads all of the data in file into the current workspace
#### Table 11.3 for options in load
![[15EA0DFC-1AA5-4AC6-8BA6-B8C07DCF0DCE.jpeg]]
### Examples of load command
- Load data from mat file to workspace 
```
	load ‘test.mat’
```
- Load selected variables from mat file to workspace. You must know the variable names
```
	load ‘test.mat’ a b c
```
- Load data in the text file to a variable of the same as the file name
```
	load. ‘test.txt’ ‘-ascii’
```
### File Operation (Read)
![[CB13AFB8-8A39-4987-A562-61D668362D5C.jpeg]]
### File Operation (Write)
![[4CEE41C3-E4ED-450E-81A1-6079482083CE.jpeg]]
### String for File Name
- It includes a path to the folder where the file resides if it is not in the current folder.
- The path is a string
- If the path contains ``\``, use ``\\`` because ``\`` is an escape symbol in the string and have special meaning when combine with the following character, e.g. ``\n``
- Path ```H:\matlab\data.mat``` should be ``` ‘H:\\matlab\\data.mat’ ```
- In the later MATLAB versions, it accepts ``` ‘H:\matlab\data.mat’ ``` as full filename
## 11.3 An Introduction to MATLAB File Processing
- Using the ==fopen== to obtain **file id** (also known as *fid*) which is a number assigned, and is used for all reading, writing, and control operations on that file
- Data can be written to and read from files in two possible ways: as binary data or as formatted character data
- File id’s are detached from the file using the ==fclose== statement
## 11.4 File Opening and Closing
- The ==fopen== functions opens a file and returns a file id number for use with the file. The most general form of this statement is:
```
fid = fopen(filename, permission)
[fid, message] = fopen(filename, permission)
[fid, message] = fopen(filename, permission, format

```
- *filename* is a string specifiying the name of the file to open and *permission* is a character string specifying the mode in which the file is opened.
- If the opening is successful, **fid** will contain a positive integer and **message** will be an empty string
### File Permission for fopen
![[1293195C-3682-435E-A457-01CD5AFB7044.jpeg]]
### Format string for fopen
![[D9F670A2-5937-4888-A7CE-E8BA62A8E511.jpeg]]
### More on File Opening and Closing
- The ==fclose== function closes a file.
```
status = fclose(fid) or status = fclose(‘all’)
```
- **fid** is a file id and **status** is the result of the operation. If the operation is successful, **status** will be 0, and if it is unsuccessful, **status** will be -1
- `status = fclose(‘all’)` closes all open files except for `stdout(fid = 1) and stderr(fid = 2)`
## 11.5 Binary I/O Function `fwrite`
- The ==fwrite== function writes binary data in a user-specified format to a file. Its form is:
```
count = fwrite(fid, array, precision)
```
- **array** is the array of values to write out, and **count** is the number of values written to the file
- MATLAB writes out data in ==column order==, which means that the entire first column is written out, followed by the entire second column, and so forth
### Precision Strings for `fwrite`
![[B1322D49-30D0-40D5-BD16-23E8BF584D93.jpeg]]
### Binary I/O Function `fread`
- The ==fread== function reads binary data in a user-specified format from a file, and returns the data in a (possibly different) user-specified format. It’s form is:
```
[array, count] = fread(fid, size, precision)
```
- The optional argument **size** specifies  the amount of data to be read from the file
- ==fread== will pad the last byte of element with zero bits if it reach the end of the file and does not find enough bits form a complete array element of the specified precision
### Double Precision Floating Point Format
