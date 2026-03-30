
---
title: Bubble Sort
noteOrder : 94

---

### Introduction

In previous lessons, we learnt how arrays are helpful in storing multiple values as a single collection. We also learnt how to use loops to iterate arrays. When you store a large number of values in arrays, you need to find good ways to manage the data or the values. 

This is where sorting and searching becomes important. I'll talk about searching in the next section. For now, we can focus on sorting. Sorting is when we arrange the elements of an array into a particular order, usually an ascending or a descending order. Using a loop, we would iterate the array and rearrange the elements until they are sorted in this particular order.

Sorting is really important. Even when you open a channel page and check the videos, you get options allowing you to sort the videos from latest to oldest or most popular to least popular. When dealing  with arrays containing thousands of elements, it is important to use efficient sorting algorithms to arrange data quickly. There are multiple sorting algorithms, but we'll only look at two of them. In this lesson, you'll learn about the bubble sort.

An important thing I want you to remember is that any sorting algorithm works the same in any programming language. I recommend understand the general idea behind the sorting algorithm. If you know that well, implementing it in a program shouldn't be too difficult. 

### Video lesson

![Bubble sort in Java](https://youtu.be/D6Izk82DVAA?si=XNgsPzEeHfsr-AyZ)


### Syntax

The following program shows how to use the bubble sort to sort an array in an ascending order.

```Java
public class BubbleSort{
	 public static void main(String[]args){
	 
		 int [] a = {1, 55, 12, 11, 13};
		 int temp = 0;
		 for(int i = 0; i<a.length; i++){
			 for(int j = 0; j<a.length; j++){
				 if(a[j]>a[j+1]){
				 //swapping
					temp = a[j+1];
					a[j+1] = a[j];
					a[j] = temp; 
				 }
			 }
		 }
	 
	 }
}
```
