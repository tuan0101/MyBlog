Whenever a child class overide a method from a parent class, we call it polymorphism. Eventhough they are closely related, but behave differently when calling the same method.

```Java
public class Animal{
  public void communicate(){
    System.out.println("communication");
  }
}

public class Dog extends Animal{
  public void communicate(){ // **overriding**
    System.out.println("gau gau");
  }
  public void communicate(string s){ // exactly method name but different parameters: **overlapping**
    System.out.println("gau gau", + s);
  }
}

public class Cat extends Animal{
  public void speak-communicate(){
    System.out.println("meow meow");
  }
}
```
