
---
title : if, if-else, if-else if
noteOrder : 23

---

## Introduction

Conditional statements are used to control the flow of the program. We can use them to execute certain blocks of code if a condition is true or even skip a certain block of code if the condition is false. We can use them to control what our program does. In Java and most other programming languages, we have three conditional statement : the if statement, the else statement, and the else if statement. In this lesson, you'll learn what these statements do and how you can effectively use them in a program.

## Video lesson

![Conditional statements in Java](https://youtu.be/QLe5Vj7Ebbw)

## Syntax

To show the syntax of all the conditional statements, I created a simple program that compares two numbers. 

```Java
public class ConditionalStatements{
	public static void main(String[]args){
		// a program to compare two numbers
		int a = 22;
		int b = 45;
		
		if(a > b){ // if statement
			System.out.println("a is larger");
		}
		else if(a < b){ // else if statement
			System.out.println("a is smaller");
		}
		else{ // else statement
			System.out.println("a and b are equal");
		}
	
	}
}
```

