
## Introduction

When you write a long program, you'll create many variables with different functions. To not just make it easier for you to understand the program you made, but to also make it easier for other programmers or other people to understand it and reuse it, it'll be really useful to write down exactly what parts of the program do in the program itself. This is done using comments.

However, we can't just type the text like code in a regular program since this is going to cause compile-time errors. Comments require us to use specific symbols that tell Java that it's a comment and that we want it to ignore it. If we do this, the compiler won't compile the comments. There are three types of comments you can use in a program.

## Single-Line Comment

Let's say that I created a program to find the sum of two numbers. The program would look like this

```Java
public class Addition{
	public static void main(String[]args){
		int var1 = 5;
		int var2 = 6;
		int sum = var1 + var2;
	}
}
```

This is a simple example and we can understand what the variable sum is supposed to do just from the name of the variable, but if I still wanted to clarify what it's doing, I can use a Single-line comment.

To use a single-line comment, we'll be using a double front slash ( // ). The whole line of code from wherever we used the double slash is commented out and ignored by the compiler. Therefore, I can write down my comment after the front slash. 

```Java
public class Addition{
	public static void main(String[]args){
		int var1 = 5;
		int var2 = 6;
		int sum = var1 + var2; // sum is storing the sum of the values
	}
}
```

You have to be careful with where you use the double front slash though. What if I used the double front slash at the beginning of the line

```Java
public class Addition{
	public static void main(String[]args){
		int var1 = 5;
		int var2 = 6;
		// int sum = var1 + var2;  sum is storing the sum of the values
	}
}
```

If we do that, you notice that the whole line including the sum variable is commented out. Whenever you're getting confused with parts of the program, you can use single-line comments to make short comments on the code.

## Multi-Line Comment

When all you want to do is add short one-line descriptions, single-line comments are enough, but sometimes you'll need  to add longer descriptions for parts of your code.  You can do this using multi-line comments. 

To create a multi-line comment we use ( $/*$  ) and  ( $*/$ ). 

$/*$  is a front slash followed by an asterisk. This indicates the start of a multi-line comment. $*/$ is an asterisk followed by a front slash. This indicates the end of a multi-line comment.

The compiler ignores whatever's written between the $/*$  and the $*/$

If we take the original program again

```Java
public class Addition{
	public static void main(String[]args){
		int var1 = 5;
		int var2 = 6;
		int sum = var1 + var2; 
	}
}
```

If I now wanted to add a comment to describe the program in a bunch of steps or points, I can use a multi-line comment.

```Java
public class Addition{
	public static void main(String[]args){
		int var1 = 5;
		int var2 = 6;
		int sum = var1 + var2; 
		/*
		1. We created a variable var1
		2. We created a variable var2
		3. We stored the sum of the variabls in a variable called sum
		*/
	}
}
```

You can see how useful these multi-line comments can get in large and complicated programs. One thing you'll need to ensure is that every starting $/*$  has an ending $*/$ 

If you don't end the multi-line comment, everything else in the program after the $/*$ will also get commented out. 

```Java
public class Addition{
	public static void main(String[]args){
		int var1 = 5;
		int var2 = 6;
		int sum = var1 + var2; 
		/*
		1. We created a variable var1
		2. We created a variable var2
		3. We stored the sum of the variabls in a variable called sum
		
	}
}
```

Without any of our ending brackets, we won't be able to execute our program. 

## Documentation Comments

Documentation comments are comments that you create at the beginning of the program to write down important information. This is usually information about the program in general : the name of the person who created the program, the date of creation of the program, the basic working of the classes and methods in the program, a description of the variables used, and much more. 

The syntax for creating a documentation comment is similar to a multi-line comment. 

To create a documentation comment, we use ( $/**$  ) and  ( $*/$ ). 

$/**$ is a front slash followed by two asterisks. $*/$ is an asterisk followed by a front slash. Any of the documentation is written between $/**$ and $*/$

If we create a documentation comment in the original program, it would look like this

```Java
/**
* Author : K.V. Siva Surya
* Date Created : 10/03/2026
* Class name : Addition
* To find the sum of two numbers
*/
public class Addition{
	public static void main(String[]args){
		int var1 = 5;
		int var2 = 6;
		int sum = var1 + var2; 
	}
}
```







