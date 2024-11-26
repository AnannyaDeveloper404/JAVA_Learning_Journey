# What is Java?

Java is a popular programming language, created in 1995.

It is owned by Oracle, and more than 3 billion devices run Java.

#### It is used for:

- Mobile applications (specially Android apps)
- Desktop applications
- Web applications
- Web servers and application servers
- Games
- Database connection
- And much, much more!

#### Why Use Java?

- Java works on different platforms **(Windows, Mac, Linux, Raspberry Pi, etc.)**
- It is one of the most popular programming languages in the world
- It has a large demand in the current job market
- It is easy to learn and simple to use
- It is open-source and free
- It is secure, fast and powerful
- It has huge community support (tens of millions of developers)
- Java is an object oriented language which gives a clear structure to programs and allows code to be reused, lowering development costs
- As Java is close to C++ and C#, it makes it easy for programmers to switch to Java or vice versa

```java
public class Main {
  public static void main(String[] args) {
    System.out.print("Hello World");
  }
}
```

## Java Output / Print

The `println()` method adds a line break after printing, while `print()` does not

```java
System.out.println("I am learning Java.");
System.out.println(50000);
```

## Java Variables

- **String** - stores text, such as "Hello". String values are surrounded by double quotes
- **int** - stores integers (whole numbers), without decimals, such as 123 or -123
- **float** - stores floating point numbers, with decimals, such as 19.99 or -19.99
- **char** - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes
- **boolean** - stores values with two states: true or false

## Java Type Casting

In Java, there are two types of casting:

Widening Casting (automatically) - converting a smaller type to a larger type size
`byte` -> `short` -> `char`-> `int` -> `long` -> `float` -> `double`

Narrowing Casting (manually) - converting a larger type to a smaller size type
`double` -> `float` -> `long` -> `int` -> `char `-> `short` -> `byte`

```java
public class Main {
  public static void main(String[] args) {
    int myInt = 9;
    double myDouble = myInt; // Automatic casting: int to double

    System.out.println(myInt);      // Outputs 9
    System.out.println(myDouble);   // Outputs 9.0
  }
}
```

## Java Strings

Strings are used for storing text.

A String variable contains a collection of characters surrounded by double quotes:

### More String Methods

There are many string methods available, for example `toUpperCase()` , `toLowerCase()`, `indexOf()`,`concat()`:

```java
// toUpperCase(), toLowerCase()
String txt = "Hello World";
System.out.println(txt.toUpperCase());   // Outputs "HELLO WORLD"
System.out.println(txt.toLowerCase());   // Outputs "hello world"


//indexOf()
String txt = "Please locate where 'locate' occurs!";
System.out.println(txt.indexOf("locate")); // Outputs 7


//concat
String firstName = "John ";
String lastName = "Doe";
System.out.println(firstName.concat(lastName));//Output:John Doe
```

| Escape character | Result | Description  |
| ---------------- | ------ | ------------ |
| \'               | '      | Single quote |
| \"               | "      | Double quote |
| \\               | \      | Backslash    |

```java
String txt = "It\'s alright.";//Output: It's alright.
```

## Java Math

The Java `Math` class has many methods that allow you to perform mathematical tasks on numbers.

### Math.max(x, y)

The `Math.max(x, y)` method can be used to find the highest value of `x` and `y`:

```java
Math.max(5, 10);
```

### Math.min(x, y)

The `Math.min(x, y)` method can be used to find the lowest value of `x` and `y`:

```java
Math.min(5, 10);
```

### Math.sqrt(x)

The `Math.sqrt(x)` method returns the square root of `x`:

```java
Math.sqrt(64);
```

### Math.abs(x)

The `Math.abs(x)` method returns the absolute (positive) value of `x`:

```java
Math.abs(-4.7);
```

### Random Numbers

`Math.random()` returns a random number between `0.0` (inclusive), and `1.0` (exclusive):

```java
Math.random();
```

Here is the content in markdown format:

## Java Method Overloading

### Method Overloading

With method overloading, multiple methods can have the same name but different parameters.

#### Example

```java
int myMethod(int x)
float myMethod(float x)
double myMethod(double x, double y)
```

Consider the following example, which has two methods that add numbers of different types:

#### Example

```java
static int plusMethodInt(int x, int y) {
  return x + y;
}

static double plusMethodDouble(double x, double y) {
  return x + y;
}

public static void main(String[] args) {
  int myNum1 = plusMethodInt(8, 5);
  double myNum2 = plusMethodDouble(4.3, 6.26);
  System.out.println("int: " + myNum1);
  System.out.println("double: " + myNum2);
}
```

#### Overloading the Method

Instead of defining two methods that should do the same thing, it is better to overload one method.

In the example below, we overload the `plusMethod` method to work for both `int` and `double`:

#### Example

```java
static int plusMethod(int x, int y) {
  return x + y;
}

static double plusMethod(double x, double y) {
  return x + y;
}

public static void main(String[] args) {
  int myNum1 = plusMethod(8, 5);
  double myNum2 = plusMethod(4.3, 6.26);
  System.out.println("int: " + myNum1);
  System.out.println("double: " + myNum2);
}
```

## Java - What is OOP?

OOP stands for **Object-Oriented Programming**.

Procedural programming focuses on writing methods or procedures that perform operations on data, while object-oriented programming involves creating objects that contain both data and methods.

#### Advantages of OOP over procedural programming:

- **Faster and easier to execute**
- **Provides a clear structure** for programs
- **Keeps Java code DRY** ("Don't Repeat Yourself"), making the code easier to maintain, modify, and debug
- **Enables reusability** with less code and shorter development time

> **Tip**: The "Don't Repeat Yourself" (DRY) principle aims to reduce code repetition. Extract common code and reuse it instead of repeating it.

---

## Java - What are Classes and Objects?

**Classes** and **Objects** are the core aspects of object-oriented programming.

#### Example:

##### Class

```java
Fruit
```

##### Objects

- Apple
- Banana
- Mango

Another example:

##### Class

```java
Car
```

##### Objects

- Volvo
- Audi
- Toyota

#### Summary:

- A **class** is a template for objects.
- An **object** is an instance of a class.
- Objects inherit all the variables and methods from the class.

---

## Exercise

What does OOP stand for?

- Operators Oriented Programming
- Output Operating Programming
- **Object-Oriented Programming**

