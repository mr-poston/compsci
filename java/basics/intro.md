# Intro to Java

## Printing to the Screen

### What is a print statement?

A print statement is a command (piece of code) in Java that will print something out to the computer’s screen.

Print statements are very useful for seeing the result of something your program did.

Programmers can use print statements to relay information about our program to the user.   This is the most basic form of output, and very useful!

### How do I use a print statement?

To use a print statement, you type the code for a print statement inside the `main` method.

**IMPORTANT** – everything in Java is CASE SENSITIVE, meaning letters that are upper case **need** to be uppercase, and the code won’t work if it’s not exactly right.

In Java, there are two basic print statements:
```java
System.out.print("Text goes here");
```
```java
System.out.println("Text goes here");
```

A print statement always ends in a semi-colon (this `;` is a semi-colon).

This is true of all **statements** in Java.  A statement is a complete line of code that runs, and you'll know it's a statement because it ends in a semi-colon!

If you have an error with your program, the first thing to check is that the line ends in a semi-colon (if required)!

### Printing Examples

```java
System.out.println("Hello world");
```
Would print:
```
Hello world
```
```java
System.out.println("Helloworld");
```
Would print:
```
Helloworld
```
*Note that it didn’t print the space (because we didn’t tell it to print the space)!*
```java
System.out.println(Hello World);
```
The above would not work!  We forgot the double quotes around Hello World.
