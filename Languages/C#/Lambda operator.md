#Lambda operator
The lambda operator ```=>``` separates the input parameters on the left side from the lambda body (usually an expression) on the right side.

example 1:
```C#
string[] words = { "banana", "apple", "apricot" };
int maxLength = words
  .Where(w => w.StartsWith("a"))
  .Max(w => w.Length);
Console.WriteLine(maxLength);   // output: 7
```

example 2:
```C#
List<int> numbers = new List<int>() {12, 15, 0, 1, 2};

var square = numbers.Select(x => x * x); 

// foreach loop to display squares 
Console.Write("Squares : ");
foreach(var value in square) 
{ 
    Console.Write("{0} ", value); 
} 
//output: Squares : 144 225 0 1 4 
```
