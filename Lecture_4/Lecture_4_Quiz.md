# Programming with C++
## Quiz: Memory management & Pointers

---

#### What is a pointer in C++?
- [x] a). A type of variable that stores a memory address
- [ ] b). A variable that stores an integer
- [ ] c). A function that returns a memory address
- [ ] d). None of the above

#### What does the & operator do in the context of pointers?
- [ ] a). Dereferences a pointer
- [ ] b). Allocates memory dynamically
- [x] c). Returns the memory address of a variable
- [ ] d). None of the above

#### What will be the output of the following code?
```cpp
int a = 10;
int *p = &a;
*p = 20;
std::cout << a;
```
- [ ] a). 10
- [x] b). 20
- [ ] c). 0
- [ ] d). Compilation error

#### What would be the correct way to allocate memory for an array of 10 integers using pointers?
- [x] a). int *arr = new int[10];
- [ ] b). int *arr = malloc(10 * sizeof(int));
- [ ] c). int arr[10];
- [ ] d). int arr = new int;

#### What happens when you try to access memory that has not been allocated to your program?
- [ ] a). The program continues normally
- [x] b). The program may crash or behave unpredictably
- [ ] c). The program automatically allocates the necessary memory
- [ ] d). None of the above

#### What will be the output of the following code snippet?
```cpp
int a = 5;
int *p = &a;
int  pp = &p;
 pp = 10;
std::cout << a;
```

- [ ] a). 5
- [x] b). 10
- [ ] c). 0
- [ ] d). Compilation error

#### What is a potential issue with using pointers and dynamic memory allocation?
- [x] a). Memory leaks
- [ ] b). Stack overflow
- [ ] c). Syntax errors
- [ ] d). None of the above

#### What is automatic memory allocation in C++?
- [ ] a). Memory allocated on the heap during runtime.
- [x] b). Memory allocated on the stack when a variable is declared.
- [ ] c). Memory allocated at compile time.
- [ ] d). Memory allocated with the `new` operator.

#### In which memory area are dynamically allocated variables stored?
- [ ] a). Stack
- [x] b). Heap
- [ ] c). Global
- [ ] d). Register

#### How do you deallocate memory that was allocated using new?
- [ ] a). `free`
- [x] b). `delete`
- [ ] c). `remove`
- [ ] d). `clear`

#### Which memory allocation type requires the use of the `new` and `delete` operators in C++?
- [ ] a). Automatic memory allocation
- [x] b). Dynamic memory allocation
- [ ] c). Static memory allocation
- [ ] d). Compile-time memory allocation

#### In C++, what does the `*` operator do when used with a pointer? 
- [ ] a). Allocates memory
- [ ] b). Deallocates memory
- [x] c). Accesses the value at the memory location
- [ ] d). Returns the pointer's address

#### Which of the following statements correctly declares a pointer to an integer in C++?
- [ ] a). `int p;`
- [x] b). `int *p;`
- [ ] c). `int &p;`
- [ ] d). `int p*;`

#### What is a stack frame?
- [ ] a). A structure in the heap to store dynamic variables
- [x] b). A section of the stack containing function parameters, local variables, and return address
- [ ] c). A memory block reserved for global variables
- [ ] d). A pointer to the stack

#### What happens when a function returns in C++?
- [x] a). The stack frame is removed from the top of the stack.
- [ ] b). The heap memory is deallocated.
- [ ] c). The global variables are reset.
- [ ] d). The entire stack is cleared.

#### Which of the following is true about the heap in C++?
- [ ] a). Memory is automatically managed by the runtime environment.
- [ ] b). Memory allocation and deallocation are performed in a Last-In-First-Out manner.
- [x] c). Memory blocks can be allocated and deallocated in any order.
- [ ] d). The memory size is fixed and cannot be resized.

#### What is a memory leak in C++?
- [x] a). When memory is allocated but not deallocated.
- [ ] b). When memory is deallocated before it is used.
- [ ] c). When memory is allocated on the stack.
- [ ] d). When memory is allocated at compile time.

#### Which of the following code snippets correctly allocates memory for an array of 20 integers?
- [ ] a). `int *P = new int;`
- [ ] b). `int P[20];`
- [x] c). `int *P = new int[20];`
- [ ] d). `int *P = malloc(20 * sizeof(int));`

#### What is the value of `a` after execution in the following code snippet?
```cpp
int a = 10;
int *b = &a;
*b = 20;
```

- [ ] a). 10
- [x] b). 20
- [ ] c). Null
- [ ] d). Uninitialized

### What does the following code do?
```cpp
int  c = &b;
 c = 30;
```
- [ ] a). Changes the value of b to 30.
- [x] b). Changes the value of a to 30.
- [ ] c). Declares a pointer to a pointer of type int.
- [ ] d). Causes a compilation error.

#### In a 32-bit system, how much memory does a pointer typically occupy?

