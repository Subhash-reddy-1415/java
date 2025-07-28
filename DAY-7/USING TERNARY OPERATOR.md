📄 README - Ternary Operator Program in Java
🔰 Program Name:
Ternary.java

📚 Description:
This Java program demonstrates how to use the ternary (conditional) operator to compare two integers entered by the user. It prints the greater value among the two.

🛠️ Technologies Used:
Language: Java

Input Method: Scanner class (from java.util package)

Operator Used: Ternary Operator (? :)

📥 Input:
The program accepts two integers from the user:

java
Copy
Edit
ENTER THE A VALUE = 15  
ENTER THE B VALUE = 25
📤 Output:
Displays the greater of the two entered numbers:

java
Copy
Edit
THE VALUE OF C = 25
🔍 Logic Used:
java
Copy
Edit
int c = (a > b) ? a : b;
This line means:

If a is greater than b, then assign a to c.

Else, assign b to c.

💡 Features:
Simple and beginner-friendly.

Demonstrates conditional logic using the ternary operator.

Uses clean console input/output.

✅ Example Test Case:
Input A	Input B	Output (C = max(a, b))
10	20	20
50	25	50
30	30	30
```
import java.util.Scanner;  // Import Scanner class for taking user input

public class Ternary {     // Declare the class named Ternary
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);  // Create Scanner object to read input

        System.out.print("ENTER THE A VALUE = ");  // Prompt user to enter value of a
        int a = sc.nextInt();                      // Read integer value and store in variable 'a'

        System.out.print("ENTER THE B VALUE = ");  // Prompt user to enter value of b
        int b = sc.nextInt();                      // Read integer value and store in variable 'b'

        // Use ternary operator to find the greater of a and b
        // If a > b is true, assign 'a' to 'c'; otherwise assign 'b' to 'c'
        int c = (a > b) ? a : b;

        // Display the result stored in variable 'c'
        System.out.println("THE VALUE OF C = " + c);
    }
}```
✅ Explanation of Logic:
int c = (a > b) ? a : b;
This is the ternary operator, a shorthand for an if-else statement:

If a > b is true, then c = a

Else, c = b

🧪 Example Output:
If user enters:

java
Copy
Edit
ENTER THE A VALUE = 15
ENTER THE B VALUE = 20
Output:

java
Copy
Edit
THE VALUE OF C = 20
