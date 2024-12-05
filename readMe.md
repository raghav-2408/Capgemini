# Capgemini - Get The Future You Want

### Capgemini SE is a French multinational information technology (IT) services and consulting company, headquartered in Paris, France.[3]

### Generative AI in cybersecurity

### What is Java?
Java is a programming language and a platform. Java is a high level, robust, object-oriented and secure programming language.

Java was developed by Sun Microsystems (which is now the subsidiary of Oracle) in the year 1995. James Gosling is known as the father of Java. Before Java, its name was Oak. Since Oak was already a registered company, so James Gosling and his team changed the name from Oak to Java.


# What is Java?

Java is a **high-level, object-oriented programming language** widely used for building various applications, including mobile apps, web applications, and enterprise systems. It was developed by **Sun Microsystems** in 1995 and is now owned by **Oracle Corporation**.

## Key Features of Java
1. **Platform Independence**:
   - Java is "write once, run anywhere" (WORA), meaning programs written in Java can run on any device or platform with the Java Virtual Machine (JVM).

2. **Object-Oriented**:
   - Supports features like classes, objects, inheritance, polymorphism, and encapsulation, enabling modular and reusable code.

3. **Robust and Secure**:
   - Includes strong memory management, exception handling, and a security manager for running untrusted code safely.

4. **Multi-threaded**:
   - Enables concurrent execution of multiple threads, making it ideal for tasks that can run in parallel.

5. **Rich API and Libraries**:
   - Provides a vast collection of libraries for tasks like data structures, networking, database connectivity, and GUI development.

6. **Garbage Collection**:
   - Automatically manages memory by reclaiming unused objects through a garbage collector.

## Common Uses of Java
- **Web Development**: Frameworks like Spring and Hibernate.
- **Android App Development**: A primary language for Android development.
- **Enterprise Applications**: Used for large-scale systems with Java EE.
- **Scientific Applications**: Known for stability and scalability.

Java is one of the most popular programming languages due to its **stability, platform independence, and extensive community support**, making it an excellent choice for beginners and experienced developers alike.


# Access Modifiers in Java

Access modifiers in Java are keywords that define **how accessible a class, method, or variable is** from other parts of your program. They control the visibility of the code and help protect it from being accessed or modified unintentionally.

## Types of Access Modifiers
1. **Public**:
   - **Accessible everywhere** in the program.
   - If a class, method, or variable is marked as `public`, it can be accessed from any other class.
   - Example:
     ```java
     public class MyClass {
         public int value = 10;
     }
     ```

2. **Private**:
   - **Accessible only within the same class**.
   - If a method or variable is `private`, it cannot be accessed directly from outside the class.
   - Example:
     ```java
     public class MyClass {
         private int value = 10;
     }
     ```

3. **Protected**:
   - **Accessible within the same package and subclasses**.
   - It allows access to inherited classes even if they are in a different package.
   - Example:
     ```java
     public class MyClass {
         protected int value = 10;
     }
     ```

4. **Default (Package-Private)**:
   - **Accessible only within the same package**.
   - If no access modifier is specified, the default access level is applied.
   - Example:
     ```java
     class MyClass {
         int value = 10; // No access modifier = default
     }
     ```

## Summary Table of Access Levels
| Modifier    | Same Class | Same Package | Subclass | Other Packages |
|-------------|------------|--------------|----------|----------------|
| `public`    | ✔️         | ✔️           | ✔️       | ✔️             |
| `protected` | ✔️         | ✔️           | ✔️       | ❌             |
| (default)   | ✔️         | ✔️           | ❌       | ❌             |
| `private`   | ✔️         | ❌           | ❌       | ❌             |

Access modifiers are essential for **data security, encapsulation, and structuring your code** in Java.


# Object-Oriented Programming (OOP) in Java

Object-Oriented Programming (OOP) is a programming style that uses **objects** and **classes** to structure software. It helps in organizing complex programs into smaller, manageable parts. Java is an object-oriented language, meaning it uses OOP principles to structure and organize code. These principles help make code more modular, reusable, and easier to maintain.

## Key Concepts of OOP in Java

### 1. **Class**
   - A **class** is like a blueprint or template for creating objects. It defines **properties** (variables) and **methods** (functions) that the objects created from it will have.
   - **Real-time Application**: Think of a `Car` class in a car manufacturing system. The class defines common properties like `color`, `model`, and methods like `drive()` or `stop()`.
   
   ```java
   public class Car {
       String color;
       String model;
       int speed;

       void drive() {
           System.out.println("Car is driving");
       }
   }
```

# 2. Object
An object is an instance of a class. It is a real, tangible entity that holds actual values for the class's properties and can perform the behaviors defined by the class.
Real-time Application: If you create an object of the Car class, it will represent a specific car, like a particular car in a car dealership, with actual attributes and methods.
```java
public class Main {
    public static void main(String[] args) {
        Car myCar = new Car(); // Creating an object of the Car class
        myCar.color = "Red";    // Setting properties
        myCar.model = "Tesla";  
        myCar.drive();          // Calling a method
    }
}
```
In this example, myCar is an object of the Car class with actual values (Red, Tesla).
# 3. Inheritance
Inheritance allows a class (child class) to inherit the properties and behaviors (methods) of another class (parent class). It enables code reuse.
Real-time Application: In a school system, a Teacher class and a Student class could both inherit from a Person class, sharing common attributes like name and age, but each class can also have its unique properties like subject for Teacher and grade for Student.
```java
class Person {
    String name;
    int age;

    void walk() {
        System.out.println(name + " is walking.");
    }
}

class Teacher extends Person {
    String subject;
}

class Student extends Person {
    int grade;
}
```
The Teacher and Student classes inherit common attributes like name and age from the Person class.
# 4. Polymorphism
Polymorphism means "many forms." It allows one method to have different behaviors based on the object that is calling it. It can be achieved through method overriding and method overloading.
Real-time Application: In a graphic design application, a Shape class could have different types of shapes like Circle, Rectangle, and Triangle. Each shape would have a draw() method that behaves differently for each shape.
```java
class Shape {
    void draw() {
        System.out.println("Drawing a shape.");
    }
}

class Circle extends Shape {
    @Override
    void draw() {
        System.out.println("Drawing a circle.");
    }
}

class Rectangle extends Shape {
    @Override
    void draw() {
        System.out.println("Drawing a rectangle.");
    }
}
```
Here, the draw() method behaves differently depending on the type of shape (circle or rectangle).
# 5. Encapsulation
Encapsulation is the concept of hiding the internal details of an object and exposing only the necessary parts. It is achieved by using private variables and public methods (getters and setters) to access or modify them.
Real-time Application: In a banking system, the balance of a bank account should not be accessed directly. Instead, the balance is hidden, and methods like deposit() and withdraw() are used to modify it, ensuring controlled access.
```java
class BankAccount {
    private double balance; // private variable

    public double getBalance() { // getter method
        return balance;
    }

    public void deposit(double amount) { // setter method
        if(amount > 0) {
            balance += amount;
        }
    }
}
```
Here, balance is private, and it can only be modified using the deposit() method.
# 6. Abstraction
Abstraction involves hiding the complex implementation details and exposing only the essential features. This is achieved through abstract classes and interfaces.
Real-time Application: In a remote control system, the remote control may have buttons for turning the TV on/off, changing the volume, etc., but the internal working of these buttons is hidden from the user.
```java
abstract class Vehicle {
    abstract void start();
}

class Car extends Vehicle {
    @Override
    void start() {
        System.out.println("Car started.");
    }
}

class Bike extends Vehicle {
    @Override
    void start() {
        System.out.println("Bike started.");
    }
}
```
In this case, the Vehicle class is abstract and hides the actual start mechanism, leaving it to the subclasses like Car or Bike to implement it.
Real-time Applications of OOP Principles
- E-commerce Websites: Classes like Product, Customer, and Order represent different entities. Inheritance and polymorphism allow flexible management of different product types and user roles.
- Banking Systems: Encapsulation ensures that sensitive data like account balances are hidden, while methods like withdraw() or deposit() control access.
- Gaming Software: Classes like Player, Enemy, and Level are used, and polymorphism allows different enemies to react differently when interacting with the player.
- Inventory Management: Inheritance helps organize product categories, and polymorphism allows various inventory items (like Electronics or Furniture) to have different behaviors.
### Conclusion
OOP in Java helps in organizing and structuring code in a way that models real-world entities. By using classes, objects, inheritance, polymorphism, encapsulation, and abstraction, developers can build efficient, scalable, and maintainable systems.


# Simple Applications of OOP in Java

Object-Oriented Programming (OOP) helps in structuring real-world problems using **objects** and **classes**. Here are simple examples of how OOP principles are applied in everyday scenarios.

## 1. **Class and Object**

   - **Real-life Example**: Think of a **Library System**.
     - A **class** in this case would be `Book`, which defines common properties such as `title`, `author`, and `ISBN`. These properties are the **attributes** of the book. 
     - An **object** is a specific book in the library, such as "Java Basics by John Doe", which has concrete values for these attributes.
     - Each book object in the library would be created from the `Book` class, which acts as a blueprint for all the books.

## 2. **Inheritance**

   - **Real-life Example**: Imagine a **Zoo System**.
     - The `Animal` class can be the base class with properties like `name` and `age` that all animals share.
     - Different animal types like `Lion` or `Elephant` can inherit from the `Animal` class and have their own specific properties, such as `maneColor` for the Lion or `trunkLength` for the Elephant.
     - This allows code to be reused. You don't need to rewrite common properties like `name` and `age` for every type of animal.

## 3. **Polymorphism**

   - **Real-life Example**: Think of a **Shape Drawing Application**.
     - A `Shape` class could define a `draw()` method, but different shapes (like `Circle`, `Square`, and `Triangle`) will have different ways to draw themselves.
     - Polymorphism allows the program to call the `draw()` method without worrying about the exact shape. It will automatically choose the correct behavior based on the specific shape (circle, square, etc.).

## 4. **Encapsulation**

   - **Real-life Example**: Consider a **Bank Account System**.
     - The `Account` class will have private information such as the `balance` of the account.
     - Instead of allowing anyone to directly access or change the balance, the system will provide methods like `deposit()` and `withdraw()` to safely modify the balance.
     - This keeps sensitive data secure and ensures that the balance can only be updated in controlled ways.

## 5. **Abstraction**

   - **Real-life Example**: Think of a **TV Remote Control**.
     - The TV remote provides simple buttons like `Power On`, `Volume Up`, and `Channel Change`. The user doesn’t need to understand the complex electronics inside the TV; they just need to know how to use the remote to control it.
     - **Abstraction** hides the complexity of how things work (like how the remote signals the TV) and only shows the necessary functions (like pressing buttons).

## Conclusion

OOP principles like **class and object**, **inheritance**, **polymorphism**, **encapsulation**, and **abstraction** are widely used in everyday applications. They help to simplify complex systems, ensure data security, and enable code reuse, making software development more efficient and maintainable.


# Access Modifiers in Java

In Java, **access modifiers** control the visibility and accessibility of classes, methods, variables, and constructors. These modifiers determine whether other classes or components can access or modify the elements they are applied to. There are four types of access modifiers in Java:

## 1. **Public**
   - **Definition**: The `public` access modifier allows a class, method, variable, or constructor to be accessible from any other class, regardless of package.
   - **Real-time Example**: If you have a `Car` class in a public transportation app, a method like `startEngine()` can be `public` so that it can be called from anywhere in the application to start the car.
   
   **Use case**:
   - **Class**: Any class marked as `public` can be accessed from any other class in the project.
   - **Method**: A `public` method can be called from any other class.
   - **Variable**: A `public` variable can be accessed and modified from any class.

   ```java
   public class Car {
       public void startEngine() {
           System.out.println("Engine started.");
       }
   }
```


# 2. Private
- Definition: The private access modifier restricts access to the class, method, variable, or constructor only within the same class. No other class can access it.
- Real-time Example: In a banking system, a balance variable can be marked private to ensure that no other class can directly access or change the balance. It can only be modified through a public method like deposit().
### Use case:

- Class: You can't declare an entire class private, but inner classes can be private.
- Method/Variable: A private method or variable can only be accessed within the same class.
```java
Copy code
public class BankAccount {
    private double balance;  // Private variable

    public void deposit(double amount) { // Public method to modify private variable
        if (amount > 0) {
            balance += amount;
        }
    }
}
```
# 3. Protected
Definition: The protected access modifier allows access to the class, method, variable, or constructor within the same package or from subclasses (even if the subclass is in a different package).
Real-time Example: In a library system, you may have a Book class and a subclass Ebook. If the content of a book is protected, it can be accessed by other classes in the same package or subclasses like Ebook.
Use case:

Class: A protected class can be accessed only within the same package or by subclasses.
Method/Variable: A protected method or variable can be accessed within the same package or by subclasses, even if they are in different packages.
```java
Copy code
public class Book {
    protected String content;  // Protected variable

    public Book(String content) {
        this.content = content;
    }
}

public class Ebook extends Book {
    public Ebook(String content) {
        super(content);
    }

    public void displayContent() {
        System.out.println(content);  // Accessing protected variable from superclass
    }
}
```
# 4. Default (Package-Private)
Definition: If no access modifier is specified, the class, method, variable, or constructor is considered default. The access is restricted to within the same package only.
Real-time Example: In a school system, if there is a class called Student, and a method enroll() is used only by classes within the same package, you can leave it with no access modifier. It will only be accessible to other classes in the same package.
Use case:

Class: A class with no access modifier can only be accessed by other classes in the same package.
Method/Variable: Methods or variables with no modifier can be accessed within the same package only.
```java
Copy code
class Student {  // Default class (package-private)
    int rollNo;  // Default variable (package-private)

    void enroll() {  // Default method (package-private)
        System.out.println("Enrolled in the course.");
    }
}
```
# Summary of Access Modifiers
- Access Modifier	Same Class	Same Package	Subclass	Everywhere
- Public	Yes	Yes	Yes	Yes
- Private	Yes	No	No	No
- Protected	Yes	Yes	Yes	No
- Default	Yes	Yes	No	No
## Conclusion
Public: Accessible anywhere.
Private: Accessible only within the same class.
Protected: Accessible within the same package and by subclasses.
Default: Accessible only within the same package.
By using access modifiers, we can ensure the right level of access and maintain data security and encapsulation in Java programs.
