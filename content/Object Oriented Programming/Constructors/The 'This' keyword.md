
---
title : this keyword
noteOrder : 66

---

### Introduction

By now, you should have a good idea of what [[Constructors|constructors]] are and how to use them. In the video lesson on constructors, I showed you how to initialise the instance variables by using the parameters of the constructor. 

This was the constructor I used

```Java
public Rocket(String colours, int ages){ // constructor
		colour = colours;
		age = ages;		
	}
```

In this constructor,  something important you need to notice is that the parameter names are not the same as the names of the instance variables. I did this on purpose.

You might think that using the same name is not possible since two variables can't have the same name, but since the parameter is a local variable (local to the method), this is actually allowed. Two instance variables can't have the same name. Two parameters of a single method also can't have the same name, but a local variable and an instance variable can have the same name. 

The actual reason I gave them different names is because of what happens inside a method. Let's take the constructor again and let's give the parameter 'colours' the same name as the instance variable 'colour'.

```Java
public Rocket(String colour, int ages){ // constructor
		colour = colour;
		age = ages;		
	}
```

Inside the method, we're just setting the value of the 'colour' variable to the 'colour' variable, but there is an instance variable 'colour' and a local variable 'colour'. What variable are we referring to?

In Java, whenever you're inside a method, if the instance variable and the local variable have the same name, Java would always access the local variable. So here, we're just setting the value of the local variable 'colour' to the local variable or parameter 'colour'. We're not changing the instance variable! 

To make it easier to differentiate between the instance variables and local variables in situations like these, we would use the 'this' keyword. Even though I added this lesson as a part of Constructors, it can be used anywhere in  a class. You'll understand how to use the 'this' keyword in the video lesson

### Video lesson


![The 'this' keyword in Java](https://youtu.be/qBhr2qVZEyM?si=GUSqVpkfeDIBRRN_)

### Syntax


The following simple program demonstrates how to use the 'this' keyword.

```Java
class Student{
	private String name;
	private int age;
	private String favSubject;
	
	public Student(String name, int age, String favSubject){
		this.name = name; //this.name refers to the instance variable name
		this.age = age; 
		this.favSubject = favSubject;
	}
	public String getName(){
		return name;
	}
	public int getAge(){
		return age;
	}
	public String getSubject(){
		return favSubject;
	}
}
```
