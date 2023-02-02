# C++ vs Java

### Operators 
| C++ | Java | 
| ------- | -------------|
| class Bar{}; | class Bar{} |
| Bar::DoStuff(); | Bar.DoStuff(); // static class |
| Bar y; // on the stack    |  alwasy allocated on the heap   |
| Bar *x = new Bar; // on the heap     |   Bar x = new Bar();  |
| y.my_field    |  y.my_field   |
| x->my_field  |  |
| references are immutable, use pointers for more flexibility | references are mutable and store addresses only to objects |
| int a = 7; int& b = a |  |
| virtual int foo();  | Java functions are virtual by default; use final to prevent overriding  |
| A class is turned to **abstract** if it includes a pure virtual function |  |
| class Bar { public: virtual void foo() = 0; };  |  abstract class Bar { public abstract void foo(); }  |
|  int *x = NULL | MyClass x = null;   |
| bool foo;  | boolean foo;  |
| const int R = 10  | final int R = 10   |
| **Arrays**  |   |
| int x[10];  |   |
| int *x = new x[10]  |  int[] x = new int[10]; |
| delete[] x; // reclaim memory  | memory reclaimed by the garbage collector  |


###  Collections and Iteration 
#### C++
Iterators are members of classes. The start of a range is <container>.begin(), and the end is <container>.end(). Advance using ++ operator, and access using *.
```C++
    vector myVec;
    for ( vector<int>::iterator itr = myVec.begin();
          itr != myVec.end();
          ++itr )
    {
        cout << *itr;
    }
```
#### Java
Iterator is just an interface. The start of the range is <collection>.iterator, and you check to see if you're at the end with itr.hasNext(). You get the next element using itr.next() (a combination of using ++ and * in C++).
```Java
    ArrayList myArrayList = new ArrayList();
    for( Object o : myArrayList ) {
        System.out.println( o );
    }
```

