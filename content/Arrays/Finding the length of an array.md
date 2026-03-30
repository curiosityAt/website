
---
title : Finding array length
noteOrder : 88

---

### Length of an array

Most times, whenever you use arrays, you don't know the number of elements in the array. Lucky for us, Java provides a way to find and store the number of elements in the array. 

The data type defining arrays contains an instance variable called  "length". Like we've done before in Object Oriented Programming, we can access this instance variable using the name of the array  and the dot keyword.

The variable "length" is of the int data type, so we can store it in an int variable. In the following program, I created an array containing 20 elements called tester. I stored the length of the array in a variable arrLength and then printed the variable.

```Java
public class ArraysLength{
	public static void main(String[]args){
		int [] tester = new int [20];
		int arrLength = tester.length; 
		System.out.println(arrLength);
	}
}
```

An important thing you need to remember is that "length" is an instance variable and not a method. Whenever you want to find the length of the array, you're  going to use the keyword "length". 

The following statement is wrong syntax. Arrays don't have a method "length( )" that you can call. We'll be using the "length( )" method later with strings.

```
arr.length();
```

This variable length is also really useful in iterating arrays. 

In the lesson on array iteration, I told you that you can use the index number of an array to iterate the array. 

```Java
public class ArrayLength{
	public static void main(String[]args){
		int [] arrCheck = new int[5];
		for(int i = 0; i<=4; i++){
			System.out.println(arrCheck[i]);
		}
	}
}
```

In the above program, since the length of the array arrCheck is 5, the index number of the last element is 4. This is why I set my condition to "i<=4". We'll iterate the loop till the index number of the last element. We'll stop executing the loop when we reach the last element.

Alternatively, we can use the length of the array as well. The only thing to remember is that the length of the array is just one more than the index number of the last element. Since the length of the array  "arrCheck" is 5, I can use the following loop.

```Java
public class ArrayLength{
	public static void main(String[]args){
		int [] arrCheck = new int[5];
		for(int i = 0; i<5; i++){
			System.out.println(arrCheck[i]);
		}
	}
}
```

You can see that I changed the condition to "i<5". This will make sure that we keep executing the loop as long as i is lesser than the array length. We'll stop executing the loop when we reach 4. This is the index number of the last element. 

In cases where we don't know the number of elements the array has, we can access the length of the array using the length variable and use it as the condition of our for loop. Take a look at the following program. I just replaced 5 with "arrCheck.length" in the above program.

```Java
public class ArrayLength{
	public static void main(String[]args){
		int [] arrCheck = new int[5];
		for(int i = 0; i<arrCheck.length; i++){
			System.out.println(arrCheck[i]);
		}
	}
}
```


