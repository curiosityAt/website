
---
title : Constructor Overloading
noteOrder : 66

---

### Introduction

Now that you understand how to [[Constructors|create a constructor]] in a class to initialise the instance variables of the class, we'll see how we can create multiple constructors in the same class using constructor overloading. In this lesson, you'll see how constructor overloading, by providing different ways to initialise the instance variables, is extremely useful. 

### Video lesson


![Constructor overloading in Java](https://youtu.be/PVrWXM8W99o?si=OedkHrkcA1H1C4ip)


### Syntax

To show how constructor overloading would work in a real program, I took a class called Superhero and I created two constructors. I took one constructor that takes no parameters and initialises all variables to the default values, and I took a different constructor to take parameters to take parameters and initialise the variables. 

```Java
class Superhero{
	private String name;
	private String power;
	private int age;
	
	public Superhero(){ // the first constructor
		name = null;
		power = null;
		age = 0;
	}
	
	public Superhero(String n, String p, int a){ // the second constructor
		name = n;
		power = p;
		age = a;
	}
	
	public String getName(){ // method to return the name
		return name;
	}
	public String getPower(){ // method to return the power
		return power;	
	}
	public String getAge(){ // method to return the age
		return age;
	}
	
}

public class ConstructorOverloading{
	public static void main(String[]args){
	
		// object using the first constructor	
		Superhero obj1 = new Superhero();
		
		// object using the second constructor	
		Superhero obj2 = new Superhero("superman", "strong", 30); 
		
	}
}
```

