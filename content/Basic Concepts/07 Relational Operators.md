
---
title : Relational operators
noteOrder : 11

---

### Introduction

Relational operators are useful in comparing two different values. If we have two values, we can use relational operators to find if one value is greater than the other, lesser than the other, or even if they're both equal. Such expressions using relational operators either evaluate to a true or a false. We already learnt about such operators in math, so it shouldn't be too hard to understand how to use them in Java. 

### Video Lesson

![Relational Operators in Java](https://youtu.be/Auqz-uLTYTU?si=i085n71UBn4I9YOo)

### Syntax

```Java
public class RelationalOperators{
	public static void main(String[]args){
		boolean boolVar = (3>6)||(5!=8); // Logical expression
		System.out.println(boolVar); // printing the value of the expression
		    boolean exp1 =  = 3 > 5; // greater than
		    boolean exp2 = 1 < 6; // lesser than
		    boolean exp2 = 1 <= 6; // lesser than or equal to
		    boolean exp3 = 9 >= 5; // greater than or equal to 
		    boolean exp4 = 2 != 3; // not equal to
		    boolean exp5 = 2 == 1; // equal to 
	                       		
		}
}
```
