
---
title : Binary Search
noteOrder : 98

---

### Introduction

We could probably call the linear search the bubble sort of searching. The linear search, although simple, is extremely inefficient and slow. To check for a single value, it'll have to check every one of the elements of the array.

A faster alternative is the Binary search. The binary search might be a bit confusing, but it's a really  useful algorithm. In this lesson, you'll learn how it works and how to implement it in a real Java program. 

### Video lesson

![Binary Search in Java](https://youtu.be/nNOeytz8O6U?si=GlV-JGQIWs9rCQuU)


### Syntax

The following program can be used to implement the binary search in a real program. Notice how I used "a.length-1" for the last index number. This is useful if you don't know what the last index number is. 

```Java
public class BinarySearch{
	public static void main(String[]args){
		 int [] a = {2, 13, 17, 34, 67};
		 int lower = 0;
		 int upper = a.length - 1;
		 int target = 11;
		 int middle = (upper + lower)/2;
		 while(upper>lower){
			 middle = (upper+lower) / 2;
			 if(target == a[middle]){
				 System.out.println("element found!");
				 break;
			 }
			 else if(target>a[middle]){
				 lower = middle+ 1;
				 break;
			 }
			 else if(target < a[middle]){
				 upper = middle - 1;
				 break;
			 }
		 }
		 if(upper>lower){
			 System.out.println("element not found!");
		 }	 
		 
	}
}
```

