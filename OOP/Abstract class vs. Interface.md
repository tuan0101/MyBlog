
### Comparisons 

| Abstract Classes | Interfaces | 
| ---------------- | -------------|
| is a superclass for all classes that sharing the same/similar nature  <br> Two classes implementing ONE interface can be completely different in nature (Type, attribute, method)   | Is a contract that you can sign whenever you want. <br> One class can have multiple interfaces | 
| Relationship between Class-Abstract Class is called "Is-a" (extend/inherit)      | Relationship between Class-Interface is "can-do" (implement)| 
| Does not support multiple inheritance| can implement multiple interfaces | 
| Can defined the implementation | Cannot |
| Can defined modifier | Modifier must be public |

![alt text](https://viblo.asia/uploads/0b503d7f-4e21-4447-a0a2-9ae31856df3c.png)

As you can see, both dog and car are capable of running, but they belong to two completely distinct categories. 
=> Regarding the use of an inteface, it can be understood as a third-party software. Implementing an interface for a class is like installing a plugin for a piece of software.
=> Abstract functions are only used to rewrite in subclasses so why not use ordinary class? The reason is that the abstract function must be overide in the subclass, otherwise it will report an error. It acts an instruction to make sure the subclass contains adequate functions (This is the same for abstract function in an interface).

Syntax:

Class Cat extends Animal{}  // Abstract Animal  
Class Cat implements Animal{} // interface Animal  

Abstract classes should be used primarily for objects that are closely related, bc it "extend" what already have, whereas interfaces are best suited for providing a common functionality to unrelated classes.
interface is just like a list of required action that programmers need to implement.

Related topic:  
What is "final method"?  
the key word "final" to indicate that the method cannot be overridden by subclasses.  

tip: add _._ 2 space at the end to break line in this github
