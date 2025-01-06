# lifes-skills

# OOPS(OBJECT-ORIENTED PROGRAMMING SYSTEM)

## INTRODUCTION:
As the name suggests, Object-Oriented Programming or Java OOPs concept refers to languages that use objects in programming, they use objects as a primary source to implement what is to happen in the code. Objects are seen by the viewer or user, performing tasks you assign.
Object means a real-world entity such as a pen, chair, table, computer, watch, etc. Object-Oriented Programming is a methodology to design a program using classes and objects. It simplifies software development and maintenance by providing some concepts:
   * Object
   * Class
   * Inheritance
   * Polymorphism
   * Abstraction
   * Encapsulation

---    
## Object
object is an instance of class.It has properties and behaviour EX:-car is an object it has both properties(datatypes) and behaviour(methods).

---
## Class
Collection of objects is called class. It is a logical entity.class is blueprint of an object.Class does not consume any space.It is imaginary and object is real.

---
## Inheritance
The child class acquiring all the properties and behaviors of a parent object, it is known as inheritance. It provides code reusability. It is used to achieve runtime polymorphism.There are 3 methods in overriden.special and inherited methods.The method which is in parent class and the body is modified then it is overriden.The method which is just inherited then it is inherited method.The methods which are not in parent class and written in child classes then it is specialized methods.
For overriding methods there are 3 rules:
* child class should maintain same access modifier as parent or greater.
* overriden methods should have same return type as parent.
* Return type should be different provided there should be "is-a" Relationship and are called co-variant return types.

---
## Polymorphism
If one task is performed in different ways, it is known as polymorphism. For example: to convince the customer differently, to draw something, for example, shape, triangle, rectangle, etc.
In Java, we use method overloading and method overriding to achieve polymorphism.
Another example can be to speak something; for example, a man can be husband,brother,boyfriend,son,son-in-law etc.
child object parent reference but the limitation is we can't directly access the specialized methods of child class.by downcasting we can achieve that.

---
## Abstraction
Hiding internal implementation and showing functionality only to the user is known as abstraction. For example, phone call, we do not know the internal processing.
In Java, we use abstract class and interface to achieve abstraction.
Abstract class consists Abstract methods.we can't create instance of abstract class.we can't give abstarct and final at a time because we can't inherit then class can't be completed.Abstract classes are not pure abstract classes.to achieve 100% abstraction we use interfaces.

---
## Encapsulation
Binding (or wrapping) code and data together into a single unit are known as encapsulation.providing sceurity for important part of an object.we use access modifiers for providing security. For example, a capsule, it is wrapped with different medicines.
A Java class is the example of encapsulation. Java bean is the fully encapsulated class because all the data members are private here.

---
## Advantage of OOPs over Procedure-Oriented Programming Language
* OOPs makes development and maintenance easier, whereas, in a procedure-oriented programming language, it is not easy to manage if code grows as project size increases.
*  OOPs provides data hiding, whereas, in a procedure-oriented programming language, global data can be accessed from anywhere.
*  Global Data OOPs provides the ability to simulate real-world event much more effectively. We can provide the solution of real word problem if we are using the Object-Oriented Programming language.

---
## What is the difference between an object-oriented programming language and object-based programming language?
Object-based programming language follows all the features of OOPs except Inheritance. JavaScript and VBScript are examples of object-based programming languages.

#### Java program for demonstrating the features and functionalities of OOPs concepts in Java.


Base class


``` elixir
 public class Animal {
     private String name;

    # Constructor  
    public Animal(String name) {  
        this.name = name;  
    }

   # Encapsulation: Getter method  
    public String getName() {  
        return name;  
    }  

    # Polymorphism: Overridden method  
    public void makeSound() {  
        System.out.println("Some sound");  
    }  
}

# Derived class (Inheritance): Dog
class Dog extends Animal {
    # Constructor
    public Dog(String name) {
        super(name);
    }

    # Polymorphism: Overriding method  
    @Override  
    public void makeSound() {  
        System.out.println("Woof");  
    }
}

# Derived class (Inheritance): Cat
class Cat extends Animal {
    # Constructor
    public Cat(String name) {
        super(name);
    }

    # Polymorphism: Overriding method  
    @Override  
    public void makeSound() {  
        System.out.println("Meow");  
    }
}

# Main class
public class OOPs {
    public static void main(String[] args) {
        # Creating objects of Dog and Cat classes
        Dog dog = new Dog("Buddy");
        Cat cat = new Cat("Whiskers");
        # Accessing methods of base class through objects of derived classes  
        System.out.println("Dog name: " + dog.getName());  
        dog.makeSound();  
        System.out.println("Cat name: " + cat.getName());  
        cat.makeSound();  
    }
} 



---
## References
* https://www.javatpoint.com/java-oops-concepts  (javat website)
* https://www.youtube.com/watch?v=BSVKUk58K6U&t=1362s (youtube link)
