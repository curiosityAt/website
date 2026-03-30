
---
title : String methods part 1
noteOrder : 101

---

### Introduction

"String" is actually a class in Java. Whenever we create a String, we're just creating an object of this "String" class. Being a class, the "String" class also contains multiple methods.

These methods are really important and they make it much easier to use Strings. Although there are many methods in the String class, in this lesson and the [[String methods part 2|next lesson]], we'll only look at a few important methods. 

In this lesson, you'll be learning about the length( ), charAt( ), indexOf( ), lastIndexOf( ), toUpperCase( ), toLowerCase( ), and the equals( ) methods.

### Video Lesson

![String methods in Java](https://youtu.be/LtTeZTut3bg?si=6u9ctqJqkH2d_c_b)


### Syntax

The following block of code shows the syntax for using different String methods.

```Java
public class StringsInJava{
	public static void main(String[]args){
		String strOne = "Welcome!";
		
		int strLength = strOne.length();
		char temp = strOne.charAt(3);
		int firstIndex = strOne.indexOf('e');
		int lastIndex = strOne.lastIndexOf('e');
		String capital = strOne.toUpperCase();
		String small = strOne.toLowerCase();
		boolean check = strOne.equals("hello!");
	}
}
```
