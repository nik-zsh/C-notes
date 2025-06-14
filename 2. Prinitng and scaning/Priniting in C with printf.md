printing information in C is mainly done via `printf()` function. ( Mind it when I say **mainly** as some data types has their own prinitng functions but that is used like 0.0001% of time. )
### syntax
```c
printf(string,arg1,arg2,arg3,....);
```

You basically give it a string and **specify** places where you want to insert the variables  with help of **conversion specification**.
### Example:
```c
#include <stdio.h>

int main(){
int x = 5;
printf("Value of x is: %d\n",x);
}
```

to specify which type of variable will come at a given place `%` character is used followed with type of variable. For integer being `%d`.  ( And to print a single `%` character you need to insert `%%` in string. )