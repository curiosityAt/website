
---
title : Unary operators
noteOrder : 8

---

### Introduction

If you watched the video lesson on arithmetic operators, you'll know that operators like  ( + ), ( - ), ( * ) , or ( / ) are called binary operators since they perform an operation on two operands. For example, If I add two numbers

```
3 + 5 = 8
```

you can see that the plus operator, being a binary operator, acts on the two operands 3 and 5.

Java also allows us to perform arithmetic operations on a single value and gives us operators to do this. Since these operators act on a single value, we call them unary operators. There are multiple unary operators, but the important ones you'll need to know are the increment operator, decrement operator and the logical not operator. You'll learn about the logical not operator in a later lesson on Logical operators. In this lesson, you're going to be learning about the increment and decrement operators and how to evaluate arithmetic expressions using them. 

### Video lesson

![Unary Operators in Java](https://youtu.be/6JKODsUvBw0)

### Syntax

```Java
public class UnaryOperators{
	public static void main(String[]args){
		int a = 3;
		int b = 5;
		int textExp = a++; // Post-increment Operator
		int textExp2 = b--; // Post-decrement Operator
		int textExp3 = ++b; // Pre-Increment Operator
		int textExp4 = --a; // Pre-Decrement Operator
		
		int expression =  (--a) + b-- + --b;// Expression using unary operators
		System.out.println(expression);	
		}
}
```



