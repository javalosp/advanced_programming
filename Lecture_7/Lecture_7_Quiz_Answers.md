# Advanced Programming with C++
## Quiz: Standard Template Library

---

#### Which header file is used for input and output streams in C++?
- [ ] a). `<fstream>`
- [x] b). `<iostream>`
- [ ] c). `<algorithm>`
- [ ] d). `<string>`

#### Which header file provides algorithms like `sort`, `copy`, etc.?
- [ ] a). `<numeric>`
- [ ] b). `<functional>`
- [x] c). `<algorithm>`
- [ ] d). `<vector>`

#### Which header file is needed for using `accumulate` and `inner_product`?
- [x] a). `<numeric>`
- [ ] b). `<algorithm>`
- [ ] c). `<functional>`
- [ ] d). `<map>`

#### Which STL algorithm is used to find the first occurrence of a value in a sequence?
- [ ] a). `find_if`
- [ ] b). `sort`
- [x] c). `find`
- [ ] d). `copy`

#### How does the `find_if` algorithm differ from the `find` algorithm?
- [x] a). `find_if` uses a predicate to find an element.
- [ ] b). `find_if` finds the last occurrence of an element.
- [ ] c). `find_if` sorts the elements before finding.
- [ ] d). `find_if` copies elements that match a condition.

#### What does the `sort` algorithm do?
- [ ] a). Finds the first occurrence of an element.
- [x] b). Sorts the elements in a sequence.
- [ ] c). Copies elements from one sequence to another.
- [ ] d). Counts the number of occurrences of an element.

#### What is a predicate in the context of STL algorithms?
- [ ] a). A sequence container.
- [x] b). A function or function object that returns a bool.
- [ ] c). A type of iterator.
- [ ] d). A sorting algorithm.

#### Which of the following is an example of a function object used as a predicate?
- [x] a). `bool operator()(int i) const { return i%2; }`
- [ ] b). `int operator()(int i, int j) const { return i+j; }`
- [ ] c). `void operator()(int i) const { cout << i; }`
- [ ] d). `string operator()(string s) const { return s; }`

#### What is the main advantage of using function objects in STL algorithms?
- [ ] a). They are easier to write than functions.
- [x] b). They allow for inlining and can be more efficient.
- [ ] c). They are mandatory for all STL algorithms.
- [ ] d). They simplify the syntax of algorithms.


#### Which standard header provides common function objects like `plus`, `minus`, `multiplies`, etc.?
- [ ] a). `<numeric>`
- [x] b). `<functional>`
- [ ] c). `<algorithm>`
- [ ] d). `<map>`

#### What is the purpose of the `accumulate` algorithm?
- [ ] a). To find the first occurrence of an element.
- [x] b). To sum the elements of a sequence.
- [ ] c). To sort the elements of a sequence.
- [ ] d). To copy elements from one sequence to another.

#### How can you use a custom binary operation with `accumulate`?
- [x] a). By passing a function object as the fourth argument.
- [ ] b). By overloading the `+` operator.
- [ ] c). By using the `sort` algorithm.
- [ ] d). By passing the initializer as the first argument.

#### What does the `inner_product` algorithm compute?
- [ ] a). The product of all elements in a sequence.
- [x] b). The dot product of two sequences.
- [ ] c). The sum of all elements in a sequence.
- [ ] d). The maximum element in a sequence.

#### Which of the following correctly uses `inner_product`?
- [x] a). `double result = inner_product(vec1.begin(), vec1.end(), vec2.begin(), 0.0);`
- [ ] b). `double result = accumulate(vec1.begin(), vec1.end(), vec2.begin(), 0.0);`
- [ ] c). `double result = sort(vec1.begin(), vec1.end(), vec2.begin(), 0.0);`
- [ ] d). `double result = copy(vec1.begin(), vec1.end(), vec2.begin(), 0.0);`

#### What does the `copy` algorithm do?
- [ ] a). Finds the first occurrence of an element.
- [x] b). Copies elements from one sequence to another.
- [ ] c). Sorts the elements in a sequence.
- [ ] d). Counts the number of occurrences of an element.

