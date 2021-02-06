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

example 3:
```C#
List<int> numbers = new List<int>() {12, 15, 0, 1, 2};
var divBy3 = numbers.FindAll(x => (x % 2) == 0); 

// foreach loop to display squares 
Console.Write("Numbers Divisible by 2 : ");
foreach(var value in divBy2) 
{ 
    Console.Write("{0} ", value); 
} 
//Numbers Divisible by 2 : 12 0 2
```

