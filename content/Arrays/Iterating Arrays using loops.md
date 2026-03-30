
---
title : Array iteration
noteOrder : 88

---

### Introduction

Using arrays, we can create and store large collections of data. We can access whatever elements whenever we want. However, arrays become a lot more useful when you use loops with them.

To understand this, Let's continue with the example from the previous lesson about a company wanting to store the details of its thousand employees. Let's say that this company wants to create a method increase( ) to increase the age of every employee by one after every year. Basically, the method needs to increase every element by one. 

How could we do this in a program?

One thing I could do is access and increase every element. If I do that, my increase() method would look like this

```Java
public class Company{ 
	public void increase(){ //method to increase every element by one
		age[0] = age[0] + 1;
		age[1] = age[1] + 1;
		age[2] = age[2] + 1;
		.
		.
		.
		.
		age[998] = age[998] + 1;
		age[999] = age[999] + 1;
		
	}	
}
```

There's no advantage with using arrays over creating variables if I have to write so many statements just to increase the elements by one. 

To make our process much faster, we use loops. We use the loop iterator as the index number so that in every single iteration of the loop, we access every element. This is called array iteration. You'll understand how and why this works in this video lesson.

### Video lesson


![Iterating arrays in Java](https://youtu.be/1G654ANfrNM?si=qtLY1-lj2_P0brgT)


### Syntax

To show the syntax for using arrays, I took the same example where we had to increase every element of the age array by one. 

```Java
public class Company{ 
	public void increase(){ //method to increase every element by one
		
		for(int i =1; i<age.length; i++){
			age[i] = age[i] + 1;
		}
		
	}	
}
```
