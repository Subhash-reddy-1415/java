📘 Java Program – Prime Number Checker
📌 Overview

This program checks whether a given number is prime or not prime.
It uses a for loop and modulus (%) operator to test divisibility.

📝 Code
import java.util.Scanner;

public class A {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Input
        System.out.print("ENTER THE NUMBER = ");
        int number = sc.nextInt();

        // 0 and 1 are not prime
        if (number == 0 || number == 1) {
            System.out.println("NOT A PRIME");
        } else {
            // Check divisibility from 2 to number/2
            for (int i = 2; i <= number / 2; i++) {
                if (number % i == 0) {
                    System.out.println("NOT A PRIME");
                    return; // Exit early if a divisor is found
                }
            }
            System.out.println("PRIME");
        }
    }
}

🖥️ Example Output
Input 1:
ENTER THE NUMBER = 7

Output:
PRIME

Input 2:
ENTER THE NUMBER = 9

Output:
NOT A PRIME

⚙️ How It Works

User enters a number.

Program checks:

If the number is 0 or 1 → Not Prime.

Else, it checks divisibility by all numbers from 2 to number/2.

If divisible, it prints NOT A PRIME and exits.

Otherwise, it prints PRIME.

🚀 Usage

Save code in A.java.

Compile:

javac A.java


Run:

java A

🎯 Learning Outcome

Understand prime numbers.

Practice using loops, conditions, and return statements in Java.

Get comfortable with user input (Scanner class).
