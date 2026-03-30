
---
title : String iteration
noteOrder : 105

---

### Introduction

Although strings in Java are actually objects of the class "String", they are really similar to arrays. Strings are an array or a collection of characters. Any string can be split into an array of characters and every one of these characters has an index numbers just like the elements of an array.

Before, you might have used these index numbers with the "String" class methods. Something else we can do using the index numbers and the "String" class methods is iterate the Strings.

Iteration isn't entirely new to you. Before, you might have used [[Iterating Arrays using loops|iteration with arrays]]. Using a for-loop or a while-loop, we could access each element of an array in every iteration of the loop. String iteration is the exact same thing. Using a loop, we can access every character of the String in every iteration of the loop.

In this video lesson, you'll learn how to use loops to iterate Strings.

### Video lesson


![String iteration](https://youtu.be/DYZNYhOqOAQ?si=2DOYPqrEUt1BQBin)


### Syntax

The following program uses a loop to iterate and print the characters of a String. Note the similarities between String and array iteration.

```Java
public class StringIteration{
	public static void main(String[]args){
		String str = "For loops are everywhere!";
		for(int i = 0; i<str.length(); i++){
			char temp = str.charAt(i);
			System.out.println(temp);
		}
	
	}
}
```
