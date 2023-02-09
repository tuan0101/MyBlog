
### Dynamic Memory Allocation
```C++
int fixedArray[] {1, 2, 3}; // fixed size: 3
int *dynamicArray1 = new int[] {1, 2, 3}; // error
int *dynamicArray2 = new int[3] {1, 2, 3}; // ok
int *array = new int[10]; // dynamic array, 10 can be a variable
```
*array* is a pointer, and thus, the first element pointed to by *array* can be accessed either with the expression *array*[0] or the expression **array* (both are equivalent). The second element can be accessed either with *array*[1] or *(*array*+1), and so on...

One issue is you cannot resize the array directly, you have to create a new one and copy over.
To solve this issue, we have Vector.

###