#### What is the difference between `copy` and `copy_if`?
- [x] a). `copy_if` only copies elements that fulfill a predicate.
- [ ] b). `copy_if` sorts the elements during copying.
- [ ] c). `copy_if` copies elements in reverse order.
- [ ] d). `copy_if` copies elements that do not fulfill a predicate.

#### Which type of iterator can be used to write to an output stream?
- [ ] a). `istream_iterator`
- [ ] b). `ostream_iterator`
- [ ] c). `vector_iterator`
- [ ] d). `list_iterator`

#### Which algorithm should be used for searching and counting the entries in a vector of strings thath have three equal letters?
- [ ] a). `find_if`
- [ ] b). `sort`
- [x] c). `find`
- [ ] d). `count_if`

#### What does the `unique_copy` algorithm do?
- [ ] a). Copies all elements from one sequence to another.
- [x] b). Copies elements but removes adjacent duplicates.
- [ ] c). Sorts the elements while copying.
- [ ] d). Copies elements but only keeps unique ones.

#### What is the purpose of the `merge` algorithm?
- [x] a). To combine two sorted sequences into one sorted sequence.
- [ ] b). To find the intersection of two sequences.
- [ ] c). To find the union of two sequences.
- [ ] d). To remove duplicates from a sequence.

#### How does the `equal` algorithm compare two sequences?
- [x] a). It checks if all elements in the first sequence are equal to the corresponding elements in the second sequence.
- [ ] b). It sorts both sequences and then compares them.
- [ ] c). It checks if any elements in the first sequence are equal to the corresponding elements in the second sequence.
- [ ] d). It merges the two sequences and checks for equality.

#### Which algorithm would you use to sum the elements of a sequence?
- [ ] a). `inner_product`
- [x] b). `accumulate`
- [ ] c). `count`
- [ ] d). `equal`

#### Which function object can be used with `accumulate` to compute the product of elements?
- [ ] a). `plus`
- [ ] b). `minus`
- [x] c). `multiplies`
- [ ] d). `divides`

#### What does the `transform` algorithm do?
- [x] a). It applies a function to each element of a sequence and stores the result in another sequence.
- [ ] b). It sorts the elements of a sequence.
- [ ] c). It merges two sequences into one.
- [ ] d). It removes elements that do not satisfy a predicate.

#### What is the purpose of the `partial_sum` algorithm?
- [x] a). To compute the cumulative sum of elements in a sequence.
- [ ] b). To find the sum of a subrange of elements.
- [ ] c). To find the difference between consecutive elements.
- [ ] d). To copy elements from one sequence to another.

#### What should be passed as the binary operation in `accumulate` to calculate the total price of items in a list of `Record` structs, where each `Record` has `units` sold and `unit_price`?
- [ ] a). `plus<double>`
- [ ] b). `multiplies<double>`
- [x] c). A custom function that multiplies `units` by `unit_price` and adds to the total.
- [ ] d). A custom function that adds `units` and `unit_price`.

#### What is the main reason to use STL algorithms instead of writing custom loops?
- [ ] a). STL algorithms are more efficient.
- [ ] b). STL algorithms are easier to read and maintain.
- [ ] c). STL algorithms are optimized and well-tested.
- [x] d). All of the above.

#### Which of the following is not an STL algorithm?
- [ ] a). `accumulate`
- [ ] b). `inner_product`
- [ ] c). `sort`
- [x] d). `print`

#### What does the `for_each` algorithm do?
- [x] a). Applies a function to each element in a sequence.
- [ ] b). Sorts the elements in a sequence.
- [ ] c). Finds the first element that satisfies a condition.
- [ ] d). Copies elements from one sequence to another.

#### How can you ensure that an STL algorithm works with different container types?
- [x] a). By using iterators.
- [ ] b). By using pointers.
- [ ] c). By using the `auto` keyword.
- [ ] d). By using templates.

---