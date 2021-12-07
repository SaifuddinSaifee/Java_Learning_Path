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

-----------------------------------------------------------------------------------------------------------
`static` : `Main` is a class, and `main()` is a method in this class. In Java, to use the features of a class such as variable, and methods (`main()` method is this case), an `object` of that `class` has to be instantiated that acquires all the properties of that class. Once the `Object` is created, it can now use all the properties that have been declared in the `class`. 

But if that's the case, then to use the `main()` method of this `class`, an object of this `class Main` has to be created, and clearly we just started writing the code and we don't see any object initialization anywhere. So, this where the `static` keyword comes into the play. `Static` keyword removes the necessity of object creation of a class for that particular `method` (`main()` method in this case). Now the JVM directly executes the `main()` method like this `Main.main()`, here the JVM directly executed the main method by referring the Class, without creating any object.

`void main()` : `void` is the return type of `main()` method, when a `method` is created, it is supposed to perform an operation with the data you pass into the `method`. But after the completion of that operation, we need the results (Why else would we perform the operation), So it's like, you give the method some data, the method processes that data, and the that processed data is returned to us. In this case, we declared the return type of this method to be `void`

To understand this better let's see what exactly is happening here. When you compile your Java program and run it, the JVM (Java Virtual machine) looks for an entry point or a starting point for the execution of code. Now, everything we write in java is inside `classes`, there's nothing outside a class. So to access any class, the JVM needs to create an `object` of that `class`. Apperently, JVM does not have the ability to instantiate a class or create an object of any class (or infact to create anything at all). 
