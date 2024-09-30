# Advanced Programming with C++
# Quiz: Mini-Introduction to Parallel

---

## Parallel programming

#### What is parallel programming?
- [ ] a). Using a single processor to complete a task  
- [x] b). Using more than one processor or computer to complete a task  
- [ ] c). Using a single thread to complete multiple tasks  
- [ ] d). Using more memory to complete a task

#### Which of the following is not a reason for using parallel computing?
- [ ] a). Save time  
- [ ] b). Solve larger problems  
- [ ] c). Provide concurrency  
- [x] d). Increase the complexity of debugging

#### What is data parallelism?
- [ ] a). Each process performs different functions on the same data  
- [x] b). Each process does the same work on unique and independent pieces of data  
- [ ] c). Each process performs different functions on different pieces of data  
- [ ] d). Each process performs the same functions but does not communicate with each other

#### What does the term "task parallelism" refer to?
- [ ] a). Each process does the same work on unique data  
- [ ] b). Each process performs different functions on the same data  
- [x] c). Each process performs the same functions but does not communicate with each other  
- [ ] d). Each process works on a part of the solution and passes the result to the next process

#### In functional parallelism, each process performs a different code section that is independent.
- [x] a). True  
- [ ] b). False

#### What does Amdahl's Law state about parallel programs?
- [ ] a). Parallel programs can achieve infinite speedup with enough processors  
- [ ] b). Parallel programs have no limit to speedup  
- [x] c). There is a strict limit on the speedup that can be realised using multiple processors  
- [ ] d). Parallel programs are always faster than serial programs

#### What is the formula for speedup according to Amdahl's Law?
- [ ] a). S = 1 / (fs + fp * N)  
- [x] b). S = 1 / (fs + fp / N)  
- [ ] c). S = (fs + fp * N) / 1  
- [ ] d). S = (fs + fp / N) / 1

#### What does the term "synchronisation" refer to in parallel programming?
- [x] a). The temporal coordination of parallel tasks  
- [ ] b). The spatial coordination of parallel tasks  
- [ ] c). The isolation of parallel tasks  
- [ ] d). The independence of parallel tasks

#### Which of the following best describes "fine-grained" parallelism?
- [x] a). Very little computation per communication-byte  
- [ ] b). Extensive computation per communication-byte  
- [ ] c). Equal computation and communication  
- [ ] d). No communication required

#### What does MPI stand for in the context of parallel programming?
- [ ] a). Multi-Processor Interface  
- [x] b). Message Passing Interface  
- [ ] c). Memory Processing Interface  
- [ ] d). Multi-Parallel Interface

#### In shared memory systems, threads share the heap but have their own stack.
- [x] a). True  
- [ ] b). False

---
## OpenMP

#### What is the primary purpose of the `#pragma omp parallel` directive in OpenMP?
- [ ] a). To define a serial region of code  
- [x] b). To define a parallel region of code  
- [ ] c). To define a function call  
- [ ] d). To define a memory allocation

#### In OpenMP, what is the default scope of variables at the beginning of a parallel block?
- [ ] a). Private to each thread  
- [x] b). Shared across threads  
- [ ] c). Undefined  
- [ ] d). Local to the master thread

#### Which directive is used to parallelise a `for` loop in OpenMP?
- [ ] a). `#pragma omp parallel`
- [ ] b). `#pragma omp for`
- [x] c). `#pragma omp parallel for`
- [ ] d). `#pragma omp task`

#### How do you enable OpenMP support when compiling a C++ program with `g++`?
- [ ] a). `g++ -openmp`
- [x] b). `g++ -fopenmp`
- [ ] c). `g++ -omp`
- [ ] d). `g++ -parallel`

#### Which environment variable controls the number of threads in an OpenMP program?
- [ ] a). `OMP_THREADS`
- [ ] b). `NUM_THREADS`
- [x] c). `OMP_NUM_THREADS`
- [ ] d). `THREAD_COUNT`

#### What is the purpose of the `#pragma omp parallel for` directive?
- [ ] a). To execute the code in parallel without splitting the loop.
- [ ] b). To create a single thread to execute the loop sequentially.
- [x] c). To split a loop among multiple threads for parallel execution.
- [ ] d). To execute the code block in a distributed manner across different machines.

#### Which is the expected behaviour of the following code snippet?
```cpp
int arr[1000];
#pragma omp parallel for
for (int i = 0; i < 1000; i++) {
    arr[i] = i * i;
}
```

- [ ] a). The loop will run sequentially.
- [x] b). The loop will run in parallel using multiple threads.
- [ ] c). The loop will run in parallel, but there will be a race condition.
- [ ] d). The loop will generate compilation errors.

#### How does OpenMP distribute iterations in a parallelised for loop by default?
- [x] a). OpenMP divides the iterations evenly among the threads.
- [ ] b). OpenMP lets the user manually assign iterations to each thread.
- [ ] c). OpenMP uses a random distribution of iterations.
- [ ] d). OpenMP assigns iterations to the first available thread.

