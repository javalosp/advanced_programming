# Quiz: Memory management: Pointers
## Programming with C++

---

Pointers Quiz
1. What is a pointer in C++?
- [ ] a). A type of variable that stores a memory address
- [ ] b). A variable that stores an integer
- [ ] c). A function that returns a memory address
- [ ] d). None of the above

2. How do you declare a pointer to an integer in C++?
- [ ] a). int &ptr;
- [ ] b). int *ptr;
- [ ] c). int ptr*;
- [ ] d). int ptr&;

3. What does the & operator do in the context of pointers?
- [ ] a). Dereferences a pointer
- [ ] b). Allocates memory dynamically
- [ ] c). Returns the memory address of a variable
- [ ] d). None of the above

4. What will be the output of the following code?

```cpp
int a = 10;
int *p = &a;
*p = 20;
std::cout << a;
```
- [ ] a). 10
- [ ] b). 20
- [ ] c). 0
- [ ] d). Compilation error

5. In which memory area are dynamically allocated variables stored?
- [ ] a). Stack
- [ ] b). Heap
- [ ] c). Global
- [ ] d). Register

6. How do you deallocate memory that was allocated using new?
- [ ] a). free
- [ ] b). delete
- [ ] c). remove
- [ ] d). clear

7. What would be the correct way to allocate memory for an array of 10 integers using pointers?
- [ ] a). int *arr = new int[10];
- [ ] b). int *arr = malloc(10 * sizeof(int));
- [ ] c). int arr[10];
- [ ] d). int arr = new int;

8. What happens when you try to access memory that has not been allocated to your program?
- [ ] a). The program continues normally
- [ ] b). The program may crash or behave unpredictably
- [ ] c). The program automatically allocates the necessary memory
- [ ] d). None of the above

9. Consider the following code:

```cpp
int a = 5;
int *p = &a;
int **pp = &p;
**pp = 10;
std::cout << a;
```
What will be the output?
- [ ] a). 5
- [ ] b). 10
- [ ] c). 0
- [ ] d). Compilation error

10. What is a potential issue with using pointers and dynamic memory allocation?
- [ ] a). Memory leaks
- [ ] b). Stack overflow
- [ ] c). Syntax errors
- [ ] d). None of the above

---

## Answers
1. a) A type of variable that stores a memory address
2. b) int *ptr;
3. c) Returns the memory address of a variable
4. b) 20
5. b) Heap
6. b) delete
7. a) int *arr = new int[10];
8. b) The program may crash or behave unpredictably
9. b) 10
10. a) Memory leaks


---
---
---


1. **What is automatic memory allocation in C++?**
- [ ] a). Memory allocated on the heap during runtime.
- [ ] b). Memory allocated on the stack when a variable is declared.
- [ ] c). Memory allocated at compile time.
- [ ] d). Memory allocated with the `new` operator.

2. **Which memory allocation type requires the use of the `new` and `delete` operators in C++?**
- [ ] a). Automatic memory allocation
- [ ] b). Dynamic memory allocation
- [ ] c). Static memory allocation
- [ ] d). Compile-time memory allocation

3. **What is the default stack size on Windows?**
- [ ] a). 512 KB
- [ ] b). 1 MB
- [ ] c). 2 MB
- [ ] d). 8 MB

4. **In C++, what does the `*` operator do when used with a pointer?**
- [ ] a). Allocates memory
- [ ] b). Deallocates memory
- [ ] c). Accesses the value at the memory location
- [ ] d). Returns the pointer's address

5. **Which of the following statements correctly declares a pointer to an integer in C++?**
- [ ] a). `int p;`
- [ ] b). `int *p;`
- [ ] c). `int &p;`
- [ ] d). `int p*;`

6. **What is a stack frame?**
- [ ] a). A structure in the heap to store dynamic variables
- [ ] b). A section of the stack containing function parameters, local variables, and return address
- [ ] c). A memory block reserved for global variables
- [ ] d). A pointer to the stack

7. **What happens when a function returns in C++?**
- [ ] a). The stack frame is removed from the top of the stack.
- [ ] b). The heap memory is deallocated.
- [ ] c). The global variables are reset.
- [ ] d). The entire stack is cleared.

8. **Which of the following is true about the heap in C++?**
- [ ] a). Memory is automatically managed by the runtime environment.
- [ ] b). Memory allocation and deallocation are performed in a Last-In-First-Out manner.
- [ ] c). Memory blocks can be allocated and deallocated in any order.
- [ ] d). The memory size is fixed and cannot be resized.