- [ ] a). 2 bytes
- [x] b). 4 bytes
- [ ] c). 8 bytes
- [ ] d). 16 bytes

#### What is the equivalent pointer notation for an array `A[10]`?
- [ ] a). `A`
- [ ] b). `&A`
- [ ] c). `A[0]`
- [x] d). `&A[0]`

#### Which of the following correctly declares and initializes an array of 6 integers?
- [x] a). `int x[6] = {19, 10, 8, 17, 9, 15};`
- [ ] b). `int x = {19, 10, 8, 17, 9, 15};`
- [ ] c). `int x[6] = {19, 10, 8};`
- [ ] d). `int x[6];`

#### What is the primary advantage of using std::vector over arrays in C++?
- [ ] a). They are faster.
- [x] b). They avoid buffer overflows.
- [ ] c). They cannot be resized.
- [ ] d). They use less memory.

#### How is memory de-allocated for a dynamically allocated array `P` in C++? 
- [ ] a). `delete P;`
- [ ] b). `free(P);`
- [x] c). `delete[] P;`
- [ ] d). `dealloc(P);`

#### What does the following code print?
```cpp
int a[5] = {1, 2, 3, 4, 5};
int *p = a;
p += 2;
std::cout << *p << std::endl;
```

- [ ] a). 1
- [ ] b). 2
- [x] c). 3
- [ ] d). 4

#### What is the correct way to define a pointer to a pointer to a double? 
- [x] a). `double **P;`
- [ ] b). `double P*;`
- [ ] c). `double &P;`
- [ ] d). `double *P;`

#### Which memory allocation method is considered to be more of a C method rather than C++?
- [ ] a). `new`
- [ ] b). `delete`
- [x] c). `malloc`
- [ ] d). `free`

#### What does the following code do?
```cpp
int *P;
P = new int;
*P = 24;
delete P;
```

- [x] a). Allocates memory for an integer, assigns it the value 24, and then deallocates the memory.
- [ ] b). Causes a memory leak.
- [ ] c). Allocates memory for an array of integers.
- [ ] d). Allocates memory for a pointer.

#### What does the following code snippet do?
```cpp
int *P = new int[20];
P[12] = 24;
delete[] P;
```

- [x] a). Allocates memory for 20 integers, assigns the 13th element the value 24, and then deallocates the memory.
- [ ] b). Causes a memory leak.
- [ ] c). Allocates memory for a single integer.
- [ ] d). Allocates memory for a double.

#### How is a static array stored in memory?
- [ ] a). Heap
- [x] b). Stack
- [ ] c). Free store
- [ ] d). Global memory

#### What is the size limit of addressable RAM in a 32-bit program?
- [ ] a). 2 GB
- [x] b). 4 GB
- [ ] c). 8 GB
- [ ] d). 16 GB

#### Which of the following statements is true about stack memory?
- [ ] a). It can become fragmented over time.
- [ ] b). It is managed manually by the programmer.
- [x] c). It is of a fixed size set by the operating system.
- [ ] d). It is used for dynamic memory allocation.

#### Why should arrays be avoided whenever possible in C++ programs?
- [ ] a). They are slower than other data structures.
- [x] b). They are the largest single source of bugs.
- [ ] c). They use more memory than other data structures.
- [ ] d). They cannot be dynamically allocated.

#### Which operator is used to obtain the memory address of a variable in C++?
- [ ] a). `*`
- [x] b). `&`
- [ ] c). `->`
- [ ] d). `::`

#### What happens when you perform pointer arithmetic in C++?
- [ ] a). The pointer changes its type.
- [x] b). The pointer moves by the size of the data type it points to.
- [ ] c). The pointer is dereferenced.
- [ ] d). The pointer is deleted.

#### Which of the following correctly declares a pointer to an array of integers?
- [ ] a). `int  P;`
- [ ] b). `int *P[10];`
- [x] c). `int (*P)[10];`
- [ ] d). `int P[10];`

#### What does the following code snippet do?
```cpp
int x[6] = {19, 10, 8};
```

- [x] a). Declares an array of 6 integers and initializes the first 3 elements.
- [ ] b). Declares an array of 3 integers.
- [ ] c). Causes a compilation error.
- [ ] d). Declares and initializes an array of 6 integers to zero.

#### How can a function return more than one value using pointers in C++?
- [ ] a). By returning an array.
- [x] b). By passing pointers as parameters and modifying the values at those addresses.
- [ ] c). By using the return statement multiple times.
- [ ] d). By using global variables.

#### What is the primary risk associated with dynamic memory allocation?
- [ ] a). Stack overflow
- [x] b). Memory fragmentation
- [ ] c). Compile-time errors
- [ ] d). Global variable conflicts

