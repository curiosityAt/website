
---
title : String methods part 2
noteOrder : 102

---

### Introduction

In the [[String methods part 1|last lesson]], you learnt about several String class methods. This lesson, we'll look at a few more. These are really important methods and you'll use them a lot later on.

In this lesson, you'll learn about the substring( ), replace( ), concat( ), startsWith( ), endsWith( ) and the trim( ) methods. There is one more method called the compareTo( ) method. Check the next lesson if you want to learn about this method. I made it a separate lesson since it's a bit harder to understand. 
### Video lesson

![String methods part 2](https://youtu.be/WDUCv9VV66c?si=EDrGOFtg4jhBiprW)

### Syntax

The following block of code shows the different ways to use the methods of the string class. 

```Java
public class StringMethods{
	public static void main(String[]args){
		String obj = "Have a great day";
		String sub = obj.substring(2);
		String sub2 = "Fun with strings".substring(2, 7);
		String change = obj.replace('a' , 'e'); 
		String newerStr = obj.concat("!!!");
		boolean check = obj.startsWith("Have");
		boolean check2 - obj.endsWith("hi");
		boolean trimmed = " hello world   ".trim();	
	}
}
```


