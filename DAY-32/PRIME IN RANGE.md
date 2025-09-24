Prime Numbers in a Range (Java)
📌 Overview

This Java program prints all the prime numbers within a given range.
The user enters the start and end of the range, and the program checks each number to determine if it is prime.

📝 Features

Takes user input for the start and end of the range.

Skips 0 and 1 since they are not prime.

Uses a simple loop-based approach (no extra functions).

Prints all prime numbers between the given range.

💻 Code
import java.util.Scanner;

public class PrimeInRange {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        System.out.print("Enter start of range: ");
        int start = sc.nextInt();
        System.out.print("Enter end of range: ");
        int end = sc.nextInt();

        System.out.println("Prime numbers between " + start + " and " + end + " are:");

        for (int number = start; number <= end; number++) {
            if (number == 0 || number == 1) {
                continue; // skip 0 and 1
            }

            boolean isPrime = true;
            for (int i = 2; i <= number / 2; i++) {
                if (number % i == 0) {
                    isPrime = false;
                    break;
                }
            }

            if (isPrime) {
                System.out.print(number + " ");
            }
        }
    }
}

▶️ Example Run

Input:

Enter start of range: 10
Enter end of range: 30


Output:

Prime numbers between 10 and 30 are:
11 13 17 19 23 29

🚀 How to Run

Save the program as PrimeInRange.java

Open a terminal/command prompt and compile:

javac PrimeInRange.java


Run the program:

java PrimeInRange
