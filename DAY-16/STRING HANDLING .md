README
Program Name
Java Program: String Handling Examples

Overview
This Java program demonstrates basic string operations such as:

Accepting user input

Converting text to lowercase

Checking the length of the string

Comparing two strings

Checking if two strings are equal

It is useful for learning the String class in Java.

Features
User Input
Uses Scanner to read strings from the user.

Lowercase Conversion
Converts the entered string into lowercase using:

java
Copy
Edit
str.toLowerCase();
String Length
Finds the length of the string using:

java
Copy
Edit
str.length();
String Comparison
Compares two strings lexicographically using:

java
Copy
Edit
str1.compareTo(str2);
Equality Check
Checks if two strings are exactly the same using:

java
Copy
Edit
str1.equals(str2);
How It Works
The program asks the user to enter a string.

Displays the string in lowercase.

Shows the number of characters in the string.

Accepts two more strings for comparison.

Displays:

Result of lexicographical comparison

Whether the two strings are equal or not.

Example Output
yaml
Copy
Edit
Enter a string: HelloWorld
Lowercase: helloworld
Length: 10

Enter first string: apple
Enter second string: banana
Lexicographical Comparison Result: -1
Strings are equal? false
Requirements
Java JDK 8 or higher

Any Java IDE (Eclipse, IntelliJ IDEA, NetBeans) or Command Prompt

How to Run
Save the file as StringExample.java

Open a terminal in the folder where the file is saved.

Compile:

bash
Copy
Edit
javac StringExample.java
Run:

bash
Copy
Edit
java StringExample
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int day = scanner.nextInt();

        if (day >= 1 && day <= 5) {
            System.out.println("Weekday");
        } else if (day >= 6 && day <= 7) {
            System.out.println("Weekend");
        } else {
            System.out.println("Invalid day number");
        }

        scanner.close();
    }
}
```
