
---
title : Math Class Methods - Part 1
noteOrder : 18

---

### Introduction

Using [[05 Arithmetic Operators|arithmetic operators]], we can perform simple arithmetic operations like addition, subtraction, multiplication, division or modulus, but they're not enough for more complex operations like finding the exponent of a number or the square root of a number. For such operations, we use an  in-built class in Java called the math class. 

The math class has many useful methods for complex mathematical operations. In this lesson, you're going to learn about the sqrt( ), cbrt( ), pow( ), max( ), min( ), and abs( ) methods. I'll talk about the other methods in the [[02 Math Class Methods part 2|next lesson]] 

### Video lesson

![Math class Methods part 1](https://youtu.be/9eDzPaHHB0g?si=5y1NNuZM-Go70b1V)

### Syntax

```Java
public class MathClassMethods{
	public static void main(String[]args){
		int numOne = 25;
		int numTwo = 19;
		
		double root = Math.sqrt(numOne); // sqrt() method
		double cubeRoot = Math.cbrt(125); // cbrt() method
		double power = Math.pow(19 , 2); // pow() method
		int maxx = Math.max(numOne, numTwo); // max() method
		int minn = Math.min(numOne, numTwo); // min() method
		int absolute = Math.abs(-3); // abs() method	
	}
}
```