#### What is the effect of the #pragma omp single directive?
- [x] a). It ensures that a specific block of code is executed by only one thread.
- [ ] b). It splits the block of code evenly between threads.
- [ ] c). It creates a barrier where all threads must wait.
- [ ] d). It duplicates the execution of the block of code across all threads.

#### Which directive is used to prevent race conditions by ensuring mutual exclusion?
- [x] a). `#pragma omp critical`
- [ ] b). `#pragma omp barrier`
- [ ] c). `#pragma omp single`
- [ ] d). `#pragma omp master`

#### Which clause allows you to specify private variables for each thread?
- [x] a). `private()`
- [ ] b). `shared()`
- [ ] c). `firstprivate()`
- [ ] d). `reduction()`

#### How do you specify that a variable should be shared between all threads?

- [x] a). By using the `shared()` clause.
- [ ] b). By declaring the variable inside the loop.
- [ ] c). By declaring the variable as static.
- [ ] d). By using the `critical()` clause.

#### What is the purpose of the reduction clause in OpenMP?
- [ ] a). To reduce the number of threads used by the program.
- [x] b). To combine the results of a parallel computation into a single result after the parallel region.
- [ ] c). To reduce the amount of memory used by the program.
- [ ] d). To limit the amount of parallelisation in a program.

#### Given the following code, what is the result after the loop?
```cpp
int sum = 0;
#pragma omp parallel for reduction(+:sum)
for (int i = 1; i <= 100; i++) {
    sum += i;
}
```

- [x] a). The sum of numbers from 1 to 100 is computed correctly.
- [ ] b). The sum will have an undefined value due to a race condition.
- [ ] c). The loop will execute sequentially because reductions do not work with parallelism.
- [ ] d). The loop will generate compilation errors.

#### Which of the following is a common pitfall when parallelising code with OpenMP?
- [ ] a). Not using enough threads.
- [x] b). Creating too many critical sections, which can reduce parallel efficiency.
- [ ] c). Forgetting to include the omp.h header file.
- [ ] d). Running the program without compiling with OpenMP flags.

#### Which of the following OpenMP directives controls nested parallelism (parallel regions within parallel regions)?
- [ ] a). `#pragma omp nested`
- [ ] b). `#pragma omp task`
- [x] c). `omp_set_nested()`
- [ ] d). `omp_nested()`

#### What is a benefit of using OpenMP over manual thread management in C++?
- [x] a). OpenMP provides an easier interface for parallelising loops and tasks.
- [ ] b). OpenMP eliminates all performance overhead.
- [ ] c). OpenMP can only be used for scientific computing.
- [ ] d). OpenMP allows direct manipulation of individual threads.

#### How do you specify the number of threads in an OpenMP parallel region?
- [ ] a). `#pragma omp threads(4)`
- [ ] b). `omp_set_num_threads(4);`
- [ ] c). `#pragma omp parallel num_threads(4)`
- [x] d). Both B and C

#### What is the default behavior if the number of threads is not specified in an OpenMP program?
- [ ] a). The program uses a single thread.
- [x] b). The program uses the maximum number of available threads.
- [ ] c). The program generates a runtime error.
- [ ] d). The program uses two threads.

#### Which of the following is true about the `#pragma omp parallel` directive?
- [ ] a). It only works for loops.
- [x] b). It creates a team of threads to execute the code block in parallel.
- [ ] c). It must always be followed by `#pragma omp for`.
- [ ] d). It automatically handles race conditions.

---
## Threads and the `std::thread` Class

#### What is the primary purpose of the `std::thread` class in C++?
- [ ] a). To manage memory allocation
- [ ] b). To handle input/output operations
- [x] c). To create and manage threads
- [ ] d). To synchronise access to shared resources

#### How do you ensure that a thread completes its execution before the main program continues?
- [ ] a). Use `std::thread::detach()`
- [x] b). Use `std::thread::join()`
- [ ] c). Use `std::thread::terminate()`
- [ ] d). Use `std::thread::wait()`

#### What happens when you call `std::thread::detach()` on a thread?
- [ ] a). The thread is terminated immediately
- [x] b). The thread runs independently of the main thread
- [ ] c). The thread waits for the main thread to finish
- [ ] d). The thread is paused until reattached

#### Which of the following is a potential risk when detaching a thread?
- [x] a). The thread may continue running after the main program has terminated
- [ ] b). The thread might rejoin the main thread automatically
- [ ] c). The thread will always complete before the main program terminates
- [ ] d). The thread will throw an exception if detached

#### What is the output of the following code snippet?
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

- [x] a). Hello from thread!
- [ ] b). Undefined behavior
- [ ] c). No output
- [ ] d). Compilation error

#### What is a race condition in the context of parallel programming?
- [ ] a). When a thread runs faster than the others
- [ ] b). When two threads compete for CPU time
- [x] c). When multiple threads access shared data simultaneously, leading to unpredictable results
- [ ] d). When a thread completes before it should

---