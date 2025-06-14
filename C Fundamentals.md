
## 1. Compiling Prodcedure

-  **Preprocessor** :  The Preprocessor first edit and makes modification to our C program based on the given instructions. (Compile time modification)

- **Compiling** :  The real compiling starts after the proprocessing is done and our C program file turns into object file.

- **Linking** : After the production of object code, it is then linked with nescessary files (one of examples can be for printing and scanning stuff which is achived with help of underlying OS ).
## 2. Structure of C program

```c
directives

int main(){
	declarationa
	statements
}
```

**Directives** :
1. Are preprocessor which are ~~always~~ on top. Based on program requirements they can be anywhere in the program.
2. Begin with `#` character
3. Are always one line long


**`int main(){}`** This is entry point of the program 

**Declarations** :
1. Related to variables
2. In C89 Declarations must come before Statements but there is no such constraint in C99.

**Statements** :
1. They can be many lines long seperated by a `,`.
2. To end a statement `;` is used.
3. Statements contain logic of the program

## Variables

Every program needs to store data for the time of execution of program. The said data is stored in variables. 

### Steps to declare a variable :
```c
type variable_name = value;
```

1. **Type** : The form of data to be stored (eg. int, float)
2. **Variable_name** : Given by Programmer to access the data later on. It is also called Identifier.
3. **Value** : Assign the data to variable name.

- **More on the BASIC TYPES Chapter**

## Keywords
Words which do some process in C and cannot be assigned as identifiers.

## Tokens
Group of Character which cannot be broken down further without changing their meaning. 
Space can be given between tokens for readability of programs.

```c
inta=4;
```
This piece of code has 5 Identifiers namely:
1. int 
2. a
3. =
4. 4
5. ;

The given code can be modifed as:
```c
int a = 4;
```

