# Quiz: Mini-Introduction to Parallel
## Programming with C++

---

### 1. What is parallel programming?
- [ ] a). Using a single processor to complete a task  
- [ ] b). Using more than one processor or computer to complete a task  
- [ ] c). Using a single thread to complete multiple tasks  
- [ ] d). Using more memory to complete a task

### 2. Which of the following is NOT a reason for using parallel computing?
- [ ] a). Save time  
- [ ] b). Solve larger problems  
- [ ] c). Provide concurrency  
- [ ] d). Increase the complexity of debugging

### 3. What is data parallelism?
- [ ] a). Each process performs different functions on the same data  
- [ ] b). Each process does the same work on unique and independent pieces of data  
- [ ] c). Each process performs different functions on different pieces of data  
- [ ] d). Each process performs the same functions but does not communicate with each other

### 4. Which library is commonly used for high-level data parallelism in C++?
- [ ] a). MPI  
- [ ] b). OpenMP  
- [ ] c). CUDA  
- [ ] d). Pthreads

### 5. What does the term "task parallelism" refer to?
- [ ] a). Each process does the same work on unique data  
- [ ] b). Each process performs different functions on the same data  
- [ ] c). Each process performs the same functions but does not communicate with each other  
- [ ] d). Each process works on a part of the solution and passes the result to the next process

### 6. True or False: In functional parallelism, each process performs a different code section that is independent.
- [ ] a). True  
- [ ] b). False

### 7. What does Amdahl's Law state about parallel programs?
- [ ] a). Parallel programs can achieve infinite speedup with enough processors  
- [ ] b). Parallel programs have no limit to speedup  
- [ ] c). There is a strict limit on the speedup that can be realized using multiple processors  
- [ ] d). Parallel programs are always faster than serial programs

### 8. What is the formula for speedup according to Amdahl's Law?
- [ ] a). S = 1 / (fs + fp * N)  
- [ ] b). S = 1 / (fs + fp / N)  
- [ ] c). S = (fs + fp * N) / 1  
- [ ] d). S = (fs + fp / N) / 1

### 9. What does the term "synchronization" refer to in parallel programming?
- [ ] a). The temporal coordination of parallel tasks  
- [ ] b). The spatial coordination of parallel tasks  
- [ ] c). The isolation of parallel tasks  
- [ ] d). The independence of parallel tasks

### 10. True or False: OpenMP is ideal for writing distributed computing applications.
- [ ] a). True  
- [ ] b). False

### 11. What is the primary purpose of the `#pragma omp parallel` directive in OpenMP?
- [ ] a). To define a serial region of code  
- [ ] b). To define a parallel region of code  
- [ ] c). To define a function call  
- [ ] d). To define a memory allocation

### 12. In OpenMP, what is the default scope of variables at the beginning of a parallel block?
- [ ] a). Private to each thread  
- [ ] b). Shared across threads  
- [ ] c). Undefined  
- [ ] d). Local to the master thread

### 13. Which of the following best describes "fine-grained" parallelism?
- [ ] a). Very little computation per communication-byte  
- [ ] b). Extensive computation per communication-byte  
- [ ] c). Equal computation and communication  
- [ ] d). No communication required

### 14. What does MPI stand for in the context of parallel programming?
- [ ] a). Multi-Processor Interface  
- [ ] b). Message Passing Interface  
- [ ] c). Memory Processing Interface  
- [ ] d). Multi-Parallel Interface

### 15. True or False: In shared memory systems, threads share the heap but have their own stack.
- [ ] a). True  
- [ ] b). False

---

## Answers

1. b) Using more than one processor or computer to complete a task
2. d) Increase the complexity of debugging
3. b) Each process does the same work on unique and independent pieces of data
4. b) OpenMP
5. c) Each process performs the same functions but does not communicate with each other
6. a) True
7. c) There is a strict limit on the speedup that can be realized using multiple processors
8. b) S = 1 / (fs + fp / N)
9. a) The temporal coordination of parallel tasks
10. b) False
11. b) To define a parallel region of code
12. b) Shared across threads
13. a) Very little computation per communication-byte
14. b) Message Passing Interface
15. a) True

