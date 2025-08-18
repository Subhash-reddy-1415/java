README
📌 Program Name

Check Multiple of 5 in Java

📖 Description

This program prompts the user to enter an integer and checks if the number is a multiple of 5.

If the number is a multiple of 5, it displays:

The number is a multiple of 5.


Regardless of the result, the program always displays:

Program Ended

🛠️ Concepts Used

Scanner class for input

if condition to check divisibility

Modulo operator (%) to determine multiples

📝 Code
```
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        // Create Scanner object to take input
        Scanner sc = new Scanner(System.in);

        // Read input number
        int number = sc.nextInt();

        // Check if number is multiple of 5
        if (number % 5 == 0) {
            System.out.println("The number is a multiple of 5.");
        }

        // This will always print
        System.out.println("Program Ended");
    }
}
```

▶️ Example Execution
Input
25

Output
The number is a multiple of 5.
Program Ended

Input
7

Output
Program Ended

✅ Key Learning

Use of if conditional statement.

Importance of % operator for divisibility checks.

Always printing a final statement regardless of condition.
