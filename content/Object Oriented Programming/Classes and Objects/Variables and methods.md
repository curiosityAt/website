
---
title : Variables and methods
noteOrder : 54

---

### Introduction

In the [[Using Classes and Objects|last lesson]], we learnt how to create a class and implement it using an object. There, I told you that every class contains characteristics and behaviours. 

The whole point of creating an object for a class is to use these characteristics and behaviours. You'll see soon that in an actual class, the characteristics are simply variables, and that the behaviours are the methods.

You'll be learning about the basic syntax for creating methods, different kinds of methods like setter or getter methods, parameters, and the return keyword.

### Video lesson


![Understanding instance variables and methods](https://youtu.be/ay0DMHKlMWs?si=5R_VnhHn5OVrNz6q)

### Syntax

To show the syntax for creating methods or variables in a class, I'll take the same program from the last lesson.

```Java
class Rocket{
	// Variables
	private String colour;
	private int age;
	
	//methods
	
	public void setColour(String colours){ //method to take colour as a parameter
		colour = colours;
	
	}
	
	public void getColour(){ // method to display the colour
		System.out.println(colour);
	}
	
	public void setAge(int ages){ // method to take age as a parameter
		age = ages;
	}
	
	public int getAge(){ // method to return the int value of the age variable
		return age;
	}
	
}
public class ClassesObjects{
	public static void main(String[]args){
		
		
		Rocket obj = new Rocket();
	}
}
```





