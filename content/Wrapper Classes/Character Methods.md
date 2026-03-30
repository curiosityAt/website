
---
title : Character Class
noteOrder : 75

---

### Introduction

The [[Wrapper Classes|previous lesson]] was a good introduction to understanding wrapper classes and how they're helpful in a program. However, there was one wrapper class I didn't mention before. This is the Character wrapper class. The Character wrapper class is extremely useful since it contains many important methods. In this video lesson, you'll learn about some of these methods.

### Video lesson

![Character Class Methods Java](https://youtu.be/3p0a7WaOAy4)

### Syntax

The following code shows the syntax for the Character class methods

```Java
public class CharacterClassMethods{
	public static void main(String[]args){
		char varOne = 'a';
		char varTwo = '$';
		char varThree = '6';
		
		// The eight Character class methods
		
		boolean val1 = Character.isDigit(varOne);
		boolean val2 = Character.isLetter(varThree);
		boolean val3 = Character.isLetterOrDigit(varThree);
		boolean val4 = Character.isUpperCase(varThree);
		boolean val5 = Character.isLowerCase('B');
		boolean val6 = Character.isWhiteSpace(' ');
		char val7 = Character.toUpperCase(varOne);
		char val8 = Character.toLowerCase('F');	
	}
}

```



