
---
title : Ternary Operator
noteOrder : 27

---

### Introduction

By now, you should know that operators in Java are generally classified based on the number of operands they act on. Binary operators are called "Binary" because they act on two operands. Unary Operators are called "Unary" because they act on a single operand. Similarly, the ternary operator is called "ternary" since it acts on three operands. Even though its an operator, I chose to include it under "Conditional Statements" and not "Operators" since they function similar to an if-else statement. This is why it's common to replace a simple if-else statement with a ternary operator expression. 

In this lesson, you're going to learn about the working of a ternary operator and how it's similar to conditional statements or constructs like the if-else construct.

### Video Lesson



### Syntax

```Java
public class TernaryOperator{
	public static void main(String[]args){
	// An if-else statement to check two numbers are equal
		boolean boolOne = false;
		int varOne = 5;
		int varTwo = 5;
		if(varOne==varTwo){
			boolOne = true;
		}
		else{
		    boolOne = false;
		}
	// The same block of code re-written using a ternary operator
		int varThree = 5;
		int varFour = 5;
		
		boolean boolTwo = (varThree == varFour)? true : false;
		
	}
}
```






