README — Perfect Square Checker (Java)
📘 Overview

This program checks whether a given number is a Perfect Square or not.
A number is said to be a Perfect Square if the square root of the number is an integer.

📂 File

PerfectSquareCheck.java

💻 Code
public class PerfectSquareCheck {
    public static void main(String[] args) {
        int number = 49; // you can change this number to test
        if (isPerfectSquare(number)) {
            System.out.println(number + " is a perfect square.");
        } else {
            System.out.println(number + " is NOT a perfect square.");
        }
    }

    public static boolean isPerfectSquare(int n) {
        if (n < 0) {
            return false; // negative numbers are not perfect squares
        }
        int sqrt = (int) Math.sqrt(n);
        return (sqrt * sqrt == n);
    }
}

🧠 Explanation
Step	Description
1	Take an integer number.
2	Compute its square root using Math.sqrt().
3	Convert the result to an integer (int).
4	Multiply the integer square root by itself.
5	If it equals the original number → it’s a Perfect Square. Otherwise, it’s Not Perfect Square.
🧩 Example

Input:

number = 49


Process:
sqrt = 7
sqrt * sqrt = 7 * 7 = 49

✅ Output:

49 is a perfect square.

⚙️ Sample Outputs
Input	Output
16	16 is a perfect square.
25	25 is a perfect square.
20	20 is NOT a perfect square.
81	81 is a perfect square.
-9	-9 is NOT a perfect square.
🧩 Key Concepts Used
Concept	Description
Math.sqrt()	Finds the square root of a number.
Type casting	Converts the square root to integer for comparison.
Conditional statements	Checks if sqrt * sqrt == n.
