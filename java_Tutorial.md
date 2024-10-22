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

````md
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
````

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

```

You can save this as a `.md` file for quick reference!
```
