## How a program works in Java

Let's dive deeper into the code and the syntax we used in the *Hello World!* program. Synthesis of the code to provide you with a deeper understanding of the concepts and the structure of Java Language.

```java
public class Main {

    public static void main(String[] args) {
        System.out.println("Hello World!");
    }
}
```

## Syntax Breakdown
We'll look at this code line by line and go through the syntax from the top for a better understanding.

```java
public class Main
```

`public` : The `public` keyword is an access modifier used for `classes`,attributes, methods and constructors, making them visible and accessible by any other class from all the packages. 

`class` : This is one of the most important keywords in this language as Java follows an Object-Oriented Methodology. `Classes` are the "Blueprint" of an `Object` (more about objects in further units). `Class` contains Contructors, variables, methods, etc. These properties are manifested by the `objects` when an object is created. Unlike C++, creating a `class` is mandatory in Java as you are allowed to create functions, methods or initiate variables inside a `class` only, doing so outside the `class` would throw an error. 

In this *Hello World!* program, we have created a `class` named `Main`. Whatever we aim to write will be written in this Class only, if not, then we may create another Class to do so with a different name to do so.

> [!tip] : It is considered as good practice to keep the initial letter for the class name to be in `uppercase` i.e. to write "Main" instead of "main".
