# Quiz: Memory management: Standard Template Library
## Programming with C++

---

### Commonly Used Standard Headers

1. **Which header file is used for input and output streams in C++?**
   - [ ] a). `<fstream>`
   - [ ] b). `<iostream>`
   - [ ] c). `<algorithm>`
   - [ ] d). `<string>`

2. **Which header file provides algorithms like `sort`, `copy`, etc.?**
   - [ ] a). `<numeric>`
   - [ ] b). `<functional>`
   - [ ] c). `<algorithm>`
   - [ ] d). `<vector>`

3. **Which header file is needed for using `accumulate` and `inner_product`?**
   - [ ] a). `<numeric>`
   - [ ] b). `<algorithm>`
   - [ ] c). `<functional>`
   - [ ] d). `<map>`

4. **Which STL algorithm is used to find the first occurrence of a value in a sequence?**
   - [ ] a). `find_if`
   - [ ] b). `sort`
   - [ ] c). `find`
   - [ ] d). `copy`

5. **How does the `find_if` algorithm differ from the `find` algorithm?**
   - [ ] a). `find_if` uses a predicate to find an element.
   - [ ] b). `find_if` finds the last occurrence of an element.
   - [ ] c). `find_if` sorts the elements before finding.
   - [ ] d). `find_if` copies elements that match a condition.

6. **What does the `sort` algorithm do?**
   - [ ] a). Finds the first occurrence of an element.
   - [ ] b). Sorts the elements in a sequence.
   - [ ] c). Copies elements from one sequence to another.
   - [ ] d). Counts the number of occurrences of an element.

7. **What is a predicate in the context of STL algorithms?**
   - [ ] a). A sequence container.
   - [ ] b). A function or function object that returns a bool.
   - [ ] c). A type of iterator.
   - [ ] d). A sorting algorithm.

8. **Which of the following is an example of a function object used as a predicate?**
   - [ ] a). `bool operator()(int i) const { return i%2; }`
   - [ ] b). `int operator()(int i, int j) const { return i+j; }`
   - [ ] c). `void operator()(int i) const { cout << i; }`
   - [ ] d). `string operator()(string s) const { return s; }`

9. **What is the main advantage of using function objects in STL algorithms?**
   - [ ] a). They are easier to write than functions.
   - [ ] b). They allow for inlining and can be more efficient.
   - [ ] c). They are mandatory for all STL algorithms.
   - [ ] d). They simplify the syntax of algorithms.

10. **Which standard header provides common function objects like `plus`, `minus`, `multiplies`, etc.?**
    - [ ] a). `<numeric>`
    - [ ] b). `<functional>`
    - [ ] c). `<algorithm>`
    - [ ] d). `<map>`

11. **What is the purpose of the `accumulate` algorithm?**
    - [ ] a). To find the first occurrence of an element.
    - [ ] b). To sum the elements of a sequence.
    - [ ] c). To sort the elements of a sequence.
    - [ ] d). To copy elements from one sequence to another.

12. **How can you use a custom binary operation with `accumulate`?**
    - [ ] a). By passing a function object as the fourth argument.
    - [ ] b). By overloading the `+` operator.
    - [ ] c). By using the `sort` algorithm.
    - [ ] d). By passing the initializer as the first argument.

### Inner Product

13. **What does the `inner_product` algorithm compute?**
    - [ ] a). The product of all elements in a sequence.
    - [ ] b). The dot product of two sequences.
    - [ ] c). The sum of all elements in a sequence.
    - [ ] d). The maximum element in a sequence.

14. **Which of the following correctly uses `inner_product`?**
    - [ ] a). `double result = inner_product(vec1.begin(), vec1.end(), vec2.begin(), 0.0);`
    - [ ] b). `double result = accumulate(vec1.begin(), vec1.end(), vec2.begin(), 0.0);`
    - [ ] c). `double result = sort(vec1.begin(), vec1.end(), vec2.begin(), 0.0);`
    - [ ] d). `double result = copy(vec1.begin(), vec1.end(), vec2.begin(), 0.0);`

### Copy and Copy_if

