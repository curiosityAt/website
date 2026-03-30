
---
title : Entry-controlled vs exit-controlled loops
noteOrder : 37

---

### Introduction

If you watched both the video lessons on [[for loops|for loops]] and [[While loops and do - while loops|while loops]], you should know what exit-controlled and entry-controlled loops mean.  If you understood the difference, you can move on to the next lesson. If something's still confusing you, I recommend reading through this text lesson.
### Entry controlled loops

Both for-loops and while loops are called entry controlled loops. The meaning is in the name itself! Any loop works the same way. It keeps executing a block of code as long as a condition is true. "Entry controlled" just means that the condition controls when we enter the loop. 

Let's say that I want to use a for loop to print all the numbers from 1 to 100. The loop would look like this

```Java
public class Loops{
	public static void main(String[]args){
		for(int i = 1; i<=100; i++){
			System.out.println(i);
		}
	}
}
```

You can see that we always check the condition first before we enter the loop. The block of code in the loop is executed only when the condition is true. This is why we call it an entry-controlled loop.

A while loop works the exact same way. Here's a while loop printing numbers from 1 to 100.

```Java
public class Loops{
	public static void main(String[]args){
		int i = 1;
		while(i<=100){
			System.out.println(i);
		}
	}
}
```

Even here, you always check the condition first. If the condition is true, we would execute the block of code in the loop. In both cases, the syntax of the loop is such that the entry into the loop is decided by the condition.

### Exit controlled loop

As you would expect, an exit controlled loop is just the opposite. For entry controlled loops, the condition determined the entry into the loop. For exit controlled loops, the condition determines the exit from the loop. The do-while loop is an exit controlled loop.

Let's rewrite the same program to print a hundred numbers using a do-while loop.

```Java
public class Loops{
	public static void main(String[]args){
		int i = 1;
		do{
			System.out.println(i);
			i++;
		}
		while(i<=100);
	}
}
```

Here, we run the block of code first and then check the condition to see if we would exit the loop or not. If the condition is true, we would stop executing the loop. Now, the order of the syntax is such that, the exit from the loop is decided by the condition.

You might have a question. If we run the block of code before checking the condition, does this mean that we'll run the block of code at least once even if the condition is false?  The answer is yes. To understand why, let's take a loop at this loop

```Java
public class Loops{
	public static void main(String[]args){
		int i = 1;
		do{
			System.out.println(i);
			i++;
		}
		while(i > 5);
	}
}
```

Here, our condition is obviously false. The initial value of i is 1 and "1>5" is false. However, since the block of code is executed first, we would execute the block of code and then check the condition. You would see a 1 on your output window and i would increase to 2, and then the condition would check if 2 is greater than 5. This is false, so we would stop executing the loop.