---


# Advanced Programming in C++ - Quiz: Code Parallelization with OpenMP

## Instructions
- Answer the following questions to the best of your ability.
- Each section is focused on different aspects of code parallelization, specifically using OpenMP.
- Select the correct answer for each question.
- Correct answers are provided at the end of the quiz.

---

## Section 1: Introduction to OpenMP

### 1. What is OpenMP?

- [ ] a). A library for parallel computing in Python.
- [ ] b). A compiler extension for parallel computing in C, C++, and Fortran.
- [ ] c). A tool for debugging parallel applications.
- [ ] d). A runtime environment for distributed computing.

### 2. Which directive is used to parallelize a `for` loop in OpenMP?

- [ ] a). `#pragma omp parallel`
- [ ] b). `#pragma omp for`
- [ ] c). `#pragma omp parallel for`
- [ ] d). `#pragma omp task`

### 3. How do you enable OpenMP support when compiling a C++ program with `g++`?

- [ ] a). `g++ -openmp`
- [ ] b). `g++ -fopenmp`
- [ ] c). `g++ -omp`
- [ ] d). `g++ -parallel`

### 4. Which environment variable controls the number of threads in an OpenMP program?

- [ ] a). `OMP_THREADS`
- [ ] b). `NUM_THREADS`
- [ ] c). `OMP_NUM_THREADS`
- [ ] d). `THREAD_COUNT`

---

## Section 2: Parallelizing Loops and Tasks

### 5. What is the purpose of the `#pragma omp parallel for` directive?

- [ ] a). To execute the code in parallel without splitting the loop.
- [ ] b). To create a single thread to execute the loop sequentially.
- [ ] c). To split a loop among multiple threads for parallel execution.
- [ ] d). To execute the code block in a distributed manner across different machines.

### 6. Which of the following code snippets correctly parallelizes a loop using OpenMP?

```cpp
int arr[1000];
#pragma omp parallel for
for (int i = 0; i < 1000; i++) {
    arr[i] = i * i;
}
```

- [ ] a). The loop will run sequentially.
- [ ] b). The loop will run in parallel using multiple threads.
- [ ] c). The loop will run in parallel, but there will be a race condition.
- [ ] d). The loop will generate compilation errors.

7. How does OpenMP distribute iterations in a parallelized for loop by default?

- [ ] a). OpenMP divides the iterations evenly among the threads.
- [ ] b). OpenMP lets the user manually assign iterations to each thread.
- [ ] c). OpenMP uses a random distribution of iterations.
- [ ] d). OpenMP assigns iterations to the first available thread.

8. What is the effect of the #pragma omp single directive?

- [ ] a). It ensures that a specific block of code is executed by only one thread.
- [ ] b). It splits the block of code evenly between threads.
- [ ] c). It creates a barrier where all threads must wait.
- [ ] d). It duplicates the execution of the block of code across all threads.

Section 3: Synchronization and Data Sharing
9. Which directive is used to prevent race conditions by ensuring mutual exclusion?

- [ ] a). #pragma omp critical
- [ ] b). #pragma omp barrier
- [ ] c). #pragma omp single
- [ ] d). #pragma omp master

10. What happens when you use #pragma omp barrier?

- [ ] a). It stops all threads permanently.
- [ ] b). It synchronizes all threads, making them wait until they all reach the barrier.
- [ ] c). It terminates all threads except for the master thread.
- [ ] d). It causes threads to skip the next section of code.

11. Which clause allows you to specify private variables for each thread?

- [ ] a). private()
- [ ] b). shared()
- [ ] c). firstprivate()
- [ ] d). reduction()

12. How do you specify that a variable should be shared between all threads?

