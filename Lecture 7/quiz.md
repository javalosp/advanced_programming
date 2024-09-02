# C++ STL Quiz

This quiz focuses on the Standard Template Library (STL) in C++, covering Algorithms, Functors and Lambdas, Allocators, and advanced topics. Each question is followed by the correct answer.

## Section 1: Algorithms

### 1. What is the time complexity of the `std::sort` algorithm?
- [ ] a). O(n)
- [ ] b). O(n^2)
- [ ] c). O(n log n)
- [ ] d). O(log n)
- **Correct Answer:** C) O(n log n)

### 2. Which STL algorithm is used to search for a specific value within a range?
- [ ] a). `std::find`
- [ ] b). `std::search`
- [ ] c). `std::binary_search`
- [ ] d). `std::equal_range`
- **Correct Answer:** A) `std::find`

### 3. Which STL algorithm is used to count the occurrences of a value in a range?
- [ ] a). `std::count_if`
- [ ] b). `std::count`
- [ ] c). `std::find`
- [ ] d). `std::accumulate`
- **Correct Answer:** B) `std::count`

### 4. What does the `std::transform` algorithm do?
- [ ] a). Copies elements from one range to another
- [ ] b). Applies a function to a range of elements
- [ ] c). Sorts the elements in a range
- [ ] d). Searches for a specific value in a range
- **Correct Answer:** B) Applies a function to a range of elements

### 5. Which STL algorithm would you use to perform a partial sum on a sequence of numbers?
- [ ] a). `std::accumulate`
- [ ] b). `std::inner_product`
- [ ] c). `std::partial_sum`
- [ ] d). `std::transform`
- **Correct Answer:** C) `std::partial_sum`

### 6. What is the output of the following code snippet?

