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
| Method      | Description | Example |
| ------------- | ------------- |-------|
| AsInt()<br>IsInt()  | Convert string into integer <br>Check if the string is int  | intVal = str.AsInt() <br>str.IsInt();
| Other methods  | AsFloat(), IsFloat, AsDecimal(), IsDecimal(), <br> AsDateTime(), IsDateTime(), AsBool(), IsBool() | Same as above pattern;
| ToString() | Convert another data type into String |myVal = 1111;<br> strVal = myVal.ToString();|
