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



# Parallel Programming in C++ Quiz

This quiz covers the basics of parallel programming in C++, including threads, mutexes, condition variables, parallel algorithms in C++17, and concurrency features in C++20. Each question is followed by the correct answer.

## Section 1: Threads and the `std::thread` Class

### 1. What is the primary purpose of the `std::thread` class in C++?
- [ ] a). To manage memory allocation
- [ ] b). To handle input/output operations
- [ ] c). To create and manage threads
- [ ] d). To synchronize access to shared resources
- **Correct Answer:** C) To create and manage threads

### 2. How do you ensure that a thread completes its execution before the main program continues?
- [ ] a). Use `std::thread::detach()`
- [ ] b). Use `std::thread::join()`
- [ ] c). Use `std::thread::terminate()`
- [ ] d). Use `std::thread::wait()`
- **Correct Answer:** B) Use `std::thread::join()`

### 3. What happens when you call `std::thread::detach()` on a thread?
- [ ] a). The thread is terminated immediately
- [ ] b). The thread runs independently of the main thread
- [ ] c). The thread waits for the main thread to finish
- [ ] d). The thread is paused until reattached
- **Correct Answer:** B) The thread runs independently of the main thread

### 4. Which of the following is a potential risk when detaching a thread?
- [ ] a). The thread may continue running after the main program has terminated
- [ ] b). The thread might rejoin the main thread automatically
- [ ] c). The thread will always complete before the main program terminates
- [ ] d). The thread will throw an exception if detached
- **Correct Answer:** A) The thread may continue running after the main program has terminated

### 5. What is the output of the following code snippet?

```cpp
#include <iostream>
#include <thread>

void print_hello() {
    std::cout << "Hello from thread!\n";
}

int main() {
    std::thread t(print_hello);
    t.detach();
    return 0;
}
```

- [ ] a). Hello from thread!
- [ ] b). Undefined behavior
- [ ] c). No output
- [ ] d). Compilation error
    Correct Answer: A) Hello from thread! (with potential for undefined behavior if the main thread exits before the detached thread prints)

Section 2: Mutexes and Synchronization
6. What is the primary purpose of a std::mutex in C++?

- [ ] a). To manage memory allocation
- [ ] b). To ensure that only one thread accesses a shared resource at a time
- [ ] c). To create and manage threads
- [ ] d). To handle exceptions in threads
    Correct Answer: B) To ensure that only one thread accesses a shared resource at a time

7. Which of the following is the correct way to use a std::mutex to protect shared data?

- [ ] a). mutex.lock(); ... mutex.unlock();
- [ ] b). std::thread::lock(); ... std::thread::unlock();
- [ ] c). mutex.acquire(); ... mutex.release();
- [ ] d). std::mutex::lock(); ... std::mutex::unlock();
    Correct Answer: A) mutex.lock(); ... mutex.unlock();

8. How does std::lock_guard help in managing mutexes?

- [ ] a). It automatically locks a mutex when created and unlocks it when destroyed
- [ ] b). It delays the locking of a mutex until needed
- [ ] c). It locks a mutex only if it is not already locked
- [ ] d). It automatically detects and resolves deadlocks
    Correct Answer: A) It automatically locks a mutex when created and unlocks it when destroyed

9. What is a race condition in the context of parallel programming?

- [ ] a). When a thread runs faster than the others
- [ ] b). When two threads compete for CPU time
- [ ] c). When multiple threads access shared data simultaneously, leading to unpredictable results
- [ ] d). When a thread completes before it should
    Correct Answer: C) When multiple threads access shared data simultaneously, leading to unpredictable results

10. What will be the output of the following code snippet if no mutex is used?

```cpp
#include <iostream>
#include <thread>

int counter = 0;

void increment() {
    for (int i = 0; i < 100000; ++i) {
        ++counter;
    }
}

int main() {
    std::thread t1(increment);
    std::thread t2(increment);

    t1.join();
    t2.join();

    std::cout << "Final counter value: " << counter << std::endl;
    return 0;
}
```

- [ ] a). 200000
- [ ] b). 100000
- [ ] c). 0
- [ ] d). An unpredictable value less than or equal to 200000
    Correct Answer: D) An unpredictable value less than or equal to 200000

Section 3: Condition Variables
11. What is the purpose of a std::condition_variable in C++?

- [ ] a). To provide mutual exclusion between threads
- [ ] b). To allow threads to wait for certain conditions to be met
- [ ] c). To manage the creation and destruction of threads
- [ ] d). To terminate threads that are no longer needed
    Correct Answer: B) To allow threads to wait for certain conditions to be met

12. Which function is used by a thread to wait on a condition variable?

