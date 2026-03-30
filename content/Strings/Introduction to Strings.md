
---
title : Introduction to Strings
noteOrder : 100

---

### Introduction

In Java (and most other programming languages), a collections of characters as something like words or sentences are called strings. 

Strings don't have to be just words or sentences. Remember. Characters include multiple things like digits, special characters like #, @, ! and many more, so even a random collection of characters like "356jdsfkj3j59@45", although not a valid word, is a String. For it to be a String, it just needs to be a collection of characters enclosed by double quotes. 

Strings aren't completely new to you though. We've used them before when printing or displaying things. Take a look at the following println statement

```Java
System.out.println("Strings are fun!");
```

Here, we're printing the String "Strings are fun!". I want you to remember that every String has double quotes around it. This is how we know it's a String and not some other data type. 

This lesson should be a good introduction to creating and using Strings in Java. We'll learn a lot more about them in the next few lessons.

### Video Lesson

![Introduction to Strings in Java](https://youtu.be/tZnFoSk4RiM?si=vutygBrKd8_P1S76)

### Syntax

The following block of code shows the syntax for creating strings in Java.

```Java
public class StringsInJava{
	public static void main(String[]args){
		// Different ways to create a string
		String obj = new String("Hello World!");
		String obj2 = "Hello World!";
		
		System.out.println(obj);
		System.out.println(obj2);
	}
}
```