#### What is the main difference between stack and heap memory allocation in C++?
- [ ] a). Stack memory is managed manually, while heap memory is managed automatically.
- [ ] b). Stack memory is dynamically allocated, while heap memory is statically allocated.
- [x] c). Stack memory is of fixed size, while heap memory can be resized.
- [ ] d). Stack memory is slower, while heap memory is faster.

##### Which of the following is a valid way to deallocate memory allocated with malloc in C++? 
- [x] a). `free()`
- [ ] b). `delete`
- [ ] c). `delete[]`
- [ ] d). `dealloc()`

#### How do you access the nth element of an array using pointer notation? 
- [ ] a). `array[n]`
- [x] b). `*(array + n)`
- [ ] c). `&array[n]`
- [ ] d). `array->n`

#### What is the correct way to declare a pointer to a function that takes an int and returns a double? 
- [x] a). `double (*func)(int);`
- [ ] b). `double (*func(int));`
- [ ] c). `double *func(int);`
- [ ] d). `double (*func) int;`

#### Which of the following statements is true about pointers in C++? 
- [ ] a). Pointers are automatically deallocated at the end of the program.
- [x] b). Pointers can be used to access array elements.
- [ ] c). Pointers cannot be incremented or decremented.
- [ ] d). Pointers are always initialized to nullptr.

#### What does the following code snippet print? 
```cpp
int a[5] = {1, 2, 3, 4, 5};
int *p = a;
std::cout << p[2] << std::endl;
```

- [ ] a). 1
- [ ] b). 2
- [x] c). 3
- [ ] d). 4

#### Which of the following correctly allocates memory for a two-dimensional array of doubles? 
- [x] a). `double  P = new double*[max_i];`
- [ ] b). `double P[max_i][max_j];`
- [ ] c). `double  P = malloc(sizeof(double) * max_i * max_j);`
- [ ] d). `double P = new double[max_i * max_j];`

#### What is the purpose of the delete operator in C++? 
- [ ] a). To allocate memory
- [x] b). To deallocate memory
- [ ] c). To access the value at a pointer's memory location
- [ ] d). To return a pointer's address

#### How can you prevent memory leaks in C++? 
- [ ] a). By using global variables
- [x] b). By deallocating memory using delete or delete[]
- [ ] c). By avoiding pointer arithmetic
- [ ] d). By using static variables

#### What does the following code snippet print? 
```cpp
int a = 10;
int *b = &a;
std::cout << *b << std::endl;
```

- [ ] a). The address of a
- [x] b). The value of a
- [ ] c). The address of b
- [ ] d). The value of b

#### How do you access the value stored at the memory address pointed to by a pointer?
- [ ] a). `&ptr`
- [x] b). `*ptr`
- [ ] c). `ptr*`
- [ ] d). `ptr&`

#### If ptr is a pointer to an integer, what does ptr + 1 do?
- [ ] a). Moves the pointer to the next memory address.
- [ ] b). Adds 1 to the value pointed to by ptr.
- [x] c). Moves the pointer to the next integer.
- [ ] d). Causes a compile-time error.

#### Given the following code, what is *(ptr + 3)?
```cpp
int arr[4] = {1, 2, 3, 4};
int *ptr = arr;
```

- [ ] a). 1
- [ ] b). 2
- [ ] c). 3
- [x] d). 4

#### Which operator is used to allocate memory dynamically for an integer in C++?
- [ ] a). `malloc()`
- [ ] b). `calloc()`
- [x] c). `new`
- [ ] d). `allocate`

#### What does the following code do?
```cpp
int *ptr = new int;
```

- [ ] a). Declares a pointer to an integer and initializes it to nullptr.
- [x] b). Declares a pointer to an integer and allocates memory for it.
- [ ] c). Declares an integer and allocates memory for it.
- [ ] d). Declares a pointer to an integer and assigns it the value 0.

#### What will happen if you try to delete a pointer twice?
- [ ] a). The program will run without errors.
- [x] b). The program will crash or exhibit undefined behavior.
- [ ] c). The memory will be freed twice.
- [ ] d). The program will delete the pointer only once.

#### Which of the following statements is true?
- [ ] a). Array elements are stored in non-contiguous memory locations.
- [x] b). The name of an array acts as a pointer to its first element.
- [ ] c). Pointers and arrays cannot be used together.
- [ ] d). Pointers cannot be used to traverse an array.

#### How do you pass a pointer to a function?
- [ ] a). `function(&ptr);`
- [ ] b). `function(*ptr);`
- [x] c). `function(ptr);`
- [ ] d). `function(ptr*);`

#### What is the advantage of passing a pointer to a function?
- [x] a). It allows for passing large amounts of data efficiently.
- [ ] b). It prevents the function from modifying the original data.
- [ ] c). It allows the function to return multiple values.
- [ ] d). It causes the program to run faster.

#### What will the following code print?
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
- [x] b). 100
- [ ] c). Memory address of x
- [ ] d). Undefined

---