- [ ] a). cv.wait(lock);
- [ ] b). cv.notify_all();
- [ ] c). cv.unlock();
- [ ] d). cv.lock();
    Correct Answer: A) cv.wait(lock);

13. How does a thread notify other threads that a condition has been met?

- [ ] a). By calling std::thread::notify_all()
- [ ] b). By calling std::mutex::notify_all()
- [ ] c). By calling std::condition_variable::notify_one() or std::condition_variable::notify_all()
- [ ] d). By setting a global flag
    Correct Answer: C) By calling std::condition_variable::notify_one() or std::condition_variable::notify_all()

14. What is the primary difference between notify_one() and notify_all()?

- [ ] a). notify_one() wakes one waiting thread, while notify_all() wakes all waiting threads
- [ ] b). notify_one() wakes one thread at a time in sequence, while notify_all() wakes one thread
- [ ] c). notify_one() terminates one thread, while notify_all() terminates all threads
- [ ] d). notify_one() is used for mutexes, while notify_all() is used for condition variables
    Correct Answer: A) notify_one() wakes one waiting thread, while notify_all() wakes all waiting threads

15. What is a potential risk of using condition variables incorrectly?

- [ ] a). Deadlock
- [ ] b). Memory leaks
- [ ] c). Compiler errors
- [ ] d). Increased CPU usage
    Correct Answer: A) Deadlock

Section 4: Parallel Algorithms in C++17
16. What was introduced in C++17 to enhance parallelism in algorithms?

- [ ] a). New thread management functions
- [ ] b). Parallel execution policies for standard algorithms
- [ ] c). Enhanced condition variables
- [ ] d). Automatic mutex handling
    Correct Answer: B) Parallel execution policies for standard algorithms

17. Which execution policy should be used to ensure that an algorithm is executed in parallel?

- [ ] a). std::execution::seq
- [ ] b). std::execution::par
- [ ] c). std::execution::unseq
- [ ] d). std::execution::vec
    Correct Answer: B) std::execution::par

18. What is the effect of using std::execution::par with a standard algorithm like std::for_each?

- [ ] a). The algorithm will run sequentially
- [ ] b). The algorithm will run in parallel, utilizing multiple cores
- [ ] c). The algorithm will not compile
- [ ] d). The algorithm will run on a single core
    Correct Answer: B) The algorithm will run in parallel, utilizing multiple cores

19. Which of the following is a valid use of parallel execution in C++17?

```cpp
std::for_each(std::execution::par, vec.begin(), vec.end(), [](int &n) { n *= 2; });
```

- [ ] a). True
- [ ] b). False
    Correct Answer: A) True

20. What is the main advantage of using parallel algorithms in C++17?

- [ ] a). Simpler syntax for thread management
- [ ] b). Automatic synchronization of threads
- [ ] c). Potentially significant performance improvements on multi-core systems
- [ ] d). Easier debugging of parallel code
    Correct Answer: C) Potentially significant performance improvements on multi-core systems

Section 5: Concurrency Features in C++20
21. What is the purpose of std::jthread introduced in C++20?

- [ ] a). To automatically handle thread creation
- [ ] b). To automatically join threads when they go out of scope
- [ ] c). To manage memory allocation for threads
- [ ] d). To provide better error handling in threads
    Correct Answer: B) To automatically join threads when they go out of scope

22. Which C++20 feature allows you to synchronize multiple threads at a specific point before they continue execution?

- [ ] a). std::barrier
- [ ] b). std::jthread
- [ ] c). std::atomic
- [ ] d). std::latch
    Correct Answer: A) std::barrier

23. What is a significant difference between std::latch and std::barrier?

- [ ] a). std::latch can only be used once, while std::barrier can be reused
- [ ] b). std::latch is for single-threaded programs, while std::barrier is for multi-threaded programs
- [ ] c). std::latch is more efficient than std::barrier
- [ ] d). std::latch is used for memory management, while std::barrier is used for synchronization
    Correct Answer: A) std::latch can only be used once, while std::barrier can be reused

24. Which of the following is a benefit of using std::jthread over std::thread?

- [ ] a). std::jthread supports detaching threads more easily
- [ ] b). std::jthread automatically manages the thread lifecycle and ensures it is joined or detached
- [ ] c). std::jthread is faster than std::thread
- [ ] d). std::jthread can be used in C++11 code
    Correct Answer: B) std::jthread automatically manages the thread lifecycle and ensures it is joined or detached

25. What is the main use of std::atomic in parallel programming?

- [ ] a). To manage the lifecycle of threads
- [ ] b). To perform atomic operations on variables, ensuring thread safety without using mutexes
- [ ] c). To synchronize the start of threads
- [ ] d). To allocate memory in parallel programs
    Correct Answer: B) To perform atomic operations on variables, ensuring thread safety without using mutexes
