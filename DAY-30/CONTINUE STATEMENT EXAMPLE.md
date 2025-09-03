Java Program to Print Numbers from 1 to N (Skipping Multiples of Both 3 and 5)
📌 Problem Statement

Write a Java program to print all numbers from 1 to N, but skip the numbers that are multiples of both 3 and 5 (i.e., skip multiples of 15).
Use the continue statement inside a loop to achieve this.

📂 Program Explanation

The program takes an integer N as input.

It iterates from 1 to N.

If a number is divisible by both 3 and 5, it is skipped using the continue statement.

All other numbers are printed.

📝 Code
import java.util.Scanner;
public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int N = scanner.nextInt();
        System.out.print("Numbers: ");
        
        for (int i = 1; i <= N; i++) {
            if (i % 3 == 0 && i % 5 == 0) {
                continue; // Skip multiples of both 3 and 5
            }
            System.out.print(i + " ");
        }
    }
}

🎯 Sample Input/Output
Example 1:

Input

15


Output

Numbers: 1 2 3 4 5 6 7 8 9 10 11 12 13 14

Example 2:

Input

20


Output

Numbers: 1 2 3 4 5 6 7 8 9 10 11 12 13 14 16 17 18 19 20

🚀 How to Run

Save the code in a file named Main.java.

Open terminal/command prompt and compile the program:

javac Main.java


Run the program:

java Main


Enter a value for N and observe the output.
