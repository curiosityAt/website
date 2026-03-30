
---
title : Minimum value
noteOrder : 91

---

### Introduction

In the last lesson, I showed you a simple program to find the maximum value in an array. With just a few changes, you can use the same program to find the smallest value in an array. It's not too different, so I hope you try this program out yourself.

### Video lesson

![Finding the minimum value](https://youtu.be/2FEExB28IEU?si=aTS3e9nQ4ySXOasW)


### Syntax

The following program can be used to find and display the minimum value in a double array. 

```Java
public class Minimum{
	public static void main(String[]args){
		double [] check = {1.5, 13.76, 12.3, 1.1, 15.67};
		double min = check[0];
		for(int i = 0; i<check.length; check++){
			if(check[i]<min){
				min =  check[i];
			}
		}
		System.out.println(min);
	}
}
```
