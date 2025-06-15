# Output

Output to the console is mainly done with library functions of `stdio.h`. 
`printf()` and `puts()` are such functions.


## Printf
`printf()` stands for print formatted. It is called so beacause it formats the given string (character array) according to format specifications. 

```c
int x = 5;
float y = 19.9f
printf("value of x is: %d\n value of y is: %f\n",x,y);
```

As said printf will modify the given string where it encouters `%` character followed by format specificatior. First one is `%d` which tells to print a integer value while the second one `%f` tells to print floating point ( decimal ) value.

>[!NOTE]
>To print single `%`  specify double `%%` in the String.

>[!NOTE]
>Sequence of arguements after the format string must match to display text properly.

>[!WARNING]
>C compiler has no obligation to check that number of format specifiers  match the given number of arguemnets

### Format Specifiers

character like `%X` where X stands for different data types are format specifiers. 
More precisely every format specifier is in form of `%m.pX` or `%-m.pX` 

1. **Minimum Field Width (m)**: This specifies minimum number of characters to print, if data has less characters as compared to its value, space are added, which by default is right justified, left justified with negative number `%-m.pX` 

```c
int x = 123;
printf("x = %4d\n",x);
```
Output : `⚪123` (using white dot to represent white space)
for `printf("x = %-4d\n",x);` output will be `123⚪`


2. **Precision (p)**: This has different effect for different data types.

| Data Type      | Effect                                                                                                                                              |
| -------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| `int` (`d`)    | Dictates the number of digits to display. Extra space is supplemented by zeros instead of spaces.                                                   |
| `float`  (`e`) | `e` displays floating point number is expotential form. `p` dictates how many digits should appear after decimal point.<br>`printf("%.1e", 12.34);` |
| `float` (`f`)  | `p` has same effect as mentioned in above                                                                                                           |
| `float (g)`    | Displays a floating point number in either exponential format or fixed decimal format. `p` diplays **maximum number of significant digit**          |
