README
Program Name
Senior Citizen Check Based on Age

Overview
This Java program checks whether a person qualifies as a senior citizen based on their age.
If the age is 60 or above, it prints "Senior Citizen".
If the age is below 60, it prints "Not Senior Citizen".

Features
User Input:

Reads an integer value for age using the Scanner class.

Method-based Approach:

Implements the logic inside a separate method checkSeniorCitizen(int age).

Simple Condition:

Uses an if-else statement to determine and print the category.

Code
java
Copy
Edit
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int age = scanner.nextInt();  // Read age from user
        checkSeniorCitizen(age);      // Call method to check status
    }

    public static void checkSeniorCitizen(int age) {
        if (age >= 60) {
            System.out.println("Senior Citizen");
        } else {
            System.out.println("Not Senior Citizen");
        }
    }
}
```
Sample Input / Output
Example 1:

makefile
Copy
Edit
Input:
65
Output:
Senior Citizen
Example 2:

makefile
Copy
Edit
Input:
50
Output:
Not Senior Citizen
Requirements
Java JDK 8 or higher

Any Java IDE or command-line environment

How to Run
Save the code as Main.java

Open a terminal in the file location.

Compile:

bash
Copy
Edit
javac Main.java
Run:

bash
Copy
Edit
java Main
Enter an age when prompted.
