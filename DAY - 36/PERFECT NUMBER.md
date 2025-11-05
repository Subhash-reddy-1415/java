README — Perfect Number Checker (Java)
📘 Overview

This Java program checks whether a given number is a Perfect Number or not.
A Perfect Number is a number that is equal to the sum of its proper divisors (excluding itself).

📂 File

Perfect.java

💻 Code
public class Perfect {

    public static void main(String[] args) {
        int number = 8128;
        if (numChecker(number, 0, number)) {
            System.out.println("number is a perfect number");
        } else {
            System.out.println("number is not a perfect number");
        }
    }

    public static boolean numChecker(int number, int sum, int temp) {
        for (int i = 1; i < number; i++) {
            if (number % i == 0) {     // Check divisor
                sum = sum + i;         // Add divisor to sum
            }
        }
        return sum == temp;            // Compare sum with original number
    }
}

🧠 Explanation
Step	Description
1	Take a number as input (e.g., 8128).
2	Find all divisors of the number (excluding the number itself).
3	Add up all the divisors.
4	If the sum equals the original number → It’s a Perfect Number.
5	Otherwise → It’s Not Perfect.
🧩 Example

Input:

number = 8128


Divisors:
1, 2, 4, 8, 16, 32, 64, 127, 254, 508, 1016, 2032, 4064

Sum:
1 + 2 + 4 + 8 + 16 + 32 + 64 + 127 + 254 + 508 + 1016 + 2032 + 4064 = 8128

✅ Output:

number is a perfect number

⚙️ Sample Outputs
Input	Divisors	Sum	Output
6	1, 2, 3	6	Perfect
28	1, 2, 4, 7, 14	28	Perfect
12	1, 2, 3, 4, 6	16	Not Perfect
496	(many divisors)	496	Perfect
8128	(many divisors)	8128	Perfect
🧩 Key Concepts Used
Concept	Description
For Loop	Iterates through possible divisors
Modulo (%)	Checks if a number divides evenly
Method with Parameters	Reusable logic for checking perfect numbers
Boolean Return	Returns true if number is perfect