9. **What is a memory leak in C++?**
- [ ] a). When memory is allocated but not deallocated.
- [ ] b). When memory is deallocated before it is used.
- [ ] c). When memory is allocated on the stack.
- [ ] d). When memory is allocated at compile time.

10. **Which of the following code snippets correctly allocates memory for an array of 20 integers?**
- [ ] a). `int *P = new int;`
- [ ] b). `int P[20];`
- [ ] c). `int *P = new int[20];`
- [ ] d). `int *P = malloc(20 * sizeof(int));`

11. **Given the code `int a = 10; int *b = &a; *b = 20;`, what is the value of `a` after execution?**
- [ ] a). 10
- [ ] b). 20
- [ ] c). Null
- [ ] d). Uninitialized

12. **What does the following code do?**
```cpp
int **c = &b;
**c = 30;
```
- [ ] a). Changes the value of b to 30.
- [ ] b). Changes the value of a to 30.
- [ ] c). Declares a pointer to a pointer of type int.
- [ ] d). Causes a compilation error.

13. **In a 32-bit system, how much memory does a pointer typically occupy?**

- [ ] a). 2 bytes
- [ ] b). 4 bytes
- [ ] c). 8 bytes
- [ ] d). 16 bytes

14. **What is the equivalent pointer notation for an array A[10]?**

- [ ] a). A
- [ ] b). &A
- [ ] c). A[0]
- [ ] d). &A[0]

15. **Which of the following correctly declares and initializes an array of 6 integers?**

- [ ] a). int x[6] = {19, 10, 8, 17, 9, 15};
- [ ] b). int x = {19, 10, 8, 17, 9, 15};
- [ ] c). int x[6] = {19, 10, 8};
- [ ] d). int x[6];

16. **What is the primary advantage of using std::vector over arrays in C++?**

- [ ] a). They are faster.
- [ ] b). They avoid buffer overflows.
- [ ] c). They cannot be resized.
- [ ] d). They use less memory.

17. **How is memory de-allocated for a dynamically allocated array in C++?**

- [ ] a). delete P;
- [ ] b). free(P);
- [ ] c). delete[] P;
- [ ] d). dealloc(P);

18. **What does the following code print?**

```cpp
int a[5] = {1, 2, 3, 4, 5};
int *p = a;
p += 2;
std::cout << *p << std::endl;
```
- [ ] a). 1
- [ ] b). 2
- [ ] c). 3
- [ ] d). 4

19. **What is the correct way to define a pointer to a pointer to a double?**

- [ ] a). double **P;
- [ ] b). double *P*;
- [ ] c). double &P;
- [ ] d). double *P;

20. **Which memory allocation method is considered to be more of a C method rather than C++?**

- [ ] a). new
- [ ] b). delete
- [ ] c). malloc
- [ ] d). free

21. **What does the following code do?**

```cpp
int *P;
P = new int;
*P = 24;
delete P;
```
- [ ] a). Allocates memory for an integer, assigns it the value 24, and then deallocates the memory.
- [ ] b). Causes a memory leak.
- [ ] c). Allocates memory for an array of integers.
- [ ] d). Allocates memory for a pointer.

22. **How is a static array stored in memory?**

- [ ] a). Heap
- [ ] b). Stack
- [ ] c). Free store
- [ ] d). Global memory

23. **What is the size limit of addressable RAM in a 32-bit program?**

- [ ] a). 2 GB
- [ ] b). 4 GB
- [ ] c). 8 GB
- [ ] d). 16 GB

24. **Which of the following statements is true about stack memory?**

- [ ] a). It can become fragmented over time.
- [ ] b). It is managed manually by the programmer.
- [ ] c). It is of a fixed size set by the operating system.
- [ ] d). It is used for dynamic memory allocation.

25. **What does the following code snippet do?**

```cpp
int *P = new int[20];
P[12] = 24;
delete[] P;
```
- [ ] a). Allocates memory for 20 integers, assigns the 13th element the value 24, and then deallocates the memory.
- [ ] b). Causes a memory leak.
- [ ] c). Allocates memory for a single integer.
- [ ] d). Allocates memory for a double.

26. **Why should arrays be avoided whenever possible in C++ programs?**

- [ ] a). They are slower than other data structures.
- [ ] b). They are the largest single source of bugs.
- [ ] c). They use more memory than other data structures.
- [ ] d). They cannot be dynamically allocated.

27. **Which operator is used to obtain the memory address of a variable in C++?**

- [ ] a). *
- [ ] b). &
- [ ] c). ->
- [ ] d). ::

28. **What happens when you perform pointer arithmetic in C++?**

