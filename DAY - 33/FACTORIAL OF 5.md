Factorial Program in Java

This program calculates the factorial of a number using a for loop.

📌 What is Factorial?

The factorial of a number n is defined as:

𝑛
!
=
𝑛
×
(
𝑛
−
1
)
×
(
𝑛
−
2
)
×
.
.
.
×
1
n!=n×(n−1)×(n−2)×...×1

Example:

5! = 5 × 4 × 3 × 2 × 1 = 120

💻 Code
class Main {
    public static void main(String[] args) {
        int factorial = 1;   // to store result
        int number = 5;      // number whose factorial we want

        // Loop to calculate factorial
        for (int i = 1; i <= number; i++) {
            factorial = factorial * i;
        }

        // Print result
        System.out.println(factorial);
    }
}

📌 Output
120

🚀 How It Works

Initialize factorial = 1.

Loop from 1 to number.

Multiply factorial by each value of i.

Print the final result.

📝 Notes

Currently, the program calculates 5!.

You can change int number = 5; to any value.

For larger numbers, consider using long or BigInteger because factorial grows very fast.