15. **What does the `copy` algorithm do?**
    - [ ] a). Finds the first occurrence of an element.
    - [ ] b). Copies elements from one sequence to another.
    - [ ] c). Sorts the elements in a sequence.
    - [ ] d). Counts the number of occurrences of an element.

16. **What is the difference between `copy` and `copy_if`?**
    - [ ] a). `copy_if` only copies elements that fulfill a predicate.
    - [ ] b). `copy_if` sorts the elements during copying.
    - [ ] c). `copy_if` copies elements in reverse order.
    - [ ] d). `copy_if` copies elements that do not fulfill a predicate.

17. **Which type of iterator can be used to write to an output stream?**
    - [ ] a). `istream_iterator`
    - [ ] b). `ostream_iterator`
    - [ ] c). `vector_iterator`
    - [ ] d). `list_iterator`

18. **How do you create an iterator to read from an input stream?**
    - [ ] a). `istream_iterator<string> ii(cout);`
    - [ ] b). `ostream_iterator<string> ii(cin);`
    - [ ] c). `istream_iterator<string> ii(cin);`
    - [ ] d). `vector_iterator<string> ii(cin);`

19. **Create a vector with 1000 random three-letter words. Use the `find` algorithm to search and count entries that have three equal letters. Which algorithm should be used?**
    - [ ] a). `find_if`
    - [ ] b). `sort`
    - [ ] c). `find`
    - [ ] d). `count_if`

20. **Create a set with 1000 random three-letter words. Use the `replace` algorithm to search words that start with the letter "a" and replace them by the same string but now starting with a 'z'. Which algorithm should be used?**
    - [ ] a). `find`
    - [ ] b). `sort`
    - [ ] c). `replace`
    - [ ] d). `count`

21. **What does the `unique_copy` algorithm do?**
    - [ ] a). Copies all elements from one sequence to another.
    - [ ] b). Copies elements but removes adjacent duplicates.
    - [ ] c). Sorts the elements while copying.
    - [ ] d). Copies elements but only keeps unique ones.

22. **What is the purpose of the `merge` algorithm?**
    - [ ] a). To combine two sorted sequences into one sorted sequence.
    - [ ] b). To find the intersection of two sequences.
    - [ ] c). To find the union of two sequences.
    - [ ] d). To remove duplicates from a sequence.

23. **What does the `equal_range` algorithm return?**
    - [ ] a). The first element that matches a value.
    - [ ] b). A pair of iterators defining the range of elements that match a value.
    - [ ] c). The last element that matches a value.
    - [ ] d). The count of elements that match a value.

24. **How does the `equal` algorithm compare two sequences?**
    - [ ] a). It checks if all elements in the first sequence are equal to the corresponding elements in the second sequence.
    - [ ] b). It sorts both sequences and then compares them.
    - [ ] c). It checks if any elements in the first sequence are equal to the corresponding elements in the second sequence.
    - [ ] d). It merges the two sequences and checks for equality.

25. **What is policy parameterization in the context of STL algorithms?**
    - [ ] a). The ability to use different data types in algorithms.
    - [ ] b). The ability to parameterize algorithms by a policy, such as a comparison criterion.
    - [ ] c). The ability to change the algorithm's behavior at runtime.
    - [ ] d). The ability to use functions and function objects interchangeably.

26. **Which algorithm would you use to sum the elements of a sequence?**
    - [ ] a). `inner_product`
    - [ ] b). `accumulate`
    - [ ] c). `count`
    - [ ] d). `equal`

27. **Which function object can be used with `accumulate` to compute the product of elements?**
    - [ ] a). `plus`
    - [ ] b). `minus`
    - [ ] c). `multiplies`
    - [ ] d). `divides`

28. **What does the `transform` algorithm do?**
    - [ ] a). It applies a function to each element of a sequence and stores the result in another sequence.
    - [ ] b). It sorts the elements of a sequence.
    - [ ] c). It merges two sequences into one.
    - [ ] d). It removes elements that do not satisfy a predicate.

