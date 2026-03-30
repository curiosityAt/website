
---
title : The static keyword
noteOrder : 65

---

### Introduction

The static keyword was something that confused me a lot when I was learning Object Oriented Programming for the first time. It's a really important keyword. It's used for both [[Variables and methods|variables and methods]]. If you use it with a variable, we would call the variable a static variable. Similarly, methods with the static keyword are called static methods. I think the video lesson does a really good job of explaining exactly what it means and how it would work for both variables and methods.

### Video lesson

![Static keyword in Java](https://youtu.be/ZVVur1F53kU?si=_mOulMJ-I0V1zDF1)


### Syntax

The following simple program demonstrates the use of the static keyword with both variables and methods.

```Java
class Superhero{
	
	private String name; // non-static variable 
	private static int goodThings; // goodThings is a static variable
	
	public void incrementGoodThings(){ // non-static method
		goodThings++;
	}
	
	public static int getGoodThings(){ // static method
		return goodThings;
	}

}
```