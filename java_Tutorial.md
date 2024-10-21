# What is Java?

Java is a popular programming language, created in 1995.

It is owned by Oracle, and more than 3 billion devices run Java.

### It is used for:

- Mobile applications (specially Android apps)
- Desktop applications
- Web applications
- Web servers and application servers
- Games
- Database connection
- And much, much more!

### Why Use Java?

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