- [ ] a). By using the shared() clause.
- [ ] b). By declaring the variable inside the loop.
- [ ] c). By declaring the variable as static.
- [ ] d). By using the critical() clause.

Section 4: Reductions and Performance Considerations
13. What is the purpose of the reduction clause in OpenMP?

- [ ] a). To reduce the number of threads used by the program.
- [ ] b). To combine the results of a parallel computation into a single result.
- [ ] c). To reduce the amount of memory used by the program.
- [ ] d). To limit the amount of parallelization in a program.

14. Which of the following OpenMP directive is used for reductions?

- [ ] a). #pragma omp critical
- [ ] b). #pragma omp barrier
- [ ] c). #pragma omp reduction
- [ ] d). #pragma omp parallel reduction

15. Given the following code, what is the result after the loop?

```cpp
int sum = 0;
#pragma omp parallel for reduction(+:sum)
for (int i = 1; i <= 100; i++) {
    sum += i;
}
```

- [ ] a). The sum of numbers from 1 to 100 is computed correctly.
- [ ] b). The sum will have an undefined value due to a race condition.
- [ ] c). The loop will execute sequentially because reductions do not work with parallelism.
- [ ] d). The loop will generate compilation errors.

16. Which of the following is a common pitfall when parallelizing code with OpenMP?

- [ ] a). Not using enough threads.
- [ ] b). Creating too many critical sections, which can reduce parallel efficiency.
- [ ] c). Forgetting to include the omp.h header file.
- [ ] d). Running the program without compiling with OpenMP flags.

Section 5: Best Practices and Advanced Topics
17. How can you control the workload distribution among threads in a parallel loop?

- [ ] a). By using the schedule clause.
- [ ] b). By modifying the loop control variable directly.
- [ ] c). By specifying the thread_count() function.
- [ ] d). By using the critical directive within the loop.

18. What does the schedule(static, chunk_size) clause do?

- [ ] a). Distributes a fixed number of loop iterations (chunk size) to each thread statically.
- [ ] b). Dynamically assigns loop iterations to each thread.
- [ ] c). Prevents threads from re-executing the same iterations.
- [ ] d). Specifies that each thread should execute all iterations in sequential order.

19. Which of the following OpenMP directives controls nested parallelism (parallel regions within parallel regions)?

- [ ] a). #pragma omp nested
- [ ] b). #pragma omp task
- [ ] c). omp_set_nested()
- [ ] d). omp_nested()

20. What is a benefit of using OpenMP over manual thread management in C++?

- [ ] a). OpenMP provides an easier interface for parallelizing loops and tasks.
- [ ] b). OpenMP eliminates all performance overhead.
- [ ] c). OpenMP can only be used for scientific computing.
- [ ] d). OpenMP allows direct manipulation of individual threads.

Answers

- [ ] b). A compiler extension for parallel computing in C, C++, and Fortran.
- [ ] c). #pragma omp parallel for
- [ ] b). g++ -fopenmp
- [ ] c). OMP_NUM_THREADS
- [ ] c). To split a loop among multiple threads for parallel execution.
- [ ] b). The loop will run in parallel using multiple threads.
- [ ] a). OpenMP divides the iterations evenly among the threads.
- [ ] a). It ensures that a specific block of code is executed by only one thread.
- [ ] a). #pragma omp critical
- [ ] b). It synchronizes all threads, making them wait until they all reach the barrier.
- [ ] a). private()
- [ ] a). By using the shared() clause.
- [ ] b). To combine the results of a parallel computation into a single result.
- [ ] c). #pragma omp reduction
- [ ] a). The sum of numbers from 1 to 100 is computed correctly.
- [ ] b). Creating too many critical sections, which can reduce parallel efficiency.
- [ ] a). By using the schedule clause.
- [ ] a). Distributes a fixed number of loop iterations (chunk size) to each thread statically.
- [ ] c). omp_set_nested()
- [ ] a). OpenMP provides an easier interface for parallelizing loops and tasks.

