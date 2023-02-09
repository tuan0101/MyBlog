
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

### Vector
Vector has built-in function .resize(n);
When passing a vector to a function, it's memory will be automatically released after exit that function => an array will not, if early return before delete the array.

```c++
    int n = 10;
    vector<int> a(n);
    vector<int> b(n);
    for (auto &key : a) key = rand()%10;    // work directly on a,
    for (auto key : b) key = rand()%10;     // create a copy of b
    for (int i = 0; i < n; i++) cout << a[i];  //=> a is changed   9,3,4,1,...
    cout << endl;
    for (int i = 0; i < n; i++) cout << b[i];  // b is not changed, 0,0,0,...
    
    a.push_back(4);         // add 4 at the end
    a.pop_back();           // remove the last element
    a.back();               // return the last element
```