- [ ] a). The pointer changes its type.
- [ ] b). The pointer moves by the size of the data type it points to.
- [ ] c). The pointer is dereferenced.
- [ ] d). The pointer is deleted.

29. **Which of the following correctly declares a pointer to an array of integers?**

- [ ] a). int **P;
- [ ] b). int *P[10];
- [ ] c). int (*P)[10];
- [ ] d). int P[10];

30. **What does the following code snippet do?**

```cpp
int x[6] = {19, 10, 8};
```
- [ ] a). Declares an array of 6 integers and initializes the first 3 elements.
- [ ] b). Declares an array of 3 integers.
- [ ] c). Causes a compilation error.
- [ ] d). Declares and initializes an array of 6 integers to zero.

31. **How can a function return more than one value using pointers in C++?**

- [ ] a). By returning an array.
- [ ] b). By passing pointers as parameters and modifying the values at those addresses.
- [ ] c). By using the return statement multiple times.
- [ ] d). By using global variables.

32. **What is the primary risk associated with dynamic memory allocation?**

- [ ] a). Stack overflow
- [ ] b). Memory fragmentation
- [ ] c). Compile-time errors
- [ ] d). Global variable conflicts

33. **What is the main difference between stack and heap memory allocation in C++?**

- [ ] a). Stack memory is managed manually, while heap memory is managed automatically.
- [ ] b). Stack memory is dynamically allocated, while heap memory is statically allocated.
- [ ] c). Stack memory is of fixed size, while heap memory can be resized.
- [ ] d). Stack memory is slower, while heap memory is faster.

34. **Which of the following is a valid way to deallocate memory allocated with malloc in C++?**

- [ ] a). free()
- [ ] b). delete
- [ ] c). delete[]
- [ ] d). dealloc()

35. **What is the correct syntax to declare a pointer to an array of 1000 integers?**

- [ ] a). int *P[1000];
- [ ] b). int (*P)[1000];
- [ ] c). int **P;
- [ ] d). int P[1000];

36. **What does the following code snippet do?**

```cpp
int a = 10;
int *b = &a;
*b = 20;
int **c = &b;
**c = 30;
```
- [ ] a). Sets a to 20 and b to 30.
- [ ] b). Sets a to 30.
- [ ] c). Sets b to 10 and c to 20.
- [ ] d). Causes a runtime error.

37. **How do you access the nth element of an array using pointer notation?**

- [ ] a). array[n]
- [ ] b). *(array + n)
- [ ] c). &array[n]
- [ ] d). array->n

38. **What is the correct way to declare a pointer to a function that takes an int and returns a double?**

- [ ] a). double (*func)(int);
- [ ] b). double (*func(int));
- [ ] c). double *func(int);
- [ ] d). double (*func) int;

39. **What does the following code do?**

```cpp
int *P;
P = new int[20];
P[12] = 24;
delete[] P;
```
- [ ] a). Allocates memory for 20 integers, assigns the 13th element the value 24, and then deallocates the memory.
- [ ] b). Causes a memory leak.
- [ ] c). Allocates memory for a single integer.
- [ ] d). Allocates memory for a double.

40. **Which of the following statements is true about pointers in C++?**

- [ ] a). Pointers are automatically deallocated at the end of the program.
- [ ] b). Pointers can be used to access array elements.
- [ ] c). Pointers cannot be incremented or decremented.
- [ ] d). Pointers are always initialized to nullptr.

41. **What is the correct way to declare a pointer to a pointer to an integer?**

- [ ] a). int **P;
- [ ] b). int *P*;
- [ ] c). int &P;
- [ ] d). int P**;

42. **What does the following code snippet print?**

```cpp
int a[5] = {1, 2, 3, 4, 5};
int *p = a;
std::cout << p[2] << std::endl;
```
- [ ] a). 1
- [ ] b). 2
- [ ] c). 3
- [ ] d). 4

43. **Which of the following correctly allocates memory for a two-dimensional array of doubles?**

- [ ] a). double **P = new double*[max_i];
- [ ] b). double P[max_i][max_j];
- [ ] c). double **P = malloc(sizeof(double) * max_i * max_j);
- [ ] d). double P = new double[max_i * max_j];

44. **What is the purpose of the delete operator in C++?**

- [ ] a). To allocate memory
- [ ] b). To deallocate memory
- [ ] c). To access the value at a pointer's memory location
- [ ] d). To return a pointer's address

45. **How can you prevent memory leaks in C++?**

- [ ] a). By using global variables
- [ ] b). By deallocating memory using delete or delete[]
- [ ] c). By avoiding pointer arithmetic
- [ ] d). By using static variables

