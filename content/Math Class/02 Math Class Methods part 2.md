
---
title : Math Class Methods- Part 2
noteOrder : 19

---

### Introduction

Now that you understand how simple methods like the max( ) or min( ) methods work, we'll look at four more useful methods : the round( ), ceil( ), floor( ), and the random( ) method. It's important to remember the parameters and return data types for the method if you want to store the result or the value returned in variables.

### Video lesson

![Math class methods part 2](https://youtu.be/0r0IhCqIr8E?si=6192sMqF3l85wwHr)

### Syntax

```Java
public class MathClassMethods{
	public static void main(String[]args){
		double val1 = 12.334;
		double val2 = 1.215;
		
		double rounds = Math.round(val1);
		double roundHigh = Math.ceil(val2);
		double roundLow = Math.floor(val1);
		double randNum = Math.random();
	}
}
```
