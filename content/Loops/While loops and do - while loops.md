
---
title : While loops and do - while loops
noteOrder : 35

---

### Introduction

Let's say you wanted to write a program to print the word "hello" ten times. You can do this by just using ten println statements. That would look like this:

```Java
public class HelloPrint{
	public static void main(String[]args){
		System.out.println("hello");
		System.out.println("hello");
		System.out.println("hello");	
		System.out.println("hello");	
		System.out.println("hello");	
		System.out.println("hello");	
		System.out.println("hello");	
		System.out.println("hello");	
		System.out.println("hello");
		System.out.println("hello");			
	}
}
```

But then, let's say you wanted to add a hundred println statements or a thousand, you can't just keep typing the same code multiple times. To do this, we can use loops.

In programming, loops are pretty straightforward. A loop would keep executing a block of code as long as a particular condition is true. Depending on the condition, we can use it to execute the block of code how many ever times we want.

In Java, there are three types of loops you can use : while loops, for loops, and do-while loops. In this lesson, you're going to be learning about while loops and do-while loops.

### Video lesson

![Understanding while loops and do-while loops](https://youtu.be/OmbTXgdvZzo)

### Syntax

To demonstrate the syntax of while loops and do-while loops, I wrote the same program to print "hello" ten times using a while loop and a do-while loop.

```Java
public class Loops{
	public static void main(String[]args){
	
		// using a while loop
		int i = 1;
		while(i<=10){
			System.out.println("hello");
			i++;
		}
		
		//using a do-while loop
		int temp = 1;
		do{
			System.out.println("hello");
			temp++;
		}
		while(temp<=10);
	}
}
```
