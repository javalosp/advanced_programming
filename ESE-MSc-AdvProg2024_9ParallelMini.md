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
