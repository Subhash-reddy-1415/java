Pizza or Burger (Java Program)
📌 Overview

This program demonstrates the use of if-else conditional statements in Java.
It allows the program to choose between two food items (Pizza or Burger) and two drinks (Coke or Pepsi) based on the values of given variables.

📜 Program Description

Create a variable a and assign it the value 1.

If a == 1, print "Here is your Pizza".

Otherwise, print "Here is your Burger".

Create another variable b and assign it the value 2.

If b == 1, print "Here is your Coke".

Otherwise, print "Here is your Pepsi".

🖥️ Code
```
public class Main {
    public static void main(String[] args) {
        int a = 1;
        if (a == 1) {
            System.out.println("Here is your Pizza");
        } else {
            System.out.println("Here is your Burger");
        }

        int b = 2;
        if (b == 1) {
            System.out.println("Here is your Coke");
        } else {
            System.out.println("Here is your Pepsi");
        }
    }
}
```
✅ Output

For a = 1 and b = 2, the output will be:

Here is your Pizza
Here is your Pepsi

📚 Concepts Used

Variables (int a, b)

Conditional Statements (if-else)

Output Statement (System.out.println())