46. **What does the following code snippet do?**

```cpp
int a = 10;
int *b = &a;
int **c = &b;
**c = 30;
```
- [ ] a). Sets a to 30.
- [ ] b). Sets b to 30.
- [ ] c). Sets c to 30.
- [ ] d). Causes a compilation error.

47. **Which of the following correctly declares a pointer to a character array?**

- [ ] a). char P[20];
- [ ] b). char *P;
- [ ] c). char **P;
- [ ] d). char P*;

48. **What does the following code snippet print?**

```cpp
int a = 10;
int *b = &a;
std::cout << *b << std::endl;
```
- [ ] a). The address of a
- [ ] b). The value of a
- [ ] c). The address of b
- [ ] d). The value of b


---

## Answers

1. b). Memory allocated on the stack when a variable is declared.
2. b). Dynamic memory allocation
3. b). 1 MB
4. c). Accesses the value at the memory location
5. b). `int *p;`
6. b). A section of the stack containing function parameters, local variables, and return address
7. a). The stack frame is removed from the top of the stack.
8. c). Memory blocks can be allocated and deallocated in any order.
9. a). When memory is allocated but not deallocated.
10. c). `int *P = new int[20];`
11. b). 20
12. b). Changes the value of a to 30.
13. b). 4 bytes
14. d). &A[0]
15. a). int x[6] = {19, 10, 8, 17, 9, 15};
16. b). They avoid buffer overflows.
17. c). delete[] P;
18. c). 3
19. a). double **P;
20. c). malloc
21. a). Allocates memory for an integer, assigns it the value 24, and then deallocates the memory.
22. b). Stack
23. b). 4 GB
24. c). It is of a fixed size set by the operating system.
25. a). Allocates memory for 20 integers, assigns the 13th element the value 24, and then deallocates the memory.
26. b). They are the largest single source of bugs.
27. b). &
28. b). The pointer moves by the size of the data type it points to.
29. c). int (*P)[10];
30. a). Declares an array of 6 integers and initializes the first 3 elements.
31. b). By passing pointers as parameters and modifying the values at those addresses.
32. b). Memory fragmentation
33. c). Stack memory is of fixed size, while heap memory can be resized.
34. a). free()
35. b). int (*P)[1000];
36. b). Sets a to 30.
37. b). *(array + n)
38. a). double (*func)(int);
39. a). Allocates memory for 20 integers, assigns the 13th element the value 24, and then deallocates the memory.
40. b). Pointers can be used to access array elements.
41. a). int **P;
42. c). 3
43. a). double **P = new double*[max_i];
44. b). To deallocate memory
45. b). By deallocating memory using delete or delete[]
46. a). Sets a to 30.
47. b). char *P;
48. b) The value of a




# Advanced Programming in C++ - Quiz: Pointers and Memory Management

## Instructions
- Answer the following questions to the best of your ability.
- Each section is focused on a specific aspect of pointers and memory management.
- Select the correct answer for each question.
- Correct answers are provided at the end of the quiz.

---

## Section 1: Pointers Basics

### 1. What is a pointer in C++?

- A) A variable that stores the memory address of another variable.
- B) A special type of integer.
- C) A function that returns the memory address of a variable.
- D) A variable that points to the next element in an array.

### 2. Which of the following correctly declares a pointer to an integer?

- A) `int *ptr;`
- B) `int ptr*;`
- C) `int &ptr;`
- D) `pointer int *ptr;`

### 3. How do you access the value stored at the memory address pointed to by a pointer?

- A) `&ptr`
- B) `*ptr`
- C) `ptr*`
- D) `ptr&`

### 4. What will the following code print?

```cpp
int x = 10;
int *ptr = &x;
cout << *ptr;
```

- [ ] a). Memory address of x
- [ ] b). 10
- [ ] c). Value of ptr
- [ ] d). Undefined

Section 2: Pointer Arithmetic
5. If ptr is a pointer to an integer, what does ptr + 1 do?

- [ ] a). Moves the pointer to the next memory address.
- [ ] b). Adds 1 to the value pointed to by ptr.
- [ ] c). Moves the pointer to the next integer.
- [ ] d). Causes a compile-time error.

6. What is the output of the following code?

```cpp
int arr[5] = {10, 20, 30, 40, 50};
int *ptr = arr;
cout << *(ptr + 2);
```

- [ ] a). 10
- [ ] b). 20
- [ ] c). 30
- [ ] d). 40

7. Given the following code, what is *(ptr + 3)?

```cpp
int arr[4] = {1, 2, 3, 4};
int *ptr = arr;
```

