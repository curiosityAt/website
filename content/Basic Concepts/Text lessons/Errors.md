
## Introduction

When you write a Java program, you'll usually encounter problems with your code. In Java (and most other programming languages), these errors are classified into three types : Logical Errors, Compile-time errors, or run-time errors. In this short text lesson, we'll take a look at what these errors mean and some common cases involving them.

## Compile-time errors

Compile-time errors are the most common type of errors. They're also known as syntax errors. Java has rules for how the code is written. When you want to write a println statement, you'll have to write 

```Java
System.out.println("errors are no fun");
```

You can't change this and write

```Java
system.out.println("errors are no fun");
```

They look the same, but if you notice, the second statement has a lower case "s". The syntax requires you to use an uppercase "s", so this would be an error.  Since it is a case-sensitive programming language, Java won't recognize the second statement and will give us an error.

Let's take another situation

```Java
int a = 3.14159;
```

What's the error here?  You notice that I'm trying to implicitly assign a double value to an int variable. The syntax is still wrong because Java cannot implicitly convert a double value to an int value and store it in the variable. If you go to your code editor, type the same code, and compile the program, you'll get an error that looks like this

```
Type mismatch: cannot convert from double to int
```

To fix the error, I'll just need to use explicit type conversion. I'll need to add an int before the double value to force the program to convert it to an int. This is correct and won't give us an error

```Java
int a = (int) 3.1456;
```

Finally, we'll look at a block of code with another compile-time error

```Java
System.out.println("be careful with compile-time errors")
```

Here, I didn't use a semicolon after the println statement. This is a very common compile-time error. 

If you notice, all syntax errors are detected after you compile the program. This is why we call them compile-time errors. To make sure you don't get any compile-time errors or compilation issues, you have to be careful with the syntax.

## Run-time errors

I told you that syntax errors are called compile-time errors since they're detected at the time of compilation. Similarly, run-time errors are just errors detected when you run the program. The compiler cannot detect these errors. These run-time errors are also called exceptions. 

As you program more, you'll encounter many types of run-time errors like the "ArrayIndexOutOfBoundsException" or the "NullPointerException". For now, to explain what run-time errors even mean, I'll show you a common run-time error. Take a look at the following block of code

```Java
int temp = 0;
System.out.println(33 / temp);
```

There's nothing wrong with the syntax, so you won't get any error during compilation, but you will get an error when you execute a program that looks like this

```
Exception in thread "main" java.lang.ArithmeticException: / by zero
```

The error is pretty self-explanatory. If you look at the block of code, you'll see that since temp is 0, dividing 33 by temp is not possible. Division by zero is mathematically undefined. This is why, when you execute the program, you'll get an exception or a run-time error. The compiler only checks for syntax. It doesn't plug in the values of the variables and test expressions. This is done during execution, so that's when we detect such run-time errors.

## Logical Errors

Compile-time errors and Run-time errors are caused when something wrong with your code is preventing you from executing the program. However, it is also possible to execute your program well and a get a good output, while making an error. 

For example, what if I wanted to write a program to calculate the perimeter of a rectangle with a length of 33 metres and a breadth of 45 metres. Let's say I use this block of code to find the perimeter of the rectangle.

```Java
int length = 33;
int breadth = 45;
int perimeter = length * breadth;
System.out.println(perimeter);
```

There's nothing wrong with the syntax, so I'm able to compile the program. I'm also not dividing by zero anywhere, so I can execute the program as well. However, is the code itself correct? I wanted to find the perimeter of a rectangle. We know that for a rectangle, 

$$  
Perimeter = 2 (l + b)  
$$
but in the block of code I used, we're calculating the perimeter as the length times breadth. Although we're able to compile and execute the program, the output itself is wrong. To fix it I'll need to rewrite the block of code as

```Java
int length = 33;
int breadth = 45;
int perimeter = 2 * (length + breadth);
System.out.println(perimeter);
```

Errors like these, where what the program is doing is different from what it's supposed to do is called a logical error. A logical error could be something as simple as multiplying two numbers in a program instead of adding them. Even though the program runs and gives us a final output, the output is going to be wrong. 








