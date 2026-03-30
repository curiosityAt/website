
---
title : Constructors
noteOrder : 65

---

### Introduction

Previously, I showed you how to create specific methods to set the values of the instance variables by taking the values as parameters from the user. These methods are useful for initialising the instance variables and for changing their values whenever you want. In this lesson, you'll learn about something called constructors. In most classes, we prefer to use constructors over setter methods to initialise the instance variables.  

In this lesson, I'll show you what constructors are and why they are so useful in initialising the instance variables.


### Video lesson


![Creating and using constructors](https://youtu.be/k8g2M7kT8QQ?si=XnHU914sKeulQus2)


### Syntax

In the previous lessons on [[Variables and methods|instance variables and methods]], we created a class called Rocket. Then, we created setter methods to initialise the variables for the age and colour of the Rocket. To show the syntax for creating constructors, I'll replace the setter methods of the class with a constructor.


```Java
class Rocket{
	private String colour;
	private int age;
	
	public Rocket(String colours, int ages){ // constructor
		colour = colours;
		age = ages;		
	}
	
	public void getColour(){ // method to display colour 
		System.out.println(colour);
	}
	
	public void getAge(){ // method to display age
		System.out.println(age);
	}
	
}
public class ClassesObjects{
	public static void main(String[]args){
		Rocket obj = new Rocket("red", "12");
		obj.getColour();
	}

}
```