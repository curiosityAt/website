
---
title : Maximum value
noteOrder : 90

---

### Introduction

By now, you should be good with using loops to iterate arrays. In this lesson and the next few lessons, I'll show you a few useful and important programs involving array iteration. 

There are multiple ways to create the same program, so I encourage you to figure out the programs yourself before watching the video lessons. 

In this lesson, I'll show you an easy way to use a loop to iterate an array and find the maximum value. This is useful when you don't know what the elements in an array are and want and easy way to find and locate the maximum value. 

### Video lesson

![Finding the maximum value in an array](https://youtu.be/Cqg_0e2Nl_E?si=CfhxLKskNIhOTLqx)

### Syntax

The following program can be used to find and display the maximum value in an int array.

```Java
public class Maximum{
	public static void main(String[]args){
		int [] check = {1, 44, 23, 15, 17};
		int max = check[0];
		for(int i = 0; i<check.length; check++){
			if(check[i]>max){
				max = check[i];
			}
		}
		System.out.println(max);
	}
}
```
