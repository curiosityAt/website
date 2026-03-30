
---
title : Introduction to arrays
noteOrder : 80

---

### Introduction

Arrays are an example of non-primitive data types which are used to  store a collection of data.  To understand this better, we'll take an example.

Let's say that you own a company and you need to store the details of all the employees at your company. You'll need to store their name and age. You can do this using variables. I  can create a name, age, and phone number variable  for each employee. If I do that for two employees, our program would look like this

```Java
public class Company{
	public static void main(String[]args){
		//details of employee 1
		String name1 = "employee name";
		int age1 = 25;
		
		//details of employee 2
		String name2 = "employee name";
		int age2 = 33;
	}
}
```

Although this works, it's a very inefficient solution. If my company had a thousand workers, I can't just keep creating variables. Not only is it hard to create variables, it's also impossible to manage all of them!

This is where arrays come in. Arrays just store collections of data. Instead of creating multiple variables for multiple values, you can just store all the values in one array. 

The array is said to store all these values in "contiguous memory locations". This just means that the values are not stored in random spaces in the memory. A single part of the memory is allocated to store the elements of the array and all the elements are stored together. 

To show you how easy it is to create and use arrays, I'll take our previous example and I'll make an array to store the names of a thousand employees. Even though you might not understand the syntax, you'll still get a good idea of why arrays are useful.

```Java
public class Company{
	public static void main(String[]args){
		
		String [] names = new String[1000]; 
		
}
```

Something that would have needed me to create a thousand variables can be done using a single array.

In this video lesson, you'll learn how to declare, initialise and use arrays in Java.

### Video lesson

![Arrays - Declaration, initialisation,  and use](https://youtu.be/ZK0wnWTsvhU?si=lObydo1gIzSwQWsv)

### Syntax

The following lines of code show the important syntax you'll need to know to create and use arrays.

```Java
public class Arrays{
	public static void main(String[]args){
		int [] age = new int[5]; //creating an empty array
		char arr [] = {'a', '#', '9', '5'}; // using an initialiser list
		
		age[3] = 15; //setting the value of element at index 3
		System.out.println(age[2]); // printing the element at index 2
	}
}
```
