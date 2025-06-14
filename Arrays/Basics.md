# Array
Way to access multiple variable/data with a single name. 
```c
int array[] = {};
```

way to initialize values of array(s) in c:
1. Just declare an array with giving it values  but have to give length.

```c  
int array[10];
```

2. without giving it length. Compiler will determine the length of array based on number of elements.
```c
int array[] = {21,2,456,6,7};
```

3. When length of array is so large but we only want to initalize some specific values at specific places:
```c
int array[] = {[10] = 20 };
```
**This method has some side effect tho**

