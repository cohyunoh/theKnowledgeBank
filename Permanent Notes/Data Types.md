# Data Types
---
| Type              | Memory (bytes) | Range                              | Notes                                                                                             |
| ----------------- | -------------- | ---------------------------------- | ------------------------------------------------------------------------------------------------- |
| **boolean**       | 1              | *true or false (0 or 1)*           |                                                                                                   |
| **char**          | 1              | *-128 to +128*                     | Used to represent an ASCII character code                                                         |
| **byte**          | 1              | *0 to 255*                         | Used for communicating serial data, as a single unit of data                                      |
| **int**           | 2              | *-32768 to +32767*                 |                                                                                                   |
| **unsigned int**  | 2              | *0 to 65536*                       | Can be used for extra precision where negative numbers are not needed                             |
| **long**          | 4              | *-2,147,483,648 to +2,147,483.647* | Needed for only representing really big numbers                                                   |
| **unsigned long** | 4              | *0 to 4,294,967,295*               | Same purpose as **unsigned int**                                                                  |
| **float**         | 4              | *-3.4028235E+38 to +3.4028235E+38* |                                                                                                   |
| **double**        | 4              | Same as **float**                  | Normally this would be 8 bytes and higher precision than **float**. But on Arduino it is the same |