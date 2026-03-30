
---
title : Finding the sum of digits
noteOrder : 44

---

As you'll see in later practice questions as well, finding the sum of the digits of a number is very useful. If I have a number, I can find the sum of the digits using the modulus operator. For example, if I take a number like 35. I can write the following program to find the sum of the digits 3 and 5 as 8.

```Java
public class DigitsSum{
	public static void main(String[]args){
		int n = 35;
		sum = sum + n % 10;
		n = n/10;
		sum = sum + n % 10;
		System.out.println(sum + " is the sum of the digits");
	}
}
```

If you look at the program, you can clearly see that all I'm doing is taking each digit and adding it to a common variable sum to find the sum of all the digits. The issue here is that this program will only work for two-digit numbers like 35. To make sure that the program works for any number, we can use loops.

Try to solve the question yourself before watching the video solution.

### Question to find the sum of the digits of a number


![[Pasted image 20260313201733.png|620]]


### Video solution


![Sum of digits - video solution](https://youtu.be/QdbYIa363Xc)