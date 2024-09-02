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

cpp

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

cpp

std::for_each(std::execution::par, vec.begin(), vec.end(), [](int &n) { n *= 2; });

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