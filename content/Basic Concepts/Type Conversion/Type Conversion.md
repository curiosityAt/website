
---
title : Type Conversion
noteOrder : 14

---

### Introduction

In Java, you'll often find it necessary to convert from one data type to another. Let's say I have an int value for the radius of a circle and I want to use this to calculate the area of the circle. We know that

$$  
Area = \pi r^2  
$$

The value of area will obviously be a decimal number, so area would be a double value. Here, I'll need to convert the int value for radius into a double to find a double answer. This process of converting a value of a particular data type into another data type is called type conversion and there are two methods of type conversion : Implicit and Explicit type conversion.

### Video lesson


### Syntax

```Java
public class UnaryOperators{
	public static void main(String[]args){
	
		double val = 6; // Implicit Type Conversion
		int val2 = (int)12.5 // Explicit Type Conversion	
			
}
```

