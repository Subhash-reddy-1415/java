Sum of Natural Numbers

This project is a simple Java program that calculates and displays the sum of the first ten natural numbers using a for loop.

📌 Problem Statement

Write a Java program to:

Calculate the sum of the first ten natural numbers (1 to 10).

Display the result on the console.

🛠️ Implementation Details

Declare an integer variable sum and initialize it to 0.

Use a for loop:

Start with i = 1.

Run the loop while i <= 10.

Increment i by 1 in each iteration.

Inside the loop, add i to sum using the += operator.

Print the final result after the loop ends.

📜 Source Code
```
public class Main {
    public static void main(String[] args) {
        int sum = 0;
        for (int i = 1; i <= 10; i++) {
            sum += i;
        }
        System.out.println("Sum of the first ten natural numbers: " + sum);
    }
}
```

▶️ Output
Sum of the first ten natural numbers: 55

📚 Explanation

The program loops through numbers 1 to 10.

Each number is added to the variable sum.

After the loop, the final value of sum is 55.

Formula check:
Sum of first n natural numbers = n(n+1)/2
For n = 10 → 10 * 11 / 2 = 55 ✅
