
---
title : Method Overloading
noteOrder : 62

---

### Introduction

Previously, we looked at [[Constructor Overloading|Constructor Overloading]] where we were able to create multiple constructors. This was really useful for multiple reasons. In my class, overloading the constructors gives me different options to initialise the variables. 

For example, let's take a class called "Superhero" with the instance variables name and age. If I want to initialise the variables to the default values, I can use a default constructor like this:

```Java
public Superhero(){
	name = "";
	age = 22;
	}
```

If I want the user to enter the values for name and age, I could add another constructor with those two parameters. This constructor would look like this

```Java
public Superhero(String n, int a){
	name = n;
	age = a;
}
```


In my class, both the constructors would co-exist. This is a much better way of initialising the variables of our class. 

The great thing is that we can do something like this with methods as well. We can use multiple methods with the same name, but different parameters. Like you've seen with constructor overloading, method overloading just gives us different options. 

To show why, we'll take a simple example. Let's say I want to make a class and add methods to calculate the areas of different shapes. I'll have to make a different method for a different shape, and my class would end up with multiple methods like areaRect( ), areaCircle( ), areaSquare( ), and so on. It isn't convenient for a user to use multiple methods to calculate the area.

Instead, we can create just one method area( ) and overload it. Depending on the number of parameters or the data type of the parameters the user enters, we would call a particular method and find the area of the shape accordingly. Watch the video lesson to see how I used method overloading to do this.

### Video lesson

![Method overloading in Java](https://youtu.be/ZQk5ddaIVwc?si=R0OroYcrN1PL3qqD)


### Syntax

```Java
public class Shapes{
	private double area;
	public double area(int radius){ // method 1 for circle area
		area = 3.14 * radius * radius;
		return area;
	}
	public double area(double base, int height){ // method 2 for triangle area
		area  = 0.5 * base* height;
	}
	
	public double area(int breadth, int length){ // method 3 for rectangle area
		area = breadth* length;
		return area;
	}
	
	public static void main(String[]args){
		Shapes obj = new Shapes();
		areaCircle = obj.area(2.5); //to call method 1
		areaTriangle = obj.area(2.4, 12); //to call method 2
		areaRect = obj.area(12, 13); //to call method 3
	}
}
```