- [ ] a). 1
- [ ] b). 2
- [ ] c). 3
- [ ] d). 4

Section 3: Dynamic Memory Allocation
8. Which operator is used to allocate memory dynamically for an integer in C++?

- [ ] a). malloc()
- [ ] b). calloc()
- [ ] c). new
- [ ] d). allocate

9. What does the following code do?

```cpp
int *ptr = new int;
```

- [ ] a). Declares a pointer to an integer and initializes it to nullptr.
- [ ] b). Declares a pointer to an integer and allocates memory for it.
- [ ] c). Declares an integer and allocates memory for it.
- [ ] d). Declares a pointer to an integer and assigns it the value 0.

10. How do you deallocate memory allocated with new?

- [ ] a). free(ptr);
- [ ] b). delete ptr;
- [ ] c). remove(ptr);
- [ ] d). dealloc(ptr);

11. What will happen if you try to delete a pointer twice?

- [ ] a). The program will run without errors.
- [ ] b). The program will crash or exhibit undefined behavior.
- [ ] c). The memory will be freed twice.
- [ ] d). The program will delete the pointer only once.

Section 4: Pointers and Arrays
12. How do you access the third element of an array arr using a pointer ptr?

- [ ] a). ptr[3]
- [ ] b). *(ptr + 2)
- [ ] c). *(ptr + 3)
- [ ] d). *ptr + 2

13. Which of the following statements is true?

- [ ] a). Array elements are stored in non-contiguous memory locations.
- [ ] b). The name of an array acts as a pointer to its first element.
- [ ] c). Pointers and arrays cannot be used together.
- [ ] d). Pointers cannot be used to traverse an array.

14. What will be the output of the following code?

```cpp
int arr[3] = {10, 20, 30};
int *ptr = arr;
cout << ptr[1];
```

- [ ] a). 10
- [ ] b). 20
- [ ] c). 30
- [ ] d). Undefined

Section 5: Pointers and Functions
15. How do you pass a pointer to a function?

- [ ] a). function(&ptr);
- [ ] b). function(*ptr);
- [ ] c). function(ptr);
- [ ] d). function(ptr*);

16. What is the advantage of passing a pointer to a function?

- [ ] a). It allows for passing large amounts of data efficiently.
- [ ] b). It prevents the function from modifying the original data.
- [ ] c). It allows the function to return multiple values.
- [ ] d). It causes the program to run faster.

17. What will the following code print?

```cpp
void updateValue(int *ptr) {
    *ptr = 100;
}

int main() {
    int x = 10;
    updateValue(&x);
    cout << x;
}
```

- [ ] a). 10
- [ ] b). 100
- [ ] c). Memory address of x
- [ ] d). Undefined

Section 6: Memory Leaks and Best Practices
18. What is a memory leak?

- [ ] a). A situation where memory is allocated but never freed.
- [ ] b). A situation where a pointer points to an invalid memory address.
- [ ] c). A situation where memory is freed twice.
- [ ] d). A situation where memory is corrupted by a pointer.

19. Which of the following is a good practice to avoid memory leaks?

- [ ] a). Always initialize pointers to nullptr.
- [ ] b). Avoid using dynamic memory allocation.
- [ ] c). Always deallocate memory using delete or delete[].
- [ ] d). Never use pointers in your programs.

20. What does the following code do?

```cpp
int *ptr = new int[10];
// Some code
delete[] ptr;
```

- [ ] a). Allocates memory for 10 integers and then deallocates it.
- [ ] b). Causes a memory leak because only the first element is deleted.
- [ ] c). Allocates memory but does not deallocate it.
- [ ] d). Deallocates the memory and then causes a runtime error.

Answers

- [ ] a). A variable that stores the memory address of another variable.
- [ ] a). int *ptr;
- [ ] b). *ptr
- [ ] b). 10
- [ ] c). Moves the pointer to the next integer.
- [ ] c). 30
- [ ] d). 4
- [ ] c). new
- [ ] b). Declares a pointer to an integer and allocates memory for it.
- [ ] b). delete ptr;
- [ ] b). The program will crash or exhibit undefined behavior.
- [ ] b). *(ptr + 2)
- [ ] b). The name of an array acts as a pointer to its first element.
- [ ] b). 20
- [ ] c). function(ptr);
- [ ] a). It allows for passing large amounts of data efficiently.
- [ ] b). 100
- [ ] a). A situation where memory is allocated but never freed.
- [ ] c). Always deallocate memory using delete or delete[].
- [ ] a). Allocates memory for 10 integers and then deallocates it.

End of Quiz
