Java Program - Number Condition Checker
📌 Overview

This program takes three integer inputs from the user and checks:

Whether the first number is positive, negative, or zero.

Whether the second number is even or odd.

Whether the third number lies within the range 1 to 100.

The program uses Java’s conditional (ternary) operator ?: to evaluate these conditions in a compact way.

🖥️ Code Explanation
```
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Taking three numbers as input
        int aman = sc.nextInt();  // First number
        int neha = sc.nextInt();  // Second number
        int raj = sc.nextInt();   // Third number

        // Condition 1: Check positive, negative, or zero
        String condition1 = (aman == 0) ? "zero" : (aman > 0) ? "positive" : "negative";

        // Condition 2: Check even or odd
        String condition2 = (neha % 2 == 0) ? "even" : "odd";

        // Condition 3: Check within range 1–100
        String condition3 = (raj >= 1 && raj <= 100) ? "true" : "false";

        // Output results
        System.out.println("Is the first number positive, negative, or zero? " + condition1);
        System.out.println("Is the second number even or odd? " + condition2);
        System.out.println("Is the third number within the range of 1 to 100? " + condition3);
    }
}
```

📝 How It Works

The user enters three numbers one by one.

The program evaluates conditions using the ternary operator:

(condition) ? value_if_true : value_if_false

Results are printed on the screen.

▶️ Sample Input & Output
Input:
10
7
50

Output:
Is the first number positive, negative, or zero? positive
Is the second number even or odd? odd
Is the third number within the range of 1 to 100? true

📚 Concepts Used

Scanner class for input.

Ternary operator (?:) for conditions.

Modulus operator (%) for even/odd checking.

Logical AND (&&) for range checking.
