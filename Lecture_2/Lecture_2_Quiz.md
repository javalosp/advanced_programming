# Advanced Programming with C++
## Quiz: C++ Expressions, Operators, Declarations & Definitions

---

#### Which of the following statements is true regarding operator precedence in C++?**
- [ ] a). `a * b + c / d` means `a * (b + c) / d`
- [x] b). `a * b + c / d` means `(a * b) + (c / d)`
- [ ] c). `a * b + c / d` means `a * (b + c / d)`
- [ ] d). `a * b + c / d` means `(a * b + c) / d`

#### What will be the value of x after running the following code snippet?

```cpp
int x = 5;
x += 10;
```

- [ ] a). 5
- [ ] b). 10
- [x] c). 15
- [ ] d). 20

#### What will be the output of the following code snippet?

```cpp
int x = 10;
int y = 20;
int z = (x > y) ? x : y;
cout << z;
```

- [ ] a). 10
- [x] b). 20
- [ ] c). 30
- [ ] d). 0

#### What does the concise operator `a += c` mean in C++?
- [x] a). `a = a + c`
- [ ] b). `a = a - c`
- [ ] c). `a = a * c`
- [ ] d). `a = a / c`

#### Which of the following is a logical operator in C++?
- [ ] a). `==`
- [ ] b). `!=`
- [x] c). `&&`
- [ ] d). `<`

#### What is the difference between `++i` and `i++`?

- [x] a). `++i` increments `i` before its value is used, while `i++` increments `i` after its value is used.
- [ ] b). `++i` increments `i` after its value is used, while `i++` increments `i` before its value is used.
- [ ] c). There is no difference.
- [ ] d). Both are syntax errors in C++.

#### Which of the following is a valid C++ statement for declaring a double variable `d2` and initialising it to 2.5?
- [ ] a). `double 2.5 = d2;`
- [x] b). `double d2 = 2.5;`
- [ ] c). `d2 = double 2.5;`
- [ ] d). `2.5 = double d2;`

#### Which of the following is the correct syntax for a for loop in C++?

- [ ] a). `for (int i; i < 10; i++) {}`
- [x] b). `for (int i = 0; i < 10; i++) {}`
- [ ] c). `for (i = 0; i < 10; i++) {}`
- [ ] d). `for int i = 0; i < 10; i++ {}`

#### Which of the following is not a valid control flow statement?

- [ ] a). `if`
- [ ] b). `while`
- [ ] c). `switch`
- [x] d). `execute`

#### Which statement is used to terminate a loop early?

- [ ] a). `continue`
- [x] b). `break`
- [ ] c). `exit`
- [ ] d). `return`

#### What is the output of the following C++ code snippet?

```cpp
for (int i = 0; i < 3; ++i) {
    cout << i << " ";
}
```
- [x] a). 0 1 2 
- [ ] b). 1 2 3 
- [ ] c). 0 1 2 3 
- [ ] d). 1 2 

#### How many times will the following loop execute?

```cpp
for (int i = 0; i < 5; i++) {
    cout << i;
}
```

- [ ] a). 4
- [x] b). 5
- [ ] c). 6
- [ ] d). 0

#### Which loop is guaranteed to execute at least once?

- [ ] a). for loop
- [ ] b). while loop
- [x] c). do-while loop
- [ ] d). None of the above

#### What does the continue statement do in a loop?

- [ ] a). Stops the loop and exits.
- [x] b). Skips the rest of the loop iteration and starts the next iteration.
- [ ] c). Causes a syntax error.
- [ ] d). Skips to the end of the program.

#### Which of the following is a valid way to declare a function in C++?

- [ ] a). `void myFunction();`
- [ ] b). `int myFunction(int a);`
- [ ] c). `float myFunction(int a, float b);`
- [x] d). All of the above

#### Which of the following is a correct function definition in C++?

- [x] a). `int max(int a, int b) { if (a < b) return b; else return a; }`
- [ ] b). `int max(int a, int b);`
- [ ] c). `int max(a, b);`
- [ ] d). `max(int a, int b);`

#### What is the purpose of the return statement in a function?

- [x] a). To terminate the function and return control to the calling function.
- [ ] b). To pass control to another function.
- [ ] c). To exit the program.
- [ ] d). To print a value to the console.

