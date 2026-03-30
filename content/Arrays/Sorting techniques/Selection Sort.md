
---
title : Selection sort
noteOrder : 95

---

### Introduction

If you remember, the bubble sort was a very simple sorting algorithm. It's probably the simplest sorting algorithm out there! All we did was swap consecutive elements till the array is completely sorted.

However, by manually iterating the loops, you could see that it's a really slow process. A better and faster way to sort an array is using what's called a selection sort. 

As you'll see in this lesson, It's really simple to understand and is much more efficient than a bubble sort.

### Video lesson


![Selection sort in Java](https://youtu.be/h4l7Eh6pAac?si=BrNUTy6XSoXGmtpo)


### Syntax

The following program shows how to use the selection sort to sort an array in an ascending order.

```Java
public class SelectionSort{
	public static void main(String[]args){
		int[]a = {1, 5,  6, 7, 12};
		int min = 0;
		int temp = 0;
		for(int i = 0; i<a.length; i++){
			min = i;
			for(int j = i; j<a.length; j++){
				if(a[j]<a[min]){
					min = j;
				}				
			}
			//swapping
			temp = a[min];
			a[min]=a[i];
			a[i] = temp;
		}
	}
}
```


