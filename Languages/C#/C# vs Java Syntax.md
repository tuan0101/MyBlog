# C# Cheat Sheet
```C#
int i = 7;
byte b = 255;
String s = “My Blog”;
char c = ‘M’;
const String MYNAME = "Tuan";
```
### Operators 
| C# | Java | 
| ------- | -------------|
| List<int> numbers = new List<__int__>();| List<__Integer__> numbers = new ArrayList<>(); | 
| numbers.__Add__(1)     | numbers.__add__(2)  | 
  | numbers.__Insert__(0, 2)     | numbers.__add__(0, 2) ```add 2 at index 0``` | 
| numbers.__Remove__(1)| numbers.__remove__(Integer.valueOf(1)) | 
| numbers.__RemoveAt__(1)| numbers.__remove__(1) |  
| -------------  |  ------------- |
| __foreach__ (int num __in__ numbers) |  for (int num : numbers) |
|  ------------- | -------------  |
| Dictionary<string, int> myMap = new Dictionary<string, int>();  |  HashMap<String, int> myMap = new HashMap<>(); |
| myMap.Add("diamond", 500);  | myMap.put("diamond", 500);  |
| myMap.TryGetValue("gold", out int value2);  |  myMap.getOrDefault("gold", "default_value");  |
| myMap.__ContainsKey__("diamond");  | myMap.__containsKey__("diamond"); |
| ------------- | -------------  |
|  HashSet<int> mySet = new HashSet<__int__>();  | HashSet<int> mySet = new HashSet<>();  |
| mySet.__Add__(100)  | mySet.__add__(100)  |
| mySet.__Contains__(100)  | mySet.__contains__(100)  |
