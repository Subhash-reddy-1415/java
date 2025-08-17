README - Largest Number & Even/Odd Sum Program
📌 Program Description

This Java program takes three integers as input:

arjun

bhaskar

chitra

It performs two tasks:

Finds the largest number among the three using the ternary operator.

Finds the sum of the first two numbers (arjun + bhaskar) and checks if the sum is even or odd.

🛠️ Concepts Used

Scanner class → for user input.

Ternary operator (?:) → to find the largest number.

Modulo operator (%) → to check if the sum is even or odd.

📜 Code
```
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Taking inputs
        int arjun = sc.nextInt();
        int bhaskar = sc.nextInt();
        int chitra = sc.nextInt();

        // Condition 1: Largest number among three
        int condition1 = (arjun > bhaskar) ? (arjun > chitra ? arjun : chitra) 
                                           : (bhaskar > chitra ? bhaskar : chitra);

        // Condition 2: Sum of first two numbers (even or odd)
        int sum = arjun + bhaskar;
        String condition2 = (sum % 2 == 0) ? "even" : "odd";

        // Output
        System.out.println("The largest number is: " + condition1);
        System.out.println("The sum of the first two numbers (" + sum + ") is " + condition2);
    }
}
```

⌨️ Sample Input
10
25
15

🖥️ Sample Output
The largest number is: 25
The sum of the first two numbers (35) is odd

✅ Explanation

Inputs: arjun = 10, bhaskar = 25, chitra = 15

Largest number among 10, 25, 15 = 25

Sum of first two numbers = 10 + 25 = 35 → Odd

📚 Learning Outcome

How to use the ternary operator for decision-making.

How to check even/odd numbers.

How to take multiple inputs in Java using Scanner.
