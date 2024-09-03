# Quiz: C++ Basic Structure, Declarations & Definitions
## Programming with C++


## Expressions

1. **What is the result of the following C++ expression: `int area = length * width;`, given `length = 20` and `width = 40`?**
- [ ] a). 60
- [ ] b). 800
- [ ] c). 100
- [ ] d). 400

2. **Which of the following statements is true regarding operator precedence in C++?**
- [ ] a). `a * b + c / d` means `a * (b + c) / d`
- [ ] b). `a * b + c / d` means `(a * b) + (c / d)`
- [ ] c). `a * b + c / d` means `a * (b + c / d)`
- [ ] d). `a * b + c / d` means `(a * b + c) / d`

## Operators

3. **What does the concise operator `a += c` mean in C++?**
- [ ] a). `a = a + c`
- [ ] b). `a = a - c`
- [ ] c). `a = a * c`
- [ ] d). `a = a / c`

4. **Which of the following is a logical operator in C++?**
- [ ] a). `==`
- [ ] b). `!=`
- [ ] c). `&&`
- [ ] d). `<`

## Statements

5. **Which of the following is a valid C++ statement for declaring a double variable `d2` and initializing it to 2.5?**
- [ ] a). `double 2.5 = d2;`
- [ ] b). `double d2 = 2.5;`
- [ ] c). `d2 = double 2.5;`
- [ ] d). `2.5 = double d2;`

## Iteration (Loops)

6. **What is the output of the following C++ code snippet?**
```cpp
for (int i = 0; i < 3; ++i) {
    cout << i << " ";
}
```
- [ ] a). 0 1 2 
- [ ] b). 1 2 3 
- [ ] c). 0 1 2 3 
- [ ] d). 1 2 

7. **Identify the loop variable in the following while loop:**

```cpp
int i = 0;
while (i < 100) {
    cout << i << '\t' << square(i) << '\n';
    ++i;
}
```
- [ ] a). cout
- [ ] b). i
- [ ] c). square
- [ ] d). '\t'

## Functions

8. **What does the following function return when called with square(5)?**

```cpp
int square(int x) {
    return x * x;
}
```
- [ ] a). 10
- [ ] b). 15
- [ ] c). 25
- [ ] d). 5

9. **Which of the following is a correct function declaration in C++?**

- [ ] a). int max(int a, int b) { if (a < b) return b; else return a; }
- [ ] b). int max(int a, int b);
- [ ] c). int max(a, b);
- [ ] d). max(int a, int b);

## Control Flow

10. **What will be the value of max after executing the following code?**

```cpp
int a = 10, b = 20, max;
if (a < b) 
    max = b;
else 
    max = a;
```
- [ ] a). 10
- [ ] b). 20
- [ ] c). 0
- [ ] d). 30

## Data Types

11. **Which of the following is not a built-in data type in C++?**

- [ ] a). int
- [ ] b). float
- [ ] c). char
- [ ] d). vector

12. **What is the size of a short integer typically?**

- [ ] a). 1 byte
- [ ] b). 2 bytes
- [ ] c). 4 bytes
- [ ] d). 8 bytes

## Declarations & Definitions

13. **What is wrong with the following code snippet?**

```cpp
int a;
int a;
```
- [ ] a). Nothing is wrong.
- [ ] b). Double declaration.
- [ ] c). Double definition.
- [ ] d). Missing semicolon.

14. **Which of the following is a declaration but not a definition?**

- [ ] a). int a = 7;
- [ ] b). int b;
- [ ] c). extern int c;
- [ ] d). double d = 3.14;

## Scope

15. **Which of the following scopes allows a variable to be accessed globally throughout the program?**

- [ ] a). Local scope
- [ ] b). Class scope
- [ ] c). Global scope
- [ ] d). Statement scope

16. **What will be the output of the following code snippet?**

```cpp
int x = 10;
{
    int x = 20;
    cout << x << " ";
}
cout << x;
```
- [ ] a). 10 10
- [ ] b). 20 20
- [ ] c). 10 20
- [ ] d). 20 10

## Namespaces

17. **Which of the following correctly uses the std namespace to print a message?**

- [ ] a). std::cout << "Hello, World!";
- [ ] b). cout << "Hello, World!";
- [ ] c). using namespace std; cout << "Hello, World!";
- [ ] d). Both A and C

18. **What is the purpose of using namespaces in C++?**

