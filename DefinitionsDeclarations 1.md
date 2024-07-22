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