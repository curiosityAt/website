
---
title : Logical Operators
noteOrder : 12

---

### Introduction

Although relational or arithmetic operators are something we use a lot in real life, logical operators might be something entirely new. In Java, we deal a lot with logical expressions : expressions that evaluate either to a true or a false. As you'll see in later lessons, they're really useful! To implement such logical expressions in a program, we'll have to use a few operators called logical operators. In this lesson, you'll learn about the three main types of logical operators and how we can use them to create or evaluate the output of logical expressions.

### Video Lesson


### Syntax


```Java
public class LogicalOperators{
	public static void main(String[]args){
		boolean boolVar = (3>6)||(5!=8); // Logical expression
		System.out.println(boolVar); // printing the value of the expression
		                                		
		}
}
```