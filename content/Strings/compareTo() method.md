
---
title : compareTo( ) method 
noteOrder : 103

---

### Introduction

By now, you should be good at using several useful String methods like the substring( ), equals( ), or the charAt( ) methods. There is one more important method called the compareTo( ) method. We can use it to compare two different Strings.

It might be a bit confusing to understand since there are many cases you'll need to know to properly use it. I explain all of them in the video lesson. 

### Video lesson

![compareTo( ) method](https://youtu.be/oD8w7xcTzZQ?si=R49d3OssSoKQefIy)


### Syntax

The following block of code shows the different cases involved with the compareTo( ) method. 

```Java
public class CompareToMethod{
	public static void main(String[]args){
		System.out.println("ball".compareTo("zebra"));
		System.out.println("tomato".compareTo("apple"));
		System.out.println("argon".compareTo("apple"));
		System.out.println("Apple".compareTo("apple"));
		System.out.println("app".compareTo("apple"));
		System.out.println("apple".compareTo("apple"));	
	}
}

```