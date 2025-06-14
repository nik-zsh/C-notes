Similar to `printf()` `scanf()` scans the input in specific format. 
scanf stand for *scan formatted*. 


## Format

`scanf(string, arg1,arg2,....)`

```c
int variable_name;
scanf("%d", &variable_name);
```

### Code Explanation:
whatever you input in the terminal goes in form of string. 
The string in scanf is needed beacause we are telling scanf() function the format of input string and what values to specially pick from that string and put it in the variables needed. 
**scanf() is dumb that is the reason we need to tell what string will be given in terminal**
# Warning(s)
+ string placement in scanf is often error prone for new users. 
+ Notice the `&` used before variable name. For now just remember we need it to get input.
+ scanf cannot digest spaces within input ( you will know later~ )
+ Always see that the string which you passed is as needed, as most probably you would give a space in format string like `"%d %d"` and this could affect the program. **( For now you might think this is hectic but belive me this will all make sense later on~ )**

### Advanced Examples:
```c
#include <stdio.h>

int main(){
	int var1, var2;
	printf("Enter the value for varibles var1: "):
	scanf("%d", &var1);
	printf("Enter the value for varibles var2: "):
	scanf("%d", &var2);
	printf("value of var1 is %d and var2 is %d\n", var1, var2);
	return 0;	
}
```

Okay so this seems cute enough but this can be modified as:
```c
printf("Enter the value of var1 and var2: ");
scanf("%d%d",&var1,&var2);
```

And you can enter the two values just seperate them with space. As said previously `scanf()` cannot digest space therefore it will just enter the value present there before it encountered the space to variable and move to next character in string. 