- [ ] a). To define a new data type
- [ ] b). To avoid name conflicts
- [ ] c). To allocate memory dynamically
- [ ] d). To define constants


---

## Answers

1. b) 800
2. b) `(a * b) + (c / d)`
3. a) `a = a + c`
4. c) `&&`
5. b) `double d2 = 2.5;`
6. a) 0 1 2 
7. b) i
8. c) 25
9. b) int max(int a, int b);
10. b) 20
11. d) vector
12. b) 2 bytes
13. c) Double definition.
14. c) extern int c;
15. c) Global scope
16. d) 20 10
17. d) Both A and C
18. b) To avoid name conflicts




# Advanced Programming in C++ - Quiz

## Instructions
- Answer the following questions to the best of your ability.
- Each section is focused on a specific topic from the lecture.
- Select the correct answer for each question.
- Correct answers are provided at the end of the quiz.

---

## Section 1: Expressions

### 1. What is the result of the following expression?

```cpp
int x = 10;
int y = 5;
int z = x + y * 2;
```

- [ ] a). 15
- [ ] b). 20
- [ ] c). 10
- [ ] d). 30

2. What is the value of x after the following code executes?

```cpp
int x = 5;
x += 10;
```

- [ ] a). 5
- [ ] b). 10
- [ ] c). 15
- [ ] d). 20

3. What will be the output of the following code?

```cpp
int x = 10;
int y = 20;
int z = (x > y) ? x : y;
cout << z;
```

- [ ] a). 10
- [ ] b). 20
- [ ] c). 30
- [ ] d). 0

Section 2: Operators
4. What is the difference between ++i and i++?

- [ ] a). ++i increments i before its value is used, while i++ increments i after its value is used.
- [ ] b). ++i increments i after its value is used, while i++ increments i before its value is used.
- [ ] c). There is no difference.
- [ ] d). Both are syntax errors in C++.

5. Which operator is used to access the members of a structure through a pointer?

- [ ] a). *
- [ ] b). .
- [ ] c). ->
- [ ] d). &

6. Which of the following is a logical operator in C++?

- [ ] a). +
- [ ] b). &&
- [ ] c). ++
- [ ] d). <<

7. What is the scope resolution operator in C++?

- [ ] a). :
- [ ] b). ::
- [ ] c). .
- [ ] d). ->

Section 3: Statements
8. Which of the following is the correct syntax for a for loop in C++?

- [ ] a). for (int i; i < 10; i++) {}
- [ ] b). for (int i = 0; i < 10; i++) {}
- [ ] c). for (i = 0; i < 10; i++) {}
- [ ] d). for int i = 0; i < 10; i++ {}

9. Which of the following is not a valid control flow statement?

- [ ] a). if
- [ ] b). while
- [ ] c). switch
- [ ] d). execute

10. Which statement is used to terminate a loop early?

- [ ] a). continue
- [ ] b). break
- [ ] c). exit
- [ ] d). return

Section 4: Iteration (Loops)
11. How many times will the following loop execute?

```cpp
for (int i = 0; i < 5; i++) {
    cout << i;
}
```

- [ ] a). 4
- [ ] b). 5
- [ ] c). 6
- [ ] d). 0

12. Which loop is guaranteed to execute at least once?

- [ ] a). for loop
- [ ] b). while loop
- [ ] c). do-while loop
- [ ] d). None of the above

13. What does the continue statement do in a loop?

- [ ] a). Stops the loop and exits.
- [ ] b). Skips the rest of the loop iteration and starts the next iteration.
- [ ] c). Causes a syntax error.
- [ ] d). Skips to the end of the program.

Section 5: Functions
14. Which of the following is a valid way to declare a function in C++?

- [ ] a). void myFunction();
- [ ] b). int myFunction(int a);
- [ ] c). float myFunction(int a, float b);
- [ ] d). All of the above

15. What is the purpose of the return statement in a function?

- [ ] a). To terminate the function and return control to the calling function.
- [ ] b). To pass control to another function.
- [ ] c). To exit the program.
- [ ] d). To print a value to the console.

16. What is a pure virtual function in C++?

- [ ] a). A function that is declared but not defined in the base class.
- [ ] b). A function that is both declared and defined in the base class.
- [ ] c). A function that is declared with the keyword virtual.
- [ ] d). None of the above.

17. What does the this pointer refer to in a class?

