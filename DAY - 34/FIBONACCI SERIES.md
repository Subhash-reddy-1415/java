📄 README.md
# Fibonacci Series Program in Java

This Java program prints the Fibonacci series up to a user-defined maximum number using a `while` loop.

---

## 📘 Fibonacci Series Explanation

The **Fibonacci series** is a sequence of numbers where each number is the sum of the two preceding ones.  
It typically starts with **0** and **1**.

Example:


0, 1, 1, 2, 3, 5, 8, 13, 21, ...


---

## 🎯 Task

Write a Java program that:
1. Takes a user input (maximum number) using `Scanner`.
2. Prints all Fibonacci numbers **up to** that number.

---

## 🧩 How It Works

1. Take user input `maxNumber` (upper limit).
2. Initialize first two Fibonacci numbers:  
   `a = 0`, `b = 1`.
3. Print numbers while the current value `a <= maxNumber`.
4. Update Fibonacci sequence as:


next = a + b
a = b
b = next

5. Stop when `a` exceeds `maxNumber`.

---

## 🧮 Example Outputs

### Input:


10

### Output:


Fibonacci series up to 10: 0 1 1 2 3 5 8


### Input:


21

### Output:


Fibonacci series up to 21: 0 1 1 2 3 5 8 13 21


---

## ▶️ How to Run

1. Save the code as `Main.java`.
2. Compile the program:
   ```bash
   javac Main.java


Run the compiled file:

java Main


Enter a number when prompted to see the Fibonacci series.
```
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        // Create a Scanner object to take input from the user
        Scanner scanner = new Scanner(System.in);

        // Prompt user to enter the maximum number up to which Fibonacci series should be printed
        System.out.print("Enter the maximum number: ");
        int maxNumber = scanner.nextInt();

        // Initialize the first two Fibonacci numbers
        int a = 0;
        int b = 1;

        // Print header for output
        System.out.print("Fibonacci series up to " + maxNumber + ": ");

        // Loop until the current Fibonacci number exceeds the maximum number
        while (a <= maxNumber) {
            // Print the current Fibonacci number
            System.out.print(a + " ");

            // Calculate the next number in the series
            int next = a + b;

            // Update 'a' and 'b' for next iteration
            a = b;
            b = next;
        }

        // Close the scanner to avoid resource leaks
        scanner.close();
    }
}
```
