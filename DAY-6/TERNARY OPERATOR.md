📄 README – Java Program: Ternary Operator
📌 Program Name: Ternary.java
📚 Purpose:
This Java program demonstrates the use of the ternary conditional operator ? : to compare two integers and print which one is greater.

🧠 Concept Covered:
Symbol	Operator Name	Description
? :	Ternary Operator	A shorthand for if-else conditional statements

💡 Syntax of Ternary Operator:
java
Copy
Edit
condition ? value_if_true : value_if_false;
💻 Program Flow:
The user is prompted to input two integers: a and b.

The ternary operator compares whether a > b.

If the condition is true, it prints "A IS GREATER".

Otherwise, it prints "B IS GREATER".

🧪 Sample Input/Output:
Case 1:
java
Copy
Edit
ENTER THE A VALUE = 10
ENTER THE B VALUE = 20
B IS GREATER
Case 2:
java
Copy
Edit
ENTER THE A VALUE = 25
ENTER THE B VALUE = 15
A IS GREATER
🛠️ How to Compile and Run:
Save the file as Ternary.java

Open terminal or command prompt

Compile the program:

bash
Copy
Edit
javac Ternary.java
Run the program:

bash
Copy
Edit
java Ternary
✅ Benefits of Using Ternary Operator:
Makes code shorter and cleaner for simple conditions.

Improves readability for compact comparisons.

📌 Note:
You can extend this logic to check equality as well:

java
Copy
Edit
System.out.println((a == b) ? "A IS EQUAL TO B" : (a > b ? "A IS GREATER" : "B IS GREATER"));
```
import java.util.Scanner;  // Import the Scanner class for input
public class Ternary {     // Class declaration
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);  // Create Scanner object for user input

        System.out.print("ENTER THE A VALUE = ");  // Prompt for first number
        int a = sc.nextInt();                      // Read first number from user

        System.out.print("ENTER THE B VALUE = ");  // Prompt for second number
        int b = sc.nextInt();                      // Read second number from user

        // Ternary operator checks if a is greater than b
        // If true, prints "A IS GREATER", else prints "B IS GREATER"
        System.out.println((a > b) ? "A IS GREATER" : "B IS GREATER");
    }
}
```
