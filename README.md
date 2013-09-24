#C++ Sorting Algorithm implementation

A collection of Sorting Algorithm implemented in C++11. See the `develop` branch for latest version.


##Insertion Sort
An adapted Bubble Sort that alternates between forward and backward passes.

|http://en.wikipedia.org/wiki/Insertion_sort|stable|
|----|---|
|Worst case performance              |O(n2) comparisons, swaps|
|Best case performance               |O(n) comparisons, O(1) swaps|
|Average case performance            |O(n2) comparisons, swaps|
|Worst case space complexity         |O(n) total, O(1)|

##Introsort
Introsort is a hybrid sorting algorithm that uses Quick Sort to a recursion depth of O(log n) and then switches to a Heap Sort. Heap Sort is implemented using the standard C++ functions `make_heap` and `sort_heap`, both of which require Random Access data iterators. For maximum flexibility, this implementation of Introsort does not switch to Heap Sort if the data iterators are not Random Access, and can therefore operator on container with any iterator category.

|http://en.wikipedia.org/wiki/Introsort|unstable|
|----|---|
|Worst case performance              |O(n log n)|
|Average case performance            |O(n log n)|

###Merge Sort
|http://en.wikipedia.org/wiki/Mergesort|stable|
|----|---
|Worst case performance              |O(n log n)
|Best case performance               |O(n log n) typical, O(n) natural variant
|Average case performance            |O(n log n)
|Worst case space complexity         |O(n) auxiliary


###Heap Sort
|http://en.wikipedia.org/wiki/Heapsort|unstable|
|----|---
|Worst case performance              |O(n log n)
|Best case performance               |Omega(n), O(n log n)
|Average case performance            |O(n log n)
|Worst case space complexity         |O(n) total, O(1) auxiliary

###Quick Sort
|http://en.wikipedia.org/wiki/Quicksort|unstable|
|----|---
|Worst case performance              |O(n2) (extremely rare)
|Best case performance               |O(n log n)
|Average case performance            |O(n log n)
|Worst case space complexity         |O(n) auxiliary (naive) O(log n) auxiliary (Sedgewick 1978)

###Bubble Sort
|http://en.wikipedia.org/wiki/Bubble_sort|stable|
|----|---
|Worst case performance              |O(n^2)
|Best case performance               |O(n)
|Average case performance            |O(n^2)
|Space                               |O(1)

###Selection Sort
|http://en.wikipedia.org/wiki/Selection_sort|stable|
|----|---
|Worst case performance              |O(n^2)
|Best case performance               |O(n)
|Average case performance            |O(n^2)
|Space                               |O(1)

###Min Max Sort
An adapted Selection Sort that finds and repositions the Min and Max elements on each pass.

|----|---
|Worst case performance              |O(n^2)
|Best case performance               |O(n)
|Average case performance            |O(n^2)
|Space                               |O(1)

###Cocktail Sort
|http://en.wikipedia.org/wiki/Cocktail_sort|stable|
|----|---
|Worst case performance              |O(n^2)
|Best case performance               |O(n)
|Average case performance            |O(n^2)
|Space                               |O(1)
