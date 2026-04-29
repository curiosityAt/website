
---
title : print vs println
noteOrder  : 3

---
### Introduction

By now, you must have understood the syntax for the basic structure of a Java program and how to print something in a program. If I want to print "Hello World", I'll use a println statement like the one below.


``` Java
System.out.println("Hello World");
```

Java also provides us with another statement called a print statement. Printing "Hello World" using a print statement would look like this

``` Java
System.out.print("Hello World");
```

Although they look similar and end up printing the same thing, they behave differently. It is both useful and important to understand the difference between them.

### Video lesson

![Print vs Println Statements](https://youtu.be/syV9_sO--4o)

### Syntax

The following block of code shows the syntax for both println and print statements.

```Java
public class Printing{
	public static void main(String[]args){
		System.out.println("hello world"); //println statement
		System.out.print("welcome to the channel!"); //print statement
	}
}
```