#### What is a pure virtual function in C++?

- [x] a). A function that is declared but not defined in the base class.
- [ ] b). A function that is both declared and defined in the base class.
- [ ] c). A function that is declared with the keyword virtual.
- [ ] d). None of the above.

#### What will be the value of max after executing the following code?**

```cpp
int a = 10, b = 20, max;
if (a < b) 
    max = b;
else 
    max = a;
```
- [ ] a). 10
- [x] b). 20
- [ ] c). 0
- [ ] d). 30

#### Which keyword is used to prevent a variable from being modified?

- [x] a). `const`
- [ ] b). `static`
- [ ] c). `volatile`
- [ ] d). `mutable`

#### Which keyword is used to create a block of code that might throw an exception?

- [ ] a). `catch`
- [ ] b). `throw`
- [x] c). `try`
- [ ] d). `finally`

#### Which of the following is not a built-in data type in C++?

- [ ] a). `int`
- [ ] b). `float`
- [ ] c). `char`
- [x] d). `vector`

### What is the size of a short integer typically?

- [ ] a). 1 byte
- [x] b). 2 bytes
- [ ] c). 4 bytes
- [ ] d). 8 bytes

#### Which of the following is not a valid C++ data type?

- [ ] a). `int`
- [ ] b). `float`
- [x] c). `real`
- [ ] d). `char`

#### Which of the following types is used to store a large range of floating-point numbers?

- [ ] a). `int`
- [ ] b). `char`
- [x] c). `double`
- [ ] d). `bool`

#### What is the size of a double data type in C++?

- [ ] a). 2 bytes
- [ ] b). 4 bytes
- [x] c). 8 bytes
- [ ] d). 10 bytes

#### Which of the following correctly declares an array of 5 integers?

- [x] a). `int arr[5];`
- [ ] b). `int arr[] = {5};`
- [ ] c). `int arr(5);`
- [ ] d). `int arr = {5};`

#### Which of the following is a declaration but not a definition?

- [ ] a). `int a = 7;`
- [ ] b). `int b;`
- [x] c). `extern int c;`
- [ ] d). `double d = 3.14;`

#### Which keyword is used to declare an enumeration?

- [x] a). `enum`
- [ ] b). `enumerate`
- [ ] c). `enumtype`
- [ ] d). `enumclass`

#### Which keyword is used to define a macro in C++?

- [ ] a). `macro`
- [x] b). `#define`
- [ ] c). `#macro`
- [ ] d). `define`

#### Which of the following scopes allows a variable to be accessed globally throughout the program?

- [ ] a). Local scope
- [ ] b). Class scope
- [x] c). Global scope
- [ ] d). Statement scope

#### What will be the output of the following code snippet?

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
- [x] d). 20 10

#### In which scope does a variable declared inside a function exist?

- [ ] a). Global scope
- [x] b). Local scope
- [ ] c). Block scope
- [ ] d). Namespace scope

#### Which of the following is true about a static variable inside a function?

- [ ] a). Retains its value between function calls.
- [ ] b). Can be accessed only inside the function.
- [x] c). Both A and B.
- [ ] d). None of the above.

#### What is the scope of a variable declared outside of any function?

- [x] a). Global
- [ ] b). Local
- [ ] c). Block
- [ ] d). None

#### What is the purpose of using namespaces in C++?

- [ ] a). To define a new data type
- [x] b). To avoid name conflicts
- [ ] c). To allocate memory dynamically
- [ ] d). To define constants

#### Which of the following is true about a namespace?

- [x] a). It allows for the grouping of identifiers to avoid name conflicts.
- [ ] b). It provides a way to organise code only in header files.
- [ ] c). It must be defined within a function.
- [ ] d). It cannot be nested.

#### Which of the following correctly uses the std namespace to print a message?

- [ ] a). `std::cout << "Hello, World!";`
- [ ] b). `cout << "Hello, World!";`
- [ ] c). `using namespace std; cout << "Hello, World!";`
- [x] d). Both A and C

#### What is the purpose of the #include directive in C++?

- [x] a). To include standard or user-defined header files.
- [ ] b). To define a new function.
- [ ] c). To start a loop.
- [ ] d). To terminate a loop.

---
