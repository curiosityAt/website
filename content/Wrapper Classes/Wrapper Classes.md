
---
title : Wrapper classes
noteOrder : 74

---

### Introduction

If you've come along this far in learning Java, you should already know what [[03 Data types|primitive data types]]
are. These are data types like int, short, float or double. They are inbuilt into the programming language. You should also have a good idea of [[Using Classes and Objects|classes and objects]]. These are user-defined data types with variables as attributes and behaviours as methods. 

Although classes and objects can't be used as easily as primitive data types, we've seen how they are still extremely useful. Just like you would create variables to store values of primitive data types, you can use classes and objects to create objects. You can also use multiple methods with the object.  This is why Java provides class versions of the primitive data types. These classes are said to "wrap" the primitive data types, hence the name wrapper classes.

By the end of this video lesson, you'll have a good idea of what wrapper classes are and how you can use them in a program.

### Video lesson

![Wrapper classes in Java](https://youtu.be/Leh9kWGcClE?si=oxaDvfIxydjc7Y5f)

### Syntax

The following code demonstrates how we can create objects of the wrapper class and use autoboxing and unboxing. 

```Java
public class WrapperClasses{
	public static void main(String[]args){
	
		Integer intObj = new Integer(5); //wrapping the primitive value 5.
		Boolean boolObj = true; //autoboxing
		System.out.println(boolObj); //unboxing
	}
}

```