End of Quiz



# Advanced Programming in C++ - Quiz: Code Parallelization with OpenMP

## Instructions
- Answer the following questions to the best of your ability.
- Each section is focused on a specific aspect of code parallelization with OpenMP.
- Select the correct answer for each question.
- Correct answers are provided at the end of the quiz.

---

## Section 1: Introduction to OpenMP

### 1. What is OpenMP?

- [ ] a). A library for distributed computing.
- [ ] b). A parallel programming API that supports multi-platform shared memory multiprocessing.
- [ ] c). A debugging tool for parallel programs.
- [ ] d). A compiler-specific optimization technique.

### 2. Which directive is used to parallelize a loop in OpenMP?

- [ ] a). `#pragma omp parallel`
- [ ] b). `#pragma omp for`
- [ ] c). `#pragma omp loop`
- [ ] d). `#pragma omp parallel for`

### 3. How do you specify the number of threads in an OpenMP parallel region?

- [ ] a). `#pragma omp threads(4)`
- [ ] b). `omp_set_num_threads(4);`
- [ ] c). `#pragma omp parallel num_threads(4)`
- [ ] d). Both B and C

### 4. What is the default behavior if the number of threads is not specified in an OpenMP program?

- [ ] a). The program uses a single thread.
- [ ] b). The program uses the maximum number of available threads.
- [ ] c). The program generates a runtime error.
- [ ] d). The program uses two threads.

### 5. Which of the following is true about the `#pragma omp parallel` directive?

- [ ] a). It only works for loops.
- [ ] b). It creates a team of threads to execute the code block in parallel.
- [ ] c). It must always be followed by `#pragma omp for`.
- [ ] d). It automatically handles race conditions.

---

## Section 2: Parallel Loops and Work-sharing Constructs

### 6. Which OpenMP directive is used to parallelize the execution of loop iterations?

- [ ] a). `#pragma omp section`
- [ ] b). `#pragma omp critical`
- [ ] c). `#pragma omp parallel`
- [ ] d). `#pragma omp for`

### 7. What is the effect of using the `schedule(static)` clause with the `#pragma omp for` directive?

- [ ] a). It assigns loop iterations to threads in a round-robin fashion.
- [ ] b). It assigns loop iterations to threads in contiguous blocks.
- [ ] c). It allows dynamic assignment of loop iterations.
- [ ] d). It prevents loop iterations from being parallelized.

### 8. What does the `reduction` clause do in OpenMP?

- [ ] a). It reduces the number of threads used in a parallel region.
- [ ] b). It combines the results of each thread into a single value after the parallel region.
- [ ] c). It reduces the amount of code executed by each thread.
- [ ] d). It ensures that only one thread executes a code block at a time.

### 9. How can you ensure that each thread gets a unique copy of a variable in an OpenMP parallel region?

- [ ] a). Use the `shared` clause.
- [ ] b). Use the `private` clause.
- [ ] c). Use the `reduction` clause.
- [ ] d). Use the `copyin` clause.

### 10. What is the purpose of the `#pragma omp single` directive?

- [ ] a). To ensure that only one thread executes a specific code block.
- [ ] b). To parallelize the execution of loop iterations.
- [ ] c). To create a single thread team.
- [ ] d). To synchronize threads at the end of a parallel region.

---

## Section 3: Synchronization in OpenMP

### 11. Which directive is used to prevent multiple threads from executing a block of code simultaneously?

- [ ] a). `#pragma omp atomic`
- [ ] b). `#pragma omp critical`
- [ ] c). `#pragma omp barrier`
- [ ] d). `#pragma omp single`

### 12. What does the `#pragma omp barrier` directive do?

- [ ] a). It prevents race conditions by ensuring atomic operations.
- [ ] b). It stops all threads at the barrier until all threads have reached it.
- [ ] c). It allows only one thread to execute a specific block of code.
- [ ] d). It reduces the number of threads in a parallel region.

