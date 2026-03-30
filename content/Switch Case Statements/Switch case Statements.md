
---
title : Switch Case statements
noteOrder : 31

---

### Introduction

Previously, we used [[if, if - else, if  - else if|conditional statements]] to control the flow of the program. We used them to execute certain blocks of code if a condition was true and skip them entirely if the condition was false. Switch case statements are used to do something very similar.

Switch case statements work by checking if two values are equal, and executing a block of code if they're equal. They aren't "conditional" entirely since there's only one condition, but they're still incredibly useful.

You'll understand this better when you watch the video, but switch case statements are usually used for programs called "menu- driven programs".  These are programs where we want to display a number of options to the user and execute something depending on what option the user enters. Instead of using a bunch of if or else-if statements, we can use switch case statements.

### Video lesson

![Switch Case Statements](https://youtu.be/S1OaKBeYsmI?si=DP44Q2L0uP2mFjyo)

### Syntax

To understand the syntax, we'll look at a simple program.

Let's say that we want to display a menu of food items to the user and print a particular food items depending on whatever option the user enters. This is the menu we'll use for the program

```
1. Butter naan
2. Biryani
3. Pulao
```

If the user enters 1, we'll print "Butter naan". If the user enters 3, we'll print "Pulao"

```Java
import java.util.*;
public class SwitchCase{
	public static void main(String[]args){	
		//displaying the menu
		System.out.println("1. Butter naan");
		System.out.println("2. Biryani");
		System.out.println("3. Pulao");
		int option = sa.nextInt();
		
		switch(option){
			case 1 :
				System.out.println("Butter naan");
				break;
			case 2 :
				System.out.println("Biryani");
				break;
			case 3 :
				System.out.println("Pulao");
				break;
			default:
				System.out.println("wrong option entered");
				
			}		
	}
}
```

