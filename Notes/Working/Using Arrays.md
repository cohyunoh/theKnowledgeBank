# Using Arrays
---
- Call a **single value** from an array:
	`Array=zeros(4,3);`
	`Array(2,3)=7;`

|    |    |    |
| -- | -- | -- |
| 0  | 0  | 0  |
| 0  | 0  | **7**  |
| 0  | 0  | 0  |
| 0  | 0  | 0  |

- Call **all values** from a row/column:
	`Array2=zeros(4,3);`
	`Array2=(:,3)=12;`

|    |    |    |
| -- | -- | -- |
| 0  | 0  | **12**  |
| 0  | 0  | **12**  |
| 0  | 0  | **12**  |
| 0  | 0  | **12**  |