### 13. How do you protect a shared variable from being updated by multiple threads simultaneously?

- [ ] a). Use the `#pragma omp atomic` directive.
- [ ] b). Use the `#pragma omp critical` directive.
- [ ] c). Use the `#pragma omp ordered` directive.
- [ ] d). Both A and B.

### 14. What is the purpose of the `#pragma omp ordered` directive?

- [ ] a). To execute loop iterations in a specific order across all threads.
- [ ] b). To ensure that all threads update a variable in a specific order.
- [ ] c). To prevent race conditions by locking shared variables.
- [ ] d). To ensure that only one thread is active at a time.

### 15. Which directive should be used to ensure that only the master thread executes a block of code?

- [ ] a). `#pragma omp master`
- [ ] b). `#pragma omp critical`
- [ ] c). `#pragma omp single`
- [ ] d). `#pragma omp barrier`

---

## Section 4: Advanced Topics in OpenMP

### 16. What is the purpose of the `#pragma omp task` directive?

- [ ] a). To create a parallel loop.
- [ ] b). To define a block of code to be executed as a task by any thread.
- [ ] c). To synchronize threads.
- [ ] d). To ensure only one thread executes a code block.

### 17. How can you enable nested parallelism in OpenMP?

- [ ] a). By using the `omp_set_num_threads()` function.
- [ ] b). By setting the `OMP_NESTED` environment variable to `TRUE`.
- [ ] c). By using the `#pragma omp nested` directive.
- [ ] d). OpenMP does not support nested parallelism.

### 18. What is the effect of the `nowait` clause in OpenMP?

- [ ] a). It prevents threads from synchronizing at the end of a work-sharing construct.
- [ ] b). It forces threads to wait at the end of a parallel region.
- [ ] c). It reduces the number of threads in a parallel region.
- [ ] d). It enables the `reduction` clause.

### 19. How can you distribute different sections of code to different threads in OpenMP?

- [ ] a). Use the `#pragma omp for` directive.
- [ ] b). Use the `#pragma omp sections` directive.
- [ ] c). Use the `#pragma omp single` directive.
- [ ] d). Use the `#pragma omp atomic` directive.

### 20. Which of the following OpenMP clauses allows a variable to retain its value across different parallel regions?

- [ ] a). `firstprivate`
- [ ] b). `shared`
- [ ] c). `lastprivate`
- [ ] d). `threadprivate`

---

## Answers

1. **B) A parallel programming API that supports multi-platform shared memory multiprocessing.**
2. **D) `#pragma omp parallel for`**
3. **D) Both B and C**
4. **B) The program uses the maximum number of available threads.**
5. **B) It creates a team of threads to execute the code block in parallel.**
6. **D) `#pragma omp for`**
7. **B) It assigns loop iterations to threads in contiguous blocks.**
8. **B) It combines the results of each thread into a single value after the parallel region.**
9. **B) Use the `private` clause.**
10. **A) To ensure that only one thread executes a specific code block.**
11. **B) `#pragma omp critical`**
12. **B) It stops all threads at the barrier until all threads have reached it.**
13. **D) Both A and B.**
14. **A) To execute loop iterations in a specific order across all threads.**
15. **A) `#pragma omp master`**
16. **B) To define a block of code to be executed as a task by any thread.**
17. **B) By setting the `OMP_NESTED` environment variable to `TRUE`.**
18. **A) It prevents threads from synchronizing at the end of a work-sharing construct.**
19. **B) Use the `#pragma omp sections` directive.**
20. **D) `threadprivate`**

---

## End of Quiz

---

This quiz covers essential aspects of parallel programming using OpenMP, including basic concepts, loop parallelization, synchronization, and advanced topics. The Markdown format ensures it can be easily integrated into any interactive or static quiz tool.

