
---
title : Classes and Objects
noteOrder : 53

---

### Introduction

An important feature of programming languages like Java, python, or C++ is that they are all Object Oriented Programming languages. 

Object Oriented Programming is when we use things called classes or objects in your programs. Classes contain functions and variables and we use objects to implement the class and use the functions and variables.

To make sure this isn't completely new to you, I'll show you an example.

Whenever we wanted to take an input from the user, we used the Scanner class. First, we imported the class into the program by importing the util package containing the scanner class. The import statement looked like this

```Java
import java.util.*; // import statement
```

After we import the scanner class, we can't directly use methods like the "nextInt( )" method or the "nextDouble( )" method. We created an object. The object creation statement looked like this:

```Java
Scanner sc = new Scanner(System.in); // creating object called sc
```

We give our object a name sc so that whenever we want to use the Scanner class, we can use the object name. We use the object name sc to call the methods of the Scanner class.

```Java
int n = sc.nextInt(); // using object sc to call nextInt( ) method
```

This is a very good example of Object Oriented Programming. Here, our Scanner class contains useful methods to take input from the user. To use the class or implement in our program, we can create an object of the Scanner class and use it to call the methods. 

If you learn Object Oriented Programming, you can create your own classes and objects. It's a huge concept so there are many lessons on Object Oriented Programming.  In this lesson, we'll learn how to create classes and objects for a class.

### Video lesson


![Understanding Classes and Objects](https://youtu.be/rruQbDwmn24?si=eX8ESwnNVRXARcQa)

### Syntax

To show the syntax for creating a class and an object, I created a class called Rocket and an object of that class called obj in the main method. I didn't add any variables or methods in the class since we haven't discussed them yet. 

```Java
class Rocket{
	// Variables and methods
}
public class ClassesObjects{
	public static void main(String[]args){
		Rocket obj = new Rocket();
	}
}
```