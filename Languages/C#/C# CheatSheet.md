# C# Cheat Sheet
### Initialization 
```C#
int i = 7;
byte b = 255;
String s = “My Blog”;
char c = ‘M’;
const String MYNAME = "Tuan";
```
### Operators 
| Operator | Description | 
| ------- | -------------|
| &&      | Logical AND | 
| ll      | Logical OR | 
| sizeof()| returns the size of a data type | 
| typeof()| returns the type of object | 

### String Data type conversion 
| Property    | Description | Example |
| ------------| ------------- |-------|
| IsFixedSize | Checks whether the Array has a fixed size | int[] numArray = new int[]{1,2,3};<br>numArray.IsFixedSize; |
| IsReadOnly  | Checks whether the Array is read-only| numArray.IsReadOnly; |
| IsSynchronized | check thread safe | numArray.IsSynchronized; |
| Length      | Gets the total number of elements <br>in all the dimensions of the Array | numArray.Length; |
| LongLength  | Length in 64-bit integer | numArray.LongLength; |
| Rank        | Gets the number of dimensions | numArray.Rank; |
| AsReadOnly()| Returns a read-only wrapper for the specified array | Array.AsReadOnly(numArray) |
| BinarySearch() | Searches a value in a one-dimensional<br>sorted array using a binary search algorithm | Array.BinarySearch(numArray, obj); |
| Clear()     | The elements at position 0 to 2 will be set<br>to default value after doing Clear() | Array.Clear(numArray, 0, 2) |
| Clone()     | Create a showllow copy of the Array | Array.Clone(numArray); |
| COnstrainedCopy() | Copies a range of elements (4) from numArr<br>starting at index 0 to newArr starting at index 2 | Array.ConstrainedCopy(numArr, 0, newArr, 2, 4); |
| Copy()       | Copies the first range of elements to newArr | Array.Copy(numArr, newArr, 5) |
| CopyTo()     | Copies all elements to newArr <br>starting at a certain index | Array.CopyTo(newArr, 3) |
| CreateInstance() | Intializes a new instance of the Array class | Array.CreateInstance(typeof(String), length); |
| Empty        | Returns an empty array | numArray.Empty(); |
| Equals()     | Determines whether the specified object<br>is equal to the current object | numArr.Equals(newArray); |
| Exists()     | Determine if a element if it matches given condition | Array.Exist(numArr, 5); |
| Find()       | Searchs for an element and returns the first<br>occurence within the array | Array.Find(numArr, n=>n>5 ); |
| FindAll()    | Returns an array containing all elements that<br>match the condition | Array.FindAll(numArr, n=>n>5 ); |
| FindIndex()  | Returns the index of the first occurrence | Array.FindIndex(numArr, n=>n>5 |
| ForEach()    | Loops through each element of the array and <br>performs the specified action | Array.ForEach(numArr, Action); |
| IndexOf()    | Searches for the specified object and<br>returns the index of its first occurence | numArr.IndexOf(5); |
| Resize()     | Changes the original length of the array | Array.resize(ref arrVal, len-5); |
| Reverse()    | Reverses the order of the elements in the array | numArr.Reverse(); |
| ToString()   | Returns a string that represents the current object | numArr.ToString(); |
| TrueForAll   | Checks whther every element matches the condition | Array.TrueForAll(numArr, n=>n>5); |

### String Data type conversion 
| Method      | Description | Example |
| ------------- | ------------- |-------|
| AsInt()<br>IsInt()  | Convert string into integer <br>Check if the string is int  | intVal = str.AsInt() <br>str.IsInt();
| Other methods  | AsFloat(), IsFloat, AsDecimal(), IsDecimal(), <br> AsDateTime(), IsDateTime(), AsBool(), IsBool() | Same as above pattern;
| ToString() | Convert another data type into String |myVal = 1111;<br> strVal = myVal.ToString();|

### Tuples
Uses a tuple to return multiple values from a method
```C#
public Tuple < int, string, string > GetEmployee()
{
    int employeeId = 1001;
    string firstName = "Rudy";
    string lastName = "Koertson";

    return Tuple.Create(employeeId, firstName, lastName);
}
```