29. **What is the purpose of the `partial_sum` algorithm?**
    - [ ] a). To compute the cumulative sum of elements in a sequence.
    - [ ] b). To find the sum of a subrange of elements.
    - [ ] c). To find the difference between consecutive elements.
    - [ ] d). To copy elements from one sequence to another.

30. **What does the `adjacent_difference` algorithm compute?**
    - [ ] a). The difference between each pair of adjacent elements in a sequence.
    - [ ] b). The sum of each pair of adjacent elements in a sequence.
    - [ ] c). The product of each pair of adjacent elements in a sequence.
    - [ ] d). The maximum difference between any two elements in a sequence.

31. **Write a function that uses `accumulate` to calculate the total price of items in a list of `Record` structs, where each `Record` has `units` sold and `unit_price`. What should be passed as the binary operation in `accumulate`?**
    - [ ] a). `plus<double>`
    - [ ] b). `multiplies<double>`
    - [ ] c). A custom function that multiplies `units` by `unit_price` and adds to the total.
    - [ ] d). A custom function that adds `units` and `unit_price`.

32. **Using the `inner_product` algorithm, calculate the Dow-Jones industrial index given vectors of share prices and weights. Which binary operations are used by default?**
    - [ ] a). `plus` for addition and `multiplies` for multiplication.
    - [ ] b). `minus` for subtraction and `divides` for division.
    - [ ] c). `multiplies` for multiplication and `plus` for addition.
    - [ ] d). `divides` for division and `minus` for subtraction.

### 

33. **What is the main reason to use STL algorithms instead of writing custom loops?**
    - [ ] a). STL algorithms are more efficient.
    - [ ] b). STL algorithms are easier to read and maintain.
    - [ ] c). STL algorithms are optimized and well-tested.
    - [ ] d). All of the above.

34. **Which of the following is not an STL algorithm?**
    - [ ] a). `accumulate`
    - [ ] b). `inner_product`
    - [ ] c). `sort`
    - [ ] d). `print`

35. **What does the `for_each` algorithm do?**
    - [ ] a). Applies a function to each element in a sequence.
    - [ ] b). Sorts the elements in a sequence.
    - [ ] c). Finds the first element that satisfies a condition.
    - [ ] d). Copies elements from one sequence to another.

36. **How can you ensure that an STL algorithm works with different container types?**
    - [ ] a). By using iterators.
    - [ ] b). By using pointers.
    - [ ] c). By using the `auto` keyword.
    - [ ] d). By using templates.

### Answers

1. b) `<iostream>`
2. c) `<algorithm>`
3. a) `<numeric>`
4. c) `find`
5. a) `find_if` uses a predicate to find an element.
6. b) Sorts the elements in a sequence.
7. b) A function or function object that returns a bool.
8. a) `bool operator()(int i) const { return i%2; }`
9. b) They allow for inlining and can be more efficient.
10. b) `<functional>`
11. b) To sum the elements of a sequence.
12. a) By passing a function object as the fourth argument.
13. b) The dot product of two sequences.
14. a) `double result = inner_product(vec1.begin(), vec1.end(), vec2.begin(), 0.0);`
15. b) Copies elements from one sequence to another.
16. a) `copy_if` only copies elements that fulfill a predicate.
17. b) `ostream_iterator`
18. c) `istream_iterator<string> ii(cin);`
19. c) `find`
20. c) `replace`
21. b) Copies elements but removes adjacent duplicates.
22. a) To combine two sorted sequences into one sorted sequence.
23. b) A pair of iterators defining the range of elements that match a value.
24. a) It checks if all elements in the first sequence are equal to the corresponding elements in the second sequence.
25. b) The ability to parameterize algorithms by a policy, such as a comparison criterion.
26. b) `accumulate`
27. c) `multiplies`
28. a) It applies a function to each element of a sequence and stores the result in another sequence.
29. a) To compute the cumulative sum of elements in a sequence.
30. a) The difference between each pair of adjacent elements in a sequence.
31. c) A custom function that multiplies `units` by `unit_price` and adds to the total.
32. a) `plus` for addition and `multiplies` for multiplication.
33. d) All of the above.
34. d) `print`
35. a) Applies a function to each element in a sequence.
36. a) By using iterators.
