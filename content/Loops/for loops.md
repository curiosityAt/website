
---
title : for loops
noteOrder : 36

---

### Introduction

[[While loops and do - while loops|While loops and do-while loops]] had really simple syntax. While a particular condition was true, they would keep executing a block of code. For loops, being loops, do the same thing. They would execute a block of code as long as a condition is true, however the arrangement of the different parts of the loop like the initialisation of the iterator, the update and the condition is different. 

If they're so similar, then when do we use while loops and when do we use for loops? If you look at the syntax of a for loop, you'll notice that you'll have to mention the initial value of the iterator and the condition in the loop heading. Therefore, for loops are useful if you already know the number of times you want to execute the loop.

When you're not sure how many times the loop has to execute, you can use a while loop. A while loop offers more freedom in terms of the syntax. 

### Video lesson

![For loops in Java](https://youtu.be/e4XPDeEhLeQ)

### Syntax

In the last lesson, I used a while loop and a do-while loop to print the word "hello" ten times. We'll do the same thing using a for loop

```Java
public class Loops{
	public static void main(String[]args){
		// using a for loop to print "hello" ten times
		for(int i = 1; i<=10; i++){
			System.out.println("hello");
		}
		
	}
}
```