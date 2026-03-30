
---
title : Sum of elements
noteOrder : 92

---

### Introduction

Another useful thing you can do with array iteration is finding the sum of all the elements of an array. If you understand loops well, this should be familiar.

Previously, we looked at something like this when we tried to find the sum of the terms of a series. We created a variable to add each element every iteration and find the total sum. Here, we're doing the same thing except we're adding each element of the array every iteration of the loop. 

Try to figure this out yourself before watching the video lesson.

### Video lesson

![Finding the sum of elements of an array](https://youtu.be/JMvgq9DnfiI?si=n8JdZORl8pFZvCl5)


### Syntax

The following program can be used to find and display the sum of the elements of an array.

```Java
public class ElementsSum{
	public static void main(String[]args){
		int [] arrOne = {21, 44, 11, 12, 4};
		int sum = 0;
		for(int i = 0; i<arrOne.length; i++){
			sum = sum + arrOne[i];	
		}
		System.out.println(sum);
	}
}
```