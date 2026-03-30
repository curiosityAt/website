
---
title : Linear Search
noteOrder : 97

---

### Introduction

As simple as it sounds, searching for an element in an array can be pretty difficult. In an array with hundreds of elements, it wouldn't make sense to print all the elements and manually look for a particular element. 

To simplify this, we use loops. Usually, we take a target value as input. This is the value we're searching for. By iterating the array with a loop, we can check for the target value. I recommend you to try to  figure out the program yourself before watching the video.

In this lesson, you'll learn about a simple searching algorithm called the linear search. 

### Video lesson

![Linear search in Java](https://youtu.be/9NHXcYx59Pk?si=lv8oSHFx1QnueMr5)


### Syntax

The following program can be used to implement the linear search in Java

```Java
public class LinearSearch{
	public static void main(String[]args){
		int [] a = {1, 12, 15, 6, 19, 20};
		int search = 15; //element to search for
		int check = 0;
		for(int i = 0; i<a.length; i++){
			if(a[i] == search){
				System.out.println("element found!");
				check  = 1;
			}
		}
		if(check==0){
			System.out.println("element not found!");
		}
	}
}
```
