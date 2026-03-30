
---
title : Immutability
noteOrder : 104

---

### Introduction

By now, you should be familiar with many [[03 Data types|primitive and non primitive data types]]. Over the past many lessons on arrays or Object Oriented Programming, we've focused more on non-primitive data types.

However, an important characteristic of data types that I haven't mentioned till now is what's called immutability. This applies to non-primitive data types. Some non-primitive data types are called "mutable" and other non-primitive data types are said to be "immutable". 

For example, [[Introduction to arrays|arrays]] are said to be mutable while strings are called immutable. In many cases, the output of your code could also be affected by whether the data type you're using is mutable or immutable. In this video lesson, you'll learn exactly what this means

### Video lesson

![Mutable and immutable data types in Java](https://youtu.be/XYP87Y972OQ?si=28t3BrqcZFeIwpsv)


### Syntax

```Java
public class Immutability{
	public static void main(String[]args){
		//arrays as mutable data types
		double a [] = {3.14, 6.8, 1.2, 1.0};
		double b [] = a;
		System.out.println(b[0]); // this would print 3.14
		
		//Strings as immutable data types
		
		String obj = "hi";
		String obj2 = obj;
		obj2 = "hello";
		System.out.println(obj); //this would print "hi" 
	
	}
}
```