- [ ] a). The address of the current object.
- [ ] b). The address of the base class.
- [ ] c). The address of the derived class.
- [ ] d). None of the above.

Section 6: Control Flow
18. What will be the output of the following code?

```cpp
int a = 10;
int b = 20;
if (a == b)
    cout << "Equal";
else
    cout << "Not equal";
```

- [ ] a). Equal
- [ ] b). Not equal
- [ ] c). No output
- [ ] d). Compilation error

19. Which keyword is used to prevent a variable from being modified?

- [ ] a). const
- [ ] b). static
- [ ] c). volatile
- [ ] d). mutable

20. Which keyword is used to create a block of code that might throw an exception?

- [ ] a). catch
- [ ] b). throw
- [ ] c). try
- [ ] d). finally

Section 7: Data Types
21. Which of the following is NOT a valid C++ data type?

- [ ] a). int
- [ ] b). float
- [ ] c). real
- [ ] d). char

22. Which of the following types is used to store a large range of floating-point numbers?

- [ ] a). int
- [ ] b). char
- [ ] c). double
- [ ] d). bool

23. What is the size of a double data type in C++?

- [ ] a). 2 bytes
- [ ] b). 4 bytes
- [ ] c). 8 bytes
- [ ] d). 10 bytes

24. Which of the following correctly declares an array of 5 integers?

- [ ] a). int arr[5];
- [ ] b). int arr[] = {5};
- [ ] c). int arr(5);
- [ ] d). int arr = {5};

Section 8: Declarations & Definitions
25. Which of the following correctly declares a pointer to an integer?

- [ ] a). int *ptr;
- [ ] b). int ptr;
- [ ] c). int &ptr;
- [ ] d). pointer int *ptr;

26. Which of the following is a correct declaration of a reference variable?

- [ ] a). int &ref = a;
- [ ] b). int ref = &a;
- [ ] c). int *ref = &a;
- [ ] d). int ref = a;

27. Which keyword is used to declare an enumeration?

- [ ] a). enum
- [ ] b). enumerate
- [ ] c). enumtype
- [ ] d). enumclass

28. Which keyword is used to define a macro in C++?

- [ ] a). macro
- [ ] b). #define
- [ ] c). #macro
- [ ] d). define

Section 9: Scope
29. In which scope does a variable declared inside a function exist?

- [ ] a). Global scope
- [ ] b). Local scope
- [ ] c). Block scope
- [ ] d). Namespace scope

30. Which of the following is true about a static variable inside a function?

- [ ] a). Retains its value between function calls.
- [ ] b). Can be accessed only inside the function.
- [ ] c). Both A and B.
- [ ] d). None of the above.

31. What is the scope of a variable declared outside of any function?

- [ ] a). Global
- [ ] b). Local
- [ ] c). Block
- [ ] d). None

Section 10: Namespace
32. Which of the following is true about a namespace?

- [ ] a). It allows for the grouping of identifiers to avoid name conflicts.
- [ ] b). It provides a way to organize code only in header files.
- [ ] c). It must be defined within a function.
- [ ] d). It cannot be nested.

33. Which of the following is not a valid namespace?

- [ ] a). std
- [ ] b). boost
- [ ] c). global
- [ ] d). mynamespace

34. What is the purpose of the #include directive in C++?

- [ ] a). To include standard or user-defined header files.
- [ ] b). To define a new function.
- [ ] c). To start a loop.
- [ ] d). To terminate a loop.

Answers

    b). 20
    c). 15
    b). 20
    a). ++i increments i before its value is used, while i++ increments i after its value is used.
    c). ->
    b). &&
    b). ::
    b). for (int i = 0; i < 10; i++) {}
    d). execute
    b). break
    b). 5
    c). do-while loop
    b). Skips the rest of the loop iteration and starts the next iteration.
    d). All of the above
    a). To terminate the function and return control to the calling function.
    a). A function that is declared but not defined in the base class.
    a). The address of the current object.
    b). Not equal
    a). const
    c). try
    c). real
    c). double
    c). 8 bytes
    a). int arr[5];
    a). int *ptr;
    a). int &ref = a;
    a). enum
    b). #define
    b). Local scope
    c). Both A and B.
    a). Global
    a). It allows for the grouping of identifiers to avoid name conflicts.
    c). global
    a). To include standard or user-defined header files.

End of Quiz