```cpp
#include <iostream>
#include <vector>
#include <algorithm>

int main() {
    std::vector<int> vec = {3, 1, 4, 1, 5, 9};
    std::sort(vec.begin(), vec.end());
    for (int n : vec) std::cout << n << " ";
    return 0;
}

- [ ] a). 3 1 4 1 5 9
- [ ] b). 1 1 3 4 5 9
- [ ] c). 9 5 4 3 1 1
- [ ] d). 3 1 1 4 5 9
    Correct Answer: B) 1 1 3 4 5 9

7. Which STL algorithm is used to check if an element exists in a sorted range?

- [ ] a). std::find
- [ ] b). std::binary_search
- [ ] c). std::count
- [ ] d). std::lower_bound
    Correct Answer: B) std::binary_search

8. What is the purpose of the std::for_each algorithm?

- [ ] a). To apply a function to each element in a range
- [ ] b). To sort the elements in a range
- [ ] c). To find a specific value in a range
- [ ] d). To remove duplicates from a range
    Correct Answer: A) To apply a function to each element in a range

9. What is the difference between std::copy and std::transform?

- [ ] a). std::copy modifies elements, std::transform does not
- [ ] b). std::copy only copies elements, std::transform applies a function while copying
- [ ] c). std::transform is used for sorting, std::copy is not
- [ ] d). std::copy is faster than std::transform
    Correct Answer: B) std::copy only copies elements, std::transform applies a function while copying

10. What is the return type of std::accumulate?

- [ ] a). The same type as the container elements
- [ ] b). The type of the initial value
- [ ] c). void
- [ ] d). bool
    Correct Answer: B) The type of the initial value

Section 2: Functors and Lambdas
11. What is a functor in C++?

- [ ] a). A function pointer
- [ ] b). A lambda expression
- [ ] c). An object that can be called as a function
- [ ] d). A template specialization
    Correct Answer: C) An object that can be called as a function

12. How is a functor typically created in C++?

- [ ] a). Using a struct or class with an overloaded operator()
- [ ] b). Using a function pointer
- [ ] c). Using a lambda expression
- [ ] d). Using std::function
    Correct Answer: A) Using a struct or class with an overloaded operator()

13. Which of the following is a valid lambda expression in C++?

- [ ] a). []() { return 42; }
- [ ] b). ()[] { return 42; }
- [ ] c). [42] { return 42; }
- [ ] d). [] { return 42 }
    Correct Answer: A) []() { return 42; }

14. What is the purpose of the capture list in a lambda expression?

- [ ] a). To specify the return type
- [ ] b). To pass arguments to the lambda
- [ ] c). To capture variables from the surrounding scope
- [ ] d). To declare the lambda as constexpr
    Correct Answer: C) To capture variables from the surrounding scope

15. What is the output of the following code snippet?

cpp

#include <iostream>
#include <vector>
#include <algorithm>

int main() {
    int factor = 2;
    std::vector<int> vec = {1, 2, 3, 4};
    std::for_each(vec.begin(), vec.end(), [factor](int &n) { n *= factor; });
    for (int n : vec) std::cout << n << " ";
    return 0;
}

- [ ] a). 1 2 3 4
- [ ] b). 2 4 6 8
- [ ] c). 4 8 12 16
- [ ] d). 0 0 0 0
    Correct Answer: B) 2 4 6 8

16. How do you specify the return type of a lambda in C++?

- [ ] a). By using a trailing return type (->)
- [ ] b). By specifying it in the capture list
- [ ] c). By using auto as the return type
- [ ] d). By specifying it before the capture list
    Correct Answer: A) By using a trailing return type (->)

17. Which of the following lambda expressions captures x by reference?

- [ ] a). [x]() { return x; }
- [ ] b). [=]() { return x; }
- [ ] c). [&x]() { return x; }
- [ ] d). [this]() { return x; }
    Correct Answer: C) [&x]() { return x; }

18. What does the following lambda expression return when called?

cpp

[]()->int { return 10; }();

- [ ] a). void
- [ ] b). nullptr
- [ ] c). 10
- [ ] d). int
    Correct Answer: C) 10

19. Can a lambda expression be passed as an argument to a function?

- [ ] a). Yes, but only if it's assigned to a std::function
- [ ] b). No, lambdas cannot be passed as arguments
- [ ] c). Yes, lambdas can be passed directly
- [ ] d). Yes, but only if it's converted to a function pointer
    Correct Answer: C) Yes, lambdas can be passed directly

20. What is the purpose of the mutable keyword in a lambda expression?

- [ ] a). To allow modification of captured variables by value
- [ ] b). To make the lambda constexpr
- [ ] c). To allow the lambda to be called multiple times
- [ ] d). To capture variables by reference
    Correct Answer: A) To allow modification of captured variables by value

Section 3: Allocators
21. What is the default allocator used by STL containers?

- [ ] a). std::malloc_allocator
- [ ] b). std::custom_allocator
- [ ] c). std::default_allocator
- [ ] d). std::allocator
    Correct Answer: D) std::allocator

22. Which function in a custom allocator is responsible for allocating memory?

- [ ] a). allocate
- [ ] b). construct
- [ ] c). deallocate
- [ ] d). destroy
    Correct Answer: A) allocate

23. What is the primary advantage of using a custom allocator?

- [ ] a). Simplifies memory management code
- [ ] b). Increases type safety
- [ ] c). Optimizes memory allocation for specific patterns of use
- [ ] d). Makes the code more readable
    Correct Answer: C) Optimizes memory allocation for specific patterns of use

24. In the context of STL allocators, what does the deallocate function do?

- [ ] a). Constructs an object in the allocated memory
- [ ] b). Destroys an object in the allocated memory
- [ ] c). Allocates a block of memory
- [ ] d). Frees a block of memory
    Correct Answer: D) Frees a block of memory

25. Which of the following operations is not typically part of a custom allocator?

- [ ] a). allocate
- [ ] b). construct
- [ ] c). reallocate
- [ ] d). deallocate
    Correct Answer: C) reallocate

26. What is the purpose of the construct function in a custom allocator?

- [ ] a). To allocate memory for an object
- [ ] b). To deallocate memory
- [ ] c). To construct an object in a pre-allocated memory block
- [ ] d). To perform a deep copy of an object
    Correct Answer: C) To construct an object in a pre-allocated memory block

27. Which of the following is a valid reason to implement a custom allocator in C++?

- [ ] a). To enforce coding standards
- [ ] b). To optimize the performance of dynamic memory allocation
- [ ] c). To avoid using exceptions
- [ ] d). To simplify the syntax of STL containers
    Correct Answer: B) To optimize the performance of dynamic memory allocation

28. What is the significance of the value_type typedef in a custom allocator?

- [ ] a). It defines the type of values that the allocator will allocate
- [ ] b). It specifies the return type of the allocate function
- [ ] c). It is used to determine the size of memory allocation
- [ ] d). It enforces type safety in the allocator
    Correct Answer: A) It defines the type of values that the allocator will allocate

29. Which of the following describes a scenario where a custom allocator would be particularly useful?

- [ ] a). Managing small, frequently allocated objects
- [ ] b). Storing elements in sorted order
- [ ] c). Ensuring exception safety
- [ ] d). Improving the readability of code
    Correct Answer: A) Managing small, frequently allocated objects

30. How can a custom allocator be used with an STL container?

- [ ] a). By passing the allocator as an argument to the container's constructor
- [ ] b). By overriding the container's default allocator
- [ ] c). By including the allocator header in the container's implementation
- [ ] d). By specifying the allocator as a template argument to the container
    Correct Answer: D) By specifying the allocator as a template argument to the container

Section 4: Additional Topics
31. What does SFINAE stand for?

- [ ] a). Static Function Inlining Not Allowed Ever
- [ ] b). Substitution Failure Is Not An Error
- [ ] c). Standard Function Implementation Needs Allocation Estimation
- [ ] d). Special Function Inlining Necessary After Expansion
    Correct Answer: B) Substitution Failure Is Not An Error

32. In which scenario is SFINAE most commonly used?

- [ ] a). To optimize memory usage in STL containers
- [ ] b). To conditionally enable template function overloads
- [ ] c). To ensure exception safety in STL algorithms
- [ ] d). To enforce the use of custom allocators
    Correct Answer: B) To conditionally enable template function overloads

33. Which header file is typically required when using SFINAE in C++?

- [ ] a). <algorithm>
- [ ] b). <type_traits>
- [ ] c). <functional>
- [ ] d). <iterator>
    Correct Answer: B) <type_traits>

34. What does std::enable_if do in the context of SFINAE?

- [ ] a). It disables a template specialization if a condition is met
- [ ] b). It enables a template function only if a condition is met
- [ ] c). It throws an exception if a condition is not met
- [ ] d). It allows a function to be compiled only if it has no side effects
    Correct Answer: B) It enables a template function only if a condition is met

35. Which of the following is an example of a type trait in C++?

- [ ] a). std::is_integral
- [ ] b). std::find_if
- [ ] c). std::partial_sum
- [ ] d). std::enable_if
    Correct Answer: A) std::is_integral

36. What is the purpose of std::is_same in C++?

- [ ] a). To determine if two objects are the same instance
- [ ] b). To compare two containers for equality
- [ ] c). To check if two types are the same
- [ ] d). To enforce type safety in STL algorithms
    Correct Answer: C) To check if two types are the same

37. How can you check if a type is an integral type using type traits?

- [ ] a). std::is_integral<T>::value
- [ ] b). std::is_same<T, int>::value
- [ ] c). std::is_type<T>::integral
- [ ] d). std::is_fundamental<T>::value
    Correct Answer: A) std::is_integral<T>::value

38. What is the role of type traits in template metaprogramming?

- [ ] a). To determine memory allocation sizes
- [ ] b). To enforce coding standards
- [ ] c). To perform compile-time checks on types
- [ ] d). To simplify function overloading
    Correct Answer: C) To perform compile-time checks on types

39. Which C++ feature introduced in C++11 is essential for writing concurrent programs using STL?

- [ ] a). Move semantics
- [ ] b). Lambda expressions
- [ ] c). Rvalue references
- [ ] d). std::thread
    Correct Answer: D) std::thread

40. What is the purpose of std::mutex in C++?

- [ ] a). To synchronize access to shared resources in a concurrent program
- [ ] b). To allocate memory dynamically
- [ ] c). To enforce type safety in template functions
- [ ] d). To perform I/O operations safely
    Correct Answer: A) To synchronize access to shared resources in a concurrent program

41. How does std::lock_guard help in managing concurrency in C++?

- [ ] a). By automatically acquiring and releasing a std::mutex
- [ ] b). By locking a thread to a specific CPU core
- [ ] c). By delaying the execution of a thread
- [ ] d). By ensuring that a function can only be called once
    Correct Answer: A) By automatically acquiring and releasing a std::mutex

42. Which of the following STL containers are thread-safe for concurrent read and write operations?

- [ ] a). std::vector
- [ ] b). std::deque
- [ ] c). std::set
- [ ] d). None of the above
    Correct Answer: D) None of the above

43. What is the output of the following code snippet?

cpp

#include <iostream>
#include <vector>
#include <thread>
#include <mutex>

std::mutex mtx;

void print_numbers(const std::vector<int>& vec) {
    std::lock_guard<std::mutex> lock(mtx);
    for (int n : vec) std::cout << n << " ";
    std::cout << std::endl;
}

int main() {
    std::vector<int> vec = {1, 2, 3, 4, 5};
    std::thread t1(print_numbers, std::ref(vec));
    std::thread t2(print_numbers, std::ref(vec));
    t1.join();
    t2.join();
    return 0;
}

- [ ] a). 1 2 3 4 5 1 2 3 4 5
- [ ] b). 1 2 3 4 5
- [ ] c). Undefined behavior
- [ ] d). 1 1 2 2 3 3 4 4 5 5
    Correct Answer: A) 1 2 3 4 5 1 2 3 4 5

44. What is the primary purpose of std::atomic in C++?

- [ ] a). To optimize memory usage
- [ ] b). To ensure that operations on a variable are performed atomically in a concurrent environment
- [ ] c). To perform mathematical operations on STL containers
- [ ] d). To allocate memory in small blocks
    Correct Answer: B) To ensure that operations on a variable are performed atomically in a concurrent environment

45. What is a race condition in concurrent programming?

- [ ] a). When two threads complete at the same time
- [ ] b). When two threads try to access the same resource simultaneously without proper synchronization
- [ ] c). When a thread is blocked indefinitely
- [ ] d). When threads are executed in a round-robin fashion
    Correct Answer: B) When two threads try to access the same resource simultaneously without proper synchronization

46. How can race conditions be prevented in C++?

- [ ] a). By using std::thread to create threads
- [ ] b). By using std::vector to store shared data
- [ ] c). By using mutexes and locks to synchronize access to shared resources
- [ ] d). By using lambda expressions to define thread functions
    Correct Answer: C) By using mutexes and locks to synchronize access to shared resources

47. What is the effect of calling std::thread::join()?

- [ ] a). It waits for the thread to finish execution
- [ ] b). It terminates the thread immediately
- [ ] c). It pauses the thread execution
- [ ] d). It detaches the thread from the main program
    Correct Answer: A) It waits for the thread to finish execution
