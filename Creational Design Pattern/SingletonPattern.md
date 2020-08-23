#Singleton Pattern
##https://www.tutorialspoint.com/design_pattern/singleton_pattern.htm

- creational pattern
- only single object gets created of the class

```java
class Singleton 
{ 
    // static variable single_instance of type Singleton 
    private static Singleton single_instance=null; 
  
    // variable of type String 
    public String s; 
  
    // private constructor restricted to this class itself 
    private Singleton() 
    { 
        s = "Hello I am a string part of Singleton class"; 
    } 
  
    // static method to create instance of Singleton class 
    public static Singleton Singleton() 
    { 
        // To ensure only one instance is created 
        if (single_instance == null) 
        { 
            single_instance = new Singleton(); 
        } 
        return single_instance; 
    } 
} 
```