---

## OOP Cheatsheet

| Concept           | Description                                                                   |
| ----------------- | ----------------------------------------------------------------------------- |
| **Class**         | A blueprint or template for creating objects.                                 |
| **Object**        | An instance of a class that contains data and methods.                        |
| **DRY Principle** | "Don't Repeat Yourself" - a principle to avoid redundancy in code.            |
| **Inheritance**   | Objects inherit properties and methods from their class.                      |
| **Encapsulation** | Bundling of data with methods that operate on that data.                      |
| **Polymorphism**  | The ability to process objects differently based on their data type or class. |
| **Abstraction**   | Hiding complex implementation details and showing only essential features.    |

## Java Class Attributes Cheatsheet

### Class Attributes

- Class attributes are variables defined within a class.
- **Example**: Create a class with two attributes `x` and `y`:
  ```java
  public class Main {
    int x = 5;
    int y = 3;
  }
  ```
- Class attributes are also known as **fields**.

### Accessing Attributes

- To access attributes, create an object of the class and use **dot syntax (.):**

  **Example**: Create an object `myObj` and access the value of `x`:

  ```java
  public class Main {
    int x = 5;

    public static void main(String[] args) {
      Main myObj = new Main();
      System.out.println(myObj.x);  // Outputs 5
    }
  }
  ```

### Modifying Attributes

- You can modify attribute values.

  **Example**: Set the value of `x` to 40:

  ```java
  public class Main {
    int x;

    public static void main(String[] args) {
      Main myObj = new Main();
      myObj.x = 40;
      System.out.println(myObj.x);  // Outputs 40
    }
  }
  ```

- You can also override existing values.

  **Example**: Change the value of `x` to 25:

  ```java
  public class Main {
    int x = 10;

    public static void main(String[] args) {
      Main myObj = new Main();
      myObj.x = 25;  // x is now 25
      System.out.println(myObj.x);  // Outputs 25
    }
  }
  ```

### Using `final` Keyword

- If you don’t want to allow changes to an attribute, use the `final` keyword.

  **Example**: Declaring `x` as final:

  ```java
  public class Main {
    final int x = 10;

    public static void main(String[] args) {
      Main myObj = new Main();
      myObj.x = 25;  // Will generate an error: cannot assign a value to a final variable
      System.out.println(myObj.x);
    }
  }
  ```

- `final` variables always store the same value (e.g., `PI = 3.14159...`).

### Multiple Objects

- You can create multiple objects of the same class, each having independent attribute values.

  **Example**: Change `x` in `myObj2` while leaving `myObj1` unchanged:

  ```java
  public class Main {
    int x = 5;

    public static void main(String[] args) {
      Main myObj1 = new Main();  // Object 1
      Main myObj2 = new Main();  // Object 2
      myObj2.x = 25;
      System.out.println(myObj1.x);  // Outputs 5
      System.out.println(myObj2.x);  // Outputs 25
    }
  }
  ```

## Java Class Methods Cheatsheet

### Declaring Methods

- Methods are declared within a class to perform actions.

  **Example**: Create a method `myMethod()` in the `Main` class:

  ```java
  public class Main {
    static void myMethod() {
      System.out.println("Hello World!");
    }
  }
  ```

### Calling Methods

- To call a method, use the method name followed by parentheses `()` and a semicolon `;`.

  **Example**: Call `myMethod()` inside `main`:

  ```java
  public class Main {
    static void myMethod() {
      System.out.println("Hello World!");
    }

    public static void main(String[] args) {
      myMethod();  // Outputs: Hello World!
    }
  }
  ```

### Static vs. Public Methods

- **Static Methods**: Can be called without creating an object.
- **Public Methods**: Must be called using an object.

  **Example**:

  ```java
  public class Main {
    // Static method
    static void myStaticMethod() {
      System.out.println("Static methods can be called without creating objects");
    }

    // Public method
    public void myPublicMethod() {
      System.out.println("Public methods must be called by creating objects");
    }

    public static void main(String[] args) {
      myStaticMethod();  // Call static method directly

      Main myObj = new Main();  // Create an object
      myObj.myPublicMethod();   // Call public method on the object
    }
  }
  ```

### Accessing Methods with an Object

- Create an object to call methods.

  **Example**: Create a `Car` object and call methods:

  ```java
  public class Main {
    // Method with no parameters
    public void fullThrottle() {
      System.out.println("The car is going as fast as it can!");
    }

    // Method with a parameter
    public void speed(int maxSpeed) {
      System.out.println("Max speed is: " + maxSpeed);
    }

    public static void main(String[] args) {
      Main myCar = new Main();  // Create an object
      myCar.fullThrottle();     // Call method
      myCar.speed(200);         // Call method with parameter
    }
  }
  ```

  **Output**:

  ```
  The car is going as fast as it can!
  Max speed is: 200
  ```

### Using Multiple Classes

- It’s a good practice to create an object of one class and access it in another class.

  **Example**:

  - **Main.java**:

  ```java
  public class Main {
    public void fullThrottle() {
      System.out.println("The car is going as fast as it can!");
    }

    public void speed(int maxSpeed) {
      System.out.println("Max speed is: " + maxSpeed);
    }
  }
  ```

  - **Second.java**:

  ```java
  class Second {
    public static void main(String[] args) {
      Main myCar = new Main();  // Create an object of Main
      myCar.fullThrottle();     // Call method
      myCar.speed(200);         // Call method with parameter
    }
  }
  ```

  **Compilation and Running**:

  ```bash
  javac Main.java
  javac Second.java
  java Second
  ```

  **Output**:

  ```
  The car is going as fast as it can!
  Max speed is: 200
  ```

### Key Points

- **Static methods** can be called directly without an object.
- **Public methods** require an object to be called.
- Use the dot `.` operator to access methods and attributes from an object.

## Java Constructors Cheatsheet

### What is a Constructor?

- A constructor in Java is a special method used to initialize objects.
- It is called when an object of a class is created.
- A constructor can be used to set initial values for object attributes.

  **Example**: Creating a constructor:

  ```java
  public class Main {
    int x;  // Class attribute

    // Constructor for the Main class
    public Main() {
      x = 5;  // Set initial value for x
    }

    public static void main(String[] args) {
      Main myObj = new Main();  // Create an object (calls the constructor)
      System.out.println(myObj.x);  // Outputs 5
    }
  }
  ```

### Constructor Key Points

- Constructor **name** must match the **class name**.
- Constructor **cannot** have a return type (not even `void`).
- **Automatically called** when an object is created.
- Java provides a **default constructor** if you don't create one, but it won't initialize attributes.

### Constructor with Parameters

- Constructors can take parameters to initialize object attributes.

  **Example**: Constructor with a parameter:

  ```java
  public class Main {
    int x;

    // Constructor with parameter
    public Main(int y) {
      x = y;
    }

    public static void main(String[] args) {
      Main myObj = new Main(5);  // Pass value 5 to constructor
      System.out.println(myObj.x);  // Outputs 5
    }
  }
  ```

- You can add **multiple parameters**.

  **Example**: Constructor with multiple parameters:

  ```java
  public class Main {
    int modelYear;
    String modelName;

    // Constructor with multiple parameters
    public Main(int year, String name) {
      modelYear = year;
      modelName = name;
    }

    public static void main(String[] args) {
      Main myCar = new Main(1969, "Mustang");
      System.out.println(myCar.modelYear + " " + myCar.modelName);  // Outputs 1969 Mustang
    }
  }
  ```

### Key Points to Remember:

- Constructors **initialize** the state of an object.
- A **no-argument constructor** is the default constructor.
- Constructors can have **parameters** to set initial values during object creation.
  Here’s a cheatsheet for Java Modifiers in markdown format:

## Java Modifiers Cheatsheet

### Modifiers Overview

Modifiers in Java are used to set the **access level** for classes, attributes, methods, and constructors.

#### Types of Modifiers:

1. **Access Modifiers** - Control access levels.
2. **Non-Access Modifiers** - Provide other functionalities (but don't control access levels).

---

### 1. Access Modifiers

#### For Classes:

| Modifier  | Description                                                                    |
| --------- | ------------------------------------------------------------------------------ |
| `public`  | Class is accessible by any other class.                                        |
| `default` | Class is accessible only by classes in the same package (no keyword required). |

#### For Attributes, Methods, and Constructors:

| Modifier    | Description                                       |
| ----------- | ------------------------------------------------- |
| `public`    | Accessible by all classes.                        |
| `private`   | Accessible only within the declared class.        |
| `default`   | Accessible within the same package.               |
| `protected` | Accessible in the same package and by subclasses. |

---

### 2. Non-Access Modifiers

#### For Classes:

| Modifier   | Description                                       |
| ---------- | ------------------------------------------------- |
| `final`    | Class cannot be inherited.                        |
| `abstract` | Class cannot be instantiated (must be inherited). |

#### For Attributes and Methods:

| Modifier       | Description                                                                             |
| -------------- | --------------------------------------------------------------------------------------- |
| `final`        | Cannot be overridden/modified.                                                          |
| `static`       | Belongs to the class rather than an object.                                             |
| `abstract`     | Must be used in an abstract class, does not have a body (e.g., `abstract void run();`). |
| `transient`    | Skips attributes when serializing objects.                                              |
| `synchronized` | Method can only be accessed by one thread at a time.                                    |
| `volatile`     | Value is always read from main memory, not cached locally.                              |

---

### 3. Examples of Non-Access Modifiers

#### `final` Modifier

- Prevents modification of attributes or methods.

```java
public class Main {
  final int x = 10;
  final double PI = 3.14;

  public static void main(String[] args) {
    Main myObj = new Main();
    myObj.x = 50;  // Error: cannot assign value to a final variable
    System.out.println(myObj.x);  // Outputs 10
  }
}
```

#### `static` Modifier

- Static methods can be called without creating an object.

```java
public class Main {
  // Static method
  static void myStaticMethod() {
    System.out.println("Static methods can be called without creating objects");
  }

  // Public method
  public void myPublicMethod() {
    System.out.println("Public methods must be called by creating objects");
  }

  public static void main(String[] args) {
    myStaticMethod();  // Call static method
    Main myObj = new Main();
    myObj.myPublicMethod();  // Call public method
  }
}
```

#### `abstract` Modifier

- Abstract methods are declared without a body and implemented by subclasses.

```java
// Abstract class
abstract class Main {
  public String fname = "John";
  public int age = 24;
  public abstract void study(); // Abstract method
}

// Subclass inheriting from Main
class Student extends Main {
  public int graduationYear = 2018;
  public void study() {  // Implementing abstract method
    System.out.println("Studying all day long");
  }
}

// Main class to test
class Second {
  public static void main(String[] args) {
    Student myObj = new Student();
    System.out.println("Name: " + myObj.fname);
    System.out.println("Age: " + myObj.age);
    System.out.println("Graduation Year: " + myObj.graduationYear);
    myObj.study();  // Call abstract method
  }
}
```

---

### Key Points:

- **public**, **private**, **protected**: Used to define access control.
- **final**, **static**, **abstract**: Define behavior of classes, methods, and attributes.
- Abstract methods **must** be implemented by subclasses.
Here’s a cheatsheet for **Java Encapsulation** in markdown format:
<!-- Finished -->

## Java Encapsulation Cheatsheet

### What is Encapsulation?

- **Encapsulation** ensures that sensitive data is hidden from users.
- Achieved by:
  1. Declaring class variables/attributes as `private`.
  2. Providing **public** `get` and `set` methods to access and update private variables.

---

### 1. Get and Set Methods

#### Syntax:

- **Getter** method: Returns the value of a private variable.
- **Setter** method: Updates the value of a private variable.

```java
public class Person {
  private String name; // private = restricted access

  // Getter
  public String getName() {
    return name;
  }

  // Setter
  public void setName(String newName) {
    this.name = newName;
  }
}
```

#### Explanation:

- `getName()`: Returns the value of `name`.
- `setName(String newName)`: Sets the value of `name` using the `this` keyword to refer to the current object.

---

### 2. Accessing Private Variables

- **Private variables** cannot be accessed directly from outside the class. Example:

```java
public class Main {
  public static void main(String[] args) {
    Person myObj = new Person();
    myObj.name = "John";  // Error: name has private access in Person
    System.out.println(myObj.name);  // Error
  }
}
```

#### Correct Way: Use Getter and Setter

```java
public class Main {
  public static void main(String[] args) {
    Person myObj = new Person();
    myObj.setName("John");  // Set the value of name
    System.out.println(myObj.getName());  // Outputs: John
  }
}
```

---

### 3. Why Use Encapsulation?

- **Better control** of class attributes and methods.
- Class attributes can be made:
  - **Read-only**: If only the `get` method is provided.
  - **Write-only**: If only the `set` method is provided.
- **Flexibility**: Changing part of the code without affecting other parts.
- **Increased security** of data.

---

### Key Points:

- Use `private` to hide variables from direct access.
- Use `get` and `set` methods to control access and modification of private variables.
- Encapsulation provides control, flexibility, and security.

Here's a summarized cheatsheet for Java Packages in markdown format:

## Java Packages & API Cheatsheet

### Overview

- **Packages** group related classes to avoid name conflicts and improve code maintainability.
- Two types:
  - **Built-in Packages**: Prewritten classes from the Java API.
  - **User-defined Packages**: Custom-created packages.

### Importing Packages

#### Syntax

```java
import package.name.Class;   // Import a single class
import package.name.*;       // Import all classes from a package
```

#### Example: Importing a Single Class

```java
import java.util.Scanner;   // Scanner class for user input

Scanner myObj = new Scanner(System.in);
String userName = myObj.nextLine();
```

#### Example: Importing an Entire Package

```java
import java.util.*;   // Imports all utility classes in java.util
```

### Java API

- A library of prewritten classes, available with the Java Development Environment.
- Components for **input handling**, **database programming**, and more.
- Full API documentation: [Oracle Java API](https://docs.oracle.com/javase/8/docs/api/).

---

### User-defined Packages

#### Package Creation

1. Define the package:

```java
package mypack;   // Package declaration
class MyPackageClass {
    public static void main(String[] args) {
        System.out.println("This is my package!");
    }
}
```

2. Save the file as `MyPackageClass.java`.
3. Compile the package:

```bash
javac -d . MyPackageClass.java   // -d specifies the destination
```

#### Running the Package

- After compiling, a directory named **mypack** will be created.
- To run the compiled class:

```bash
java mypack.MyPackageClass
```

#### Output

```
This is my package!
```

## Java Inheritance Cheatsheet

### Overview

- **Inheritance**: Enables one class to inherit fields and methods from another.
- Two categories:
  - **Superclass (parent)**: The class being inherited from.
  - **Subclass (child)**: The class that inherits from another class.

### Key Terms

- **`extends`**: Used to inherit from a superclass.

---

### Example: Basic Inheritance

```java
class Vehicle {
  protected String brand = "Ford";   // Vehicle attribute
  public void honk() {               // Vehicle method
    System.out.println("Tuut, tuut!");
  }
}

class Car extends Vehicle {
  private String modelName = "Mustang";  // Car attribute
  public static void main(String[] args) {
    Car myCar = new Car();         // Create an object of Car
    myCar.honk();                  // Call inherited method from Vehicle
    System.out.println(myCar.brand + " " + myCar.modelName);  // Access attributes
  }
}
```

#### Output:

```
Tuut, tuut!
Ford Mustang
```

---

### Protected Modifier

- **`protected`**: Allows access within the same package and by subclasses.
- If `brand` in the `Vehicle` class was **private**, the `Car` class couldn't access it.

---

### Why Use Inheritance?

- **Code Reusability**: Reuse fields and methods of an existing class in a new class.
- Facilitates easier maintenance and flexibility.

---

### The `final` Keyword

- **`final` class**: Prevents other classes from inheriting from it.
- Example:

  ```java
  final class Vehicle {
    // code
  }

  class Car extends Vehicle {   // This will cause an error
    // code
  }
  ```

- **Error Output**:
  ```
  Main.java:9: error: cannot inherit from final Vehicle
  class Car extends Vehicle {
                        ^
  1 error
  ```

---

### Java Polymorphism Cheatsheet

### Overview

- **Polymorphism**: "Many forms" – Allows methods to perform different tasks in classes that share inheritance.
- **Key Concept**: A single method behaves differently based on the object it is called on.
- Relies on **inheritance** to achieve method overriding in subclasses.

---

### Example: Polymorphism in Action

#### Superclass: `Animal`

```java
class Animal {
  public void animalSound() {
    System.out.println("The animal makes a sound");
  }
}
```

#### Subclass: `Pig`

```java
class Pig extends Animal {
  public void animalSound() {
    System.out.println("The pig says: wee wee");
  }
}
```

#### Subclass: `Dog`

```java
class Dog extends Animal {
  public void animalSound() {
    System.out.println("The dog says: bow wow");
  }
}
```

---

### Using Polymorphism

#### Main Method Example

```java
class Main {
  public static void main(String[] args) {
    Animal myAnimal = new Animal();  // Create an Animal object
    Animal myPig = new Pig();        // Create a Pig object
    Animal myDog = new Dog();        // Create a Dog object

    myAnimal.animalSound();   // Outputs: The animal makes a sound
    myPig.animalSound();      // Outputs: The pig says: wee wee
    myDog.animalSound();      // Outputs: The dog says: bow wow
  }
}
```

#### Output:

```
The animal makes a sound
The pig says: wee wee
The dog says: bow wow
```

---

### Key Takeaways

- **Method Overriding**: Subclasses override the `animalSound()` method of the superclass.
- **Single Method, Multiple Forms**: The same method behaves differently based on the object type (Pig, Dog, etc.).
- **Inheritance & Polymorphism** work hand-in-hand to provide flexibility and reuse in code.

---

### Advantages

- **Code Reusability**: Use a single method for different tasks across subclasses.
- **Maintainability**: Reduces code duplication and improves scalability.

Here's a summarized cheatsheet for Java Inner Classes in markdown format:

## Java Inner Classes Cheatsheet

## Overview

- **Inner Classes**: A class within another class. Used to group classes that logically belong together, improving code readability and maintainability.

---

## Types of Inner Classes

1. **Regular Inner Class**: A non-static class inside another class.
2. **Private Inner Class**: An inner class with private access.
3. **Static Inner Class**: Can be accessed without creating an instance of the outer class.

---

## Example: Regular Inner Class

### Accessing an Inner Class

```java
class OuterClass {
  int x = 10;

  class InnerClass {
    int y = 5;
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass myOuter = new OuterClass();
    OuterClass.InnerClass myInner = myOuter.new InnerClass();
    System.out.println(myInner.y + myOuter.x);  // Outputs 15 (5 + 10)
  }
}
```

---

## Private Inner Class

- An inner class can be declared **private** to restrict access from outside classes.

```java
class OuterClass {
  private class InnerClass {
    int y = 5;
  }
}
```

- Trying to access a private inner class from an outer class will cause an error.

---

## Static Inner Class

- A **static inner class** can be accessed without creating an instance of the outer class.

### Example:

```java
class OuterClass {
  static class InnerClass {
    int y = 5;
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass.InnerClass myInner = new OuterClass.InnerClass();
    System.out.println(myInner.y);  // Outputs 5
  }
}
```

- **Note**: Static inner classes do not have access to non-static members of the outer class.

---

## Accessing Outer Class from Inner Class

- Inner classes can access the members (attributes and methods) of their outer class.

### Example:

```java
class OuterClass {
  int x = 10;

  class InnerClass {
    public int myInnerMethod() {
      return x;
    }
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass myOuter = new OuterClass();
    OuterClass.InnerClass myInner = myOuter.new InnerClass();
    System.out.println(myInner.myInnerMethod());  // Outputs 10
  }
}
```

---

## Key Points

- **Regular Inner Classes**: Require an instance of the outer class to be instantiated.
- **Private Inner Classes**: Cannot be accessed outside the outer class.
- **Static Inner Classes**: Can be accessed without the outer class but cannot access non-static members.
- **Inner Class Access to Outer Class**: Inner classes can access outer class members.

Here is a summarized cheatsheet for **Java Abstract Classes and Methods** in markdown format:

## Java Abstract Classes and Methods Cheatsheet

## Overview

- **Abstraction**: Hides unnecessary details and shows only essential information to the user.
- Can be achieved through:
  - **Abstract classes**
  - **Interfaces** (discussed in next chapter)

---

## Abstract Class

- **Abstract class**: A restricted class that **cannot be instantiated** (cannot create objects from it).
- Must be inherited by a subclass to use its abstract methods.

### Example:

````java
abstract class Animal {
  public abstract void animalSound();  // Abstract method (no body)
  public void sleep() {                // Regular method
    System.out.println("Zzz");
  }
}

---

## Abstract Method

- **Abstract method**: Declared in an abstract class **without a body**.
- The body of the method is provided in the subclass.

### Example:

```java
abstract class Animal {
  public abstract void animalSound();  // Abstract method
  public void sleep() {
    System.out.println("Zzz");
  }
}

class Pig extends Animal {
  public void animalSound() {          // Body of abstract method
    System.out.println("The pig says: wee wee");
  }
}

---

## Using Abstract Classes and Methods

- Abstract classes **cannot be instantiated** directly:

  ```java
  Animal myObj = new Animal();  // Error! Cannot create an object of abstract class
````

- To use an abstract class, it **must be inherited**:

  ```java
  class Pig extends Animal {
    public void animalSound() {
      System.out.println("The pig says: wee wee");
    }
  }

  class Main {
    public static void main(String[] args) {
      Pig myPig = new Pig();  // Create an object of Pig (subclass)
      myPig.animalSound();    // Calls abstract method
      myPig.sleep();          // Calls regular method
    }
  }
  ```

---

## Key Points

- **Abstract class**: Cannot create objects from it, used for inheritance.
- **Abstract method**: Must be overridden in the subclass, no method body in the abstract class.
- An abstract class can have **both abstract and non-abstract methods**.
- **Concrete classes** (subclasses) provide implementation for abstract methods.

Here’s the summarized **Java Interfaces** cheatsheet in markdown format:

# Java Interfaces Cheatsheet

## Overview

- **Interface**: A completely abstract class used to group related methods **without bodies**.
- Interfaces **achieve abstraction** and **multiple inheritance** in Java.

---

## Defining an Interface

- An interface only contains **method declarations** and **constants**.

### Example:

```java
// Define interface
interface Animal {
  public void animalSound(); // No method body
  public void sleep();       // No method body
}
```

---

## Implementing an Interface

- Use the `implements` keyword to implement an interface in a class.
- The implementing class **must provide bodies** for all the interface methods.

### Example:

```java
// Implementing the interface
class Pig implements Animal {
  public void animalSound() {
    System.out.println("The pig says: wee wee");
  }
  public void sleep() {
    System.out.println("Zzz");
  }
}

class Main {
  public static void main(String[] args) {
    Pig myPig = new Pig();    // Create Pig object
    myPig.animalSound();      // Call interface method
    myPig.sleep();            // Call interface method
  }
}
```

---

## Key Points on Interfaces

- **Cannot instantiate**: Interfaces cannot be used to create objects.
- **Method bodies**: Methods in an interface do not have bodies; they are provided by the implementing class.
- **Must override**: All interface methods **must be overridden** in the implementing class.
- **Default modifiers**:
  - Methods are **public** and **abstract** by default.
  - Attributes are **public**, **static**, and **final** by default.
- **No constructor**: Interfaces cannot have constructors since they cannot be instantiated.

---

## Multiple Interfaces

- A class can implement multiple interfaces, which helps in **multiple inheritance**.

### Example:

```java
// Define interfaces
interface FirstInterface {
  public void myMethod();     // Interface method
}

interface SecondInterface {
  public void myOtherMethod(); // Interface method
}

// Implement both interfaces
class DemoClass implements FirstInterface, SecondInterface {
  public void myMethod() {
    System.out.println("Some text..");
  }
  public void myOtherMethod() {
    System.out.println("Some other text...");
  }
}

class Main {
  public static void main(String[] args) {
    DemoClass myObj = new DemoClass();
    myObj.myMethod();
    myObj.myOtherMethod();
  }
}
```

---

## Why Use Interfaces?

1. **Achieve abstraction**: Hide implementation details and only expose necessary methods.
2. **Multiple inheritance**: Unlike classes, interfaces allow a class to inherit from multiple sources.
   Here’s a cheat sheet for Java Enums in markdown format:

## Java Enums Cheat Sheet

### What is an Enum?

- A **special "class"** to represent a **group of constants** (unchangeable variables).
- Created using the `enum` keyword.

### Basic Syntax

```java
enum Level {
  LOW,
  MEDIUM,
  HIGH
}
Level myVar = Level.MEDIUM;
```

### Enum inside a Class

- Enums can be nested within classes.

```java
public class Main {
  enum Level {
    LOW,
    MEDIUM,
    HIGH
  }
  public static void main(String[] args) {
    Level myVar = Level.MEDIUM;
    System.out.println(myVar); // Output: MEDIUM
  }
}
```

### Enum in a Switch Statement

- Enums can be used in `switch` statements.

```java
enum Level {
  LOW,
  MEDIUM,
  HIGH
}

public class Main {
  public static void main(String[] args) {
    Level myVar = Level.MEDIUM;
    switch (myVar) {
      case LOW:
        System.out.println("Low level");
        break;
      case MEDIUM:
        System.out.println("Medium level");
        break;
      case HIGH:
        System.out.println("High level");
        break;
    }
  }
}
// Output: Medium level
```

### Loop Through an Enum

- Use the `values()` method to get all constants in an enum.

```java
for (Level myVar : Level.values()) {
  System.out.println(myVar);
}
// Output:
// LOW
// MEDIUM
// HIGH
```

### Enum Attributes and Methods

- Enums can have **attributes and methods** but **constants are `public`, `static`, and `final`**.
- **Cannot create objects** of enums or extend other classes (can implement interfaces).

### When to Use Enums?

- Use enums when values are **fixed** and won’t change (e.g., **days, colors, card suits**).

```

This cheat sheet provides a concise summary of the key concepts and usage of enums in Java.
```

Here’s a cheat sheet for Java Wrapper Classes in markdown format:

## Java Wrapper Classes Cheat Sheet

### What are Wrapper Classes?

- Wrapper classes allow using **primitive data types as objects**.
- Useful in Collections (e.g., `ArrayList`) where **only objects** can be stored.

#### Primitive Types vs Wrapper Classes

| Primitive Type | Wrapper Class |
| -------------- | ------------- |
| `byte`         | `Byte`        |
| `short`        | `Short`       |
| `int`          | `Integer`     |
| `long`         | `Long`        |
| `float`        | `Float`       |
| `double`       | `Double`      |
| `boolean`      | `Boolean`     |
| `char`         | `Character`   |

### Creating Wrapper Objects

- Use the wrapper class instead of the primitive type.

```java
Integer myInt = 5;
Double myDouble = 5.99;
Character myChar = 'A';

System.out.println(myInt);    // Output: 5
System.out.println(myDouble);  // Output: 5.99
System.out.println(myChar);    // Output: A
```

### Wrapper Methods

#### Value Methods

- Methods to get the primitive value from a wrapper object:
  - `intValue()`, `doubleValue()`, `charValue()`, etc.

```java
Integer myInt = 5;
System.out.println(myInt.intValue());  // Output: 5
```

#### `toString()` Method

- Converts a wrapper object to a `String`.

```java
Integer myInt = 100;
String myString = myInt.toString();
System.out.println(myString.length());  // Output: 3
```

### Why Use Wrapper Classes?

- Needed when **only objects** are accepted (e.g., Collections).
- Provides **methods for data manipulation** and **type conversion**.

```

This cheat sheet captures the essentials of Java Wrapper Classes, making it easy to understand and reference.
```

Here’s the **Java Exceptions** cheatsheet in markdown format:

## Java Exceptions Cheatsheet

### Overview

- **Exceptions**: Errors that occur during execution, stopping the program unless handled.
- Common exception types: `ArrayIndexOutOfBoundsException`, `ArithmeticException`, `FileNotFoundException`, `SecurityException`, etc.

---

### Try and Catch

- Use `try` to define a block of code to test for errors.
- Use `catch` to define code to handle errors if they occur.

#### Syntax:

```java
try {
  // Code to try
} catch (Exception e) {
  // Code to handle error
}
```

#### Example:

```java
public class Main {
  public static void main(String[] args) {
    try {
      int[] myNumbers = {1, 2, 3};
      System.out.println(myNumbers[10]); // Error!
    } catch (Exception e) {
      System.out.println("Something went wrong.");
    }
  }
}
```

#### Output:

```
Something went wrong.
```

---

### Finally

- The `finally` block executes **regardless of the result** of the `try-catch`.

#### Example:

```java
public class Main {
  public static void main(String[] args) {
    try {
      int[] myNumbers = {1, 2, 3};
      System.out.println(myNumbers[10]);
    } catch (Exception e) {
      System.out.println("Something went wrong.");
    } finally {
      System.out.println("The 'try catch' is finished.");
    }
  }
}
```

#### Output:

```
Something went wrong.
The 'try catch' is finished.
```

---

### Throw Keyword

- The `throw` statement allows creating custom exceptions with a specified type.

#### Example:

Throw an exception if `age` is below 18:

```java
public class Main {
  static void checkAge(int age) {
    if (age < 18) {
      throw new ArithmeticException("Access denied - You must be at least 18 years old.");
    } else {
      System.out.println("Access granted - You are old enough!");
    }
  }

  public static void main(String[] args) {
    checkAge(15); // Triggers exception
  }
}
```

#### Output:

```
Exception in thread "main" java.lang.ArithmeticException: Access denied - You must be at least 18 years old.
```

If `age` was set to 20:

```java
checkAge(20);
```

#### Output:

```
Access granted - You are old enough!
```

---

### Exercise

Complete the code to handle exceptions:

```java
try {
  int[] myNumbers = {1, 2, 3};
  System.out.println(myNumbers[10]);
} catch (Exception e) {
  System.out.println("Something went wrong.");
}
```

## Java Constructors

A constructor in Java is a special method that is used to initialize objects. The constructor is called when an object of a class is created.

```java
public class Main {
  int x;  // Create a class attribute

  // Create a class constructor for the Main class
  public Main() {
    x = 5;  // Set the initial value for the class attribute x
  }

  public static void main(String[] args) {
    Main myObj = new Main(); // Create an object of class Main (This will call the constructor)
    System.out.println(myObj.x); // Print the value of x
  }
}

// Outputs 5
```

## Access Modifier

For attributes and methods, you can use the one of the following:

| Modifier     | Description                                                                                                                                                                                                                                                                                         |
| ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| final        | Attributes and methods cannot be overridden/modified                                                                                                                                                                                                                                                |
| static       | Attributes and methods belongs to the class, rather than an object                                                                                                                                                                                                                                  |
| abstract     | Can only be used in an abstract class, and can only be used on methods. The method does not have a body, for example abstract void run();. The body is provided by the subclass (inherited from). You will learn more about inheritance and abstraction in the Inheritance and Abstraction chapters |
| transient    | Attributes and methods are skipped when serializing the object containing them                                                                                                                                                                                                                      |
| synchronized | Methods can only be accessed by one thread at a time                                                                                                                                                                                                                                                |
| volatile     | The value of an attribute is not cached thread-locally, and is always read from the "main memory                                                                                                                                                                                                    |

### static method and public method

```java
public class Main {
  // Static method
  static void myStaticMethod() {
    System.out.println("Static methods can be called without creating objects");
  }

  // Public method
  public void myPublicMethod() {
    System.out.println("Public methods must be called by creating objects");
  }

  // Main method
  public static void main(String[] args) {
    myStaticMethod(); // Call the static method

    Main myObj = new Main(); // Create an object of MyClass
    myObj.myPublicMethod(); // Call the public method
  }
}

```

```
output:

Static methods can be called without creating objects
Public methods must be called by creating objects
```

### abstract method

```java
// Code from filename: Main.java
// abstract class
abstract class Main {
  public String fname = "John";
  public int age = 24;
  public abstract void study(); // abstract method
}

// Subclass (inherit from Main)
class Student extends Main {
  public int graduationYear = 2018;
  public void study() { // the body of the abstract method is provided here
    System.out.println("Studying all day long");
  }
}
// End code from filename: Main.java

// Code from filename: Second.java
class Second {
  public static void main(String[] args) {
    // create an object of the Student class (which inherits attributes and methods from Main)
    Student myObj = new Student();

    System.out.println("Name: " + myObj.fname);
    System.out.println("Age: " + myObj.age);
    System.out.println("Graduation Year: " + myObj.graduationYear);
    myObj.study(); // call abstract method
  }
}
```

### final modifier

```java
public class Main {
  final int x = 10;
  final double PI = 3.14;

  public static void main(String[] args) {
    Main myObj = new Main();
    myObj.x = 50; // will generate an error: cannot assign a value to a final variable
    myObj.PI = 25; // will generate an error: cannot assign a value to a final variable
    System.out.println(myObj.x);
  }
}
```

## What is Encapsulation?

Encapsulation ensures that **sensitive data** is hidden from users.

### How to Achieve Encapsulation:

1. **Declare class variables/attributes as `private`.**
2. **Provide public `get` and `set` methods** to access and update private variables.

---

## Get and Set Methods

- **`get` Method:** Returns the variable value.
- **`set` Method:** Sets the variable value.

### Syntax:

Method names start with `get` or `set` followed by the variable name with the first letter in uppercase.

---

### Example:

```java
public class Person {
  private String name; // Private variable

  // Getter
  public String getName() {
    return name;
  }

  // Setter
  public void setName(String newName) {
    this.name = newName;
  }
}
```

---

### Using Encapsulation:

```java
public class Main {
  public static void main(String[] args) {
    Person myObj = new Person();
    myObj.setName("John"); // Set the value of name
    System.out.println(myObj.getName()); // Get the value of name
  }
}
// Outputs: John
```

---

## Why Use Encapsulation?

1. **Better control** over class attributes and methods.
2. **Flexible:** Changes in one part of the code don’t affect others.
3. **Increased security** of data.
4. Can make attributes **read-only** (only `get`) or **write-only** (only `set`).

````markdown
# Java Packages

## What are Java Packages?

Packages in Java are used to group related classes, helping to:

1. Avoid **name conflicts**.
2. Improve code **readability** and **maintainability**

### Types of Packages:

1. **Built-in Packages:** Provided by Java API.
2. **User-defined Packages:** Custom packages created by developers.

---

## Built-in Packages

Java API provides prewritten classes for functionalities like input handling, database programming, etc.

### Importing Built-in Packages:

- Import a single class:
  ```java
  import package.name.Class;
  ```
````

- Import all classes from a package:
  ```java
  import package.name.*;
  ```

### Example: Importing `Scanner` Class

```java
import java.util.Scanner;

class MyClass {
  public static void main(String[] args) {
    Scanner myObj = new Scanner(System.in);
    System.out.println("Enter username:");
    String userName = myObj.nextLine();
    System.out.println("Username is: " + userName);
  }
}
```

---

## User-defined Packages

### Steps to Create a Package:

1. Use the `package` keyword:
   ```java
   package mypack;
   class MyPackageClass {
     public static void main(String[] args) {
       System.out.println("This is my package!");
     }
   }
   ```
2. Save the file as `MyPackageClass.java`.

3. Compile the file and create the package:

   ```bash
   javac -d . MyPackageClass.java
   ```

   - **`-d` flag**: Specifies the destination folder for the package.
   - A new folder `mypack` will be created.

4. Run the compiled package:
   ```bash
   java mypack.MyPackageClass
   ```
   **Output:**
   ```
   This is my package!
   ```

### Notes:

- Package names should be written in **lowercase** to avoid conflicts with class names.

## Java Inner Classes

In Java, you can nest classes (a class within a class) to group related classes together, making your code more readable and maintainable.

---

## Types of Inner Classes

### 1. **Regular Inner Class**

To access an inner class, create an object of the outer class, then create an object of the inner class.

#### Example:

```java
class OuterClass {
  int x = 10;

  class InnerClass {
    int y = 5;
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass myOuter = new OuterClass();
    OuterClass.InnerClass myInner = myOuter.new InnerClass();
    System.out.println(myInner.y + myOuter.x); // Outputs 15 (5 + 10)
  }
}
```

---

### 2. **Private Inner Class**

An inner class can be declared `private` or `protected`, restricting its access from outside the outer class.

#### Example:

```java
class OuterClass {
  int x = 10;

  private class InnerClass {
    int y = 5;
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass myOuter = new OuterClass();
    OuterClass.InnerClass myInner = myOuter.new InnerClass(); // Error: InnerClass is private
  }
}
```

#### Error:

```
Main.java:13: error: OuterClass.InnerClass has private access in OuterClass
```

---

### 3. **Static Inner Class**

A `static` inner class can be accessed without creating an object of the outer class. However, it cannot access non-static members of the outer class.

#### Example:

```java
class OuterClass {
  int x = 10;

  static class InnerClass {
    int y = 5;
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass.InnerClass myInner = new OuterClass.InnerClass();
    System.out.println(myInner.y); // Outputs 5
  }
}
```

---

### 4. **Access Outer Class Members From Inner Class**

An inner class can directly access members (both fields and methods) of its outer class.

#### Example:

```java
class OuterClass {
  int x = 10;

  class InnerClass {
    public int myInnerMethod() {
      return x; // Accessing outer class member
    }
  }
}

public class Main {
  public static void main(String[] args) {
    OuterClass myOuter = new OuterClass();
    OuterClass.InnerClass myInner = myOuter.new InnerClass();
    System.out.println(myInner.myInnerMethod()); // Outputs 10
  }
}
```

---

## Key Points:

1. Inner classes can be **regular**, **private**, or **static**.
2. **Regular and private inner classes** require an outer class instance for access.
3. **Static inner classes** can be accessed without an outer class instance but cannot access non-static members of the outer class.
4. Inner classes can access the outer class's members directly.

# Abstract Classes and Methods

## What is Data Abstraction?

Data abstraction is the process of hiding implementation details while showing only essential information to the user. In Java, abstraction can be achieved through:

- **Abstract Classes**
- **Interfaces** (discussed in the next chapter)

---

## Key Concepts of Abstract Classes and Methods

### 1. **Abstract Class**

- A class declared with the `abstract` keyword.
- **Cannot be instantiated** directly (i.e., you cannot create objects of an abstract class).
- Can contain both:
  - **Abstract methods** (without a body).
  - **Regular methods** (with a body).

#### Syntax:

```java
abstract class Animal {
  public abstract void animalSound(); // Abstract method
  public void sleep() {               // Regular method
    System.out.println("Zzz");
  }
}
```

---

### 2. **Abstract Method**

- Declared within an abstract class using the `abstract` keyword.
- **Does not have a body**—the body is provided by the subclass inheriting the abstract class.

---

### 3. **Inheritance with Abstract Classes**

To use an abstract class, it must be inherited by another class. Use the `extends` keyword for inheritance.

#### Example:

```java
// Abstract class
abstract class Animal {
  public abstract void animalSound(); // Abstract method
  public void sleep() {               // Regular method
    System.out.println("Zzz");
  }
}

// Subclass (inherits from Animal)
class Pig extends Animal {
  public void animalSound() {
    System.out.println("The pig says: wee wee");
  }
}

class Main {
  public static void main(String[] args) {
    Pig myPig = new Pig(); // Create a Pig object
    myPig.animalSound();   // Outputs: The pig says: wee wee
    myPig.sleep();         // Outputs: Zzz
  }
}
```

---

### 4. **Why Use Abstract Classes and Methods?**

- **Security**: Hide implementation details and show only the necessary features.
- Ensure that certain methods must be implemented by subclasses, enforcing a design contract.

---

### Key Points:

1. Abstract classes **cannot be instantiated** directly.
   - Example:
     ```java
     Animal myObj = new Animal(); // Error: Animal is abstract
     ```
2. Subclasses must provide a body for all abstract methods from the abstract class.
3. Abstraction can also be achieved using **interfaces** (discussed in the next chapter).

# Java ArrayList

The `ArrayList` class in Java, part of the `java.util` package, is a resizable array that allows elements to be added or removed dynamically, unlike standard arrays with fixed sizes.

---

## Key Features of ArrayList

1. **Dynamic Resizing**: Size adjusts as elements are added/removed.
2. **Flexible Syntax**: Easier to manipulate compared to arrays.

---

## Creating an ArrayList

```java
import java.util.ArrayList;

ArrayList<String> cars = new ArrayList<String>();
```

---

## Common Operations

### 1. **Adding Items**

- Use the `add()` method:
  ```java
  cars.add("Volvo");
  cars.add("BMW");
  ```
- Insert at a specific position:
  ```java
  cars.add(0, "Mazda");
  ```

### 2. **Accessing Items**

- Use the `get()` method:
  ```java
  cars.get(0);
  ```

### 3. **Modifying Items**

- Use the `set()` method:
  ```java
  cars.set(0, "Opel");
  ```

### 4. **Removing Items**

- Remove a specific item:
  ```java
  cars.remove(0);
  ```
- Clear all elements:
  ```java
  cars.clear();
  ```

### 5. **Finding Size**

- Use the `size()` method:
  ```java
  cars.size();
  ```

---

## Looping Through an ArrayList

- **For Loop**:
  ```java
  for (int i = 0; i < cars.size(); i++) {
    System.out.println(cars.get(i));
  }
  ```
- **For-Each Loop**:
  ```java
  for (String car : cars) {
    System.out.println(car);
  }
  ```

---

## Using Other Types in ArrayList

- ArrayLists store objects. For primitive types, use wrapper classes:
  - `Integer` for `int`, `Boolean` for `boolean`, etc.

#### Example:

```java
ArrayList<Integer> myNumbers = new ArrayList<Integer>();
myNumbers.add(10);
myNumbers.add(15);
```

---

## Sorting an ArrayList

- Use the `Collections.sort()` method from the `java.util.Collections` package.

#### Example: Sort Strings

```java
import java.util.Collections;

Collections.sort(cars);
```

#### Example: Sort Integers

```java
Collections.sort(myNumbers);
```

---

## Complete Example

```java
import java.util.ArrayList;
import java.util.Collections;

public class Main {
  public static void main(String[] args) {
    ArrayList<String> cars = new ArrayList<String>();
    cars.add("Volvo");
    cars.add("BMW");
    cars.add("Ford");
    cars.add("Mazda");

    // Add an element
    cars.add(0, "Toyota");

    // Modify an element
    cars.set(1, "Tesla");

    // Remove an element
    cars.remove(2);

    // Sort the ArrayList
    Collections.sort(cars);

    // Loop through the ArrayList
    for (String car : cars) {
      System.out.println(car);
    }

    // Find size
    System.out.println("Size: " + cars.size());
  }
}
```

---

## Advantages of ArrayList

- **Dynamic Resizing**: Automatically grows/shrinks.
- **Rich Functionality**: Provides methods for common operations.
- **Flexibility**: Supports generic types and easy integration.

---

For more advanced sorting or functionality, explore the `java.util.Collections` and `java.util.stream` packages.

```

```
