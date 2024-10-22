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

# Java - What are Classes and Objects?

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

# Exercise

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
