📘 README.md
# Digits Delight — Sum of Digits of an Integer in Java

This Java program calculates the **sum of digits** of a given integer entered by the user.

---

## 📖 Problem Description

Write a Java program that takes an integer input and finds the sum of its digits.

For example:
- Input: `123`
- Output: `6` (because 1 + 2 + 3 = 6)

---

## 🧩 Logic Explanation

1. Use a `Scanner` to take user input.
2. Initialize `sum = 0`.
3. Use a `while` loop that runs as long as `number != 0`.
   - Get the last digit using `number % 10`.
   - Add it to `sum`.
   - Remove the last digit using `number / 10`.
4. Print the sum.

---

## 🧮 Example Runs

### Input:


123

### Output:


Sum of digits: 6


### Input:


456

### Output:


Sum of digits: 15


---

## ⚙️ How to Run the Program

1. Save the code as `Main.java`.
2. Open a terminal and compile the program:
   ```bash
   javac Main.java


Run the compiled file:

java Main


Enter a number when prompted.

💡 Sample Run
Enter a number: 789
Sum of digits: 24

🧠 Concepts Used

Loops (while)

Arithmetic operations (% and /)

User input via Scanner

```
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        // Create a Scanner object to take input from the user
        Scanner scanner = new Scanner(System.in);

        // Prompt the user to enter an integer
        System.out.print("Enter a number: ");
        int number = scanner.nextInt();

        // Initialize a variable to store the sum of digits
        int sum = 0;

        // Loop continues until the number becomes 0
        while (number != 0) {
            // Extract the last digit using modulus operator (%)
            int remainder = number % 10;

            // Add the extracted digit to the sum
            sum = sum + remainder;

            // Remove the last digit by integer division
            number = number / 10;
        }

        // Print the final sum of digits
        System.out.println("Sum of digits: " + sum);

        // Close the Scanner to avoid resource leaks
        scanner.close();
    }
}

```
