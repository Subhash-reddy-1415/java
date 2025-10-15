# Armstrong Number Checker in Java

This Java program checks whether a given number is an **Armstrong number** or not.

---

## 📖 What is an Armstrong Number?

An **Armstrong number** (or **Narcissistic number**) is a number that is equal to the sum of its own digits, each raised to the power of the number of digits.

### Examples:
- 153 → (1³ + 5³ + 3³) = 1 + 125 + 27 = **153**
- 370 → (3³ + 7³ + 0³) = 27 + 343 + 0 = **370**
- 9474 → (9⁴ + 4⁴ + 7⁴ + 4⁴) = 9474

---

## 🧩 Program Explanation

1. Store a number to check (e.g., 153).
2. Count how many digits it has using:
   ```java
   int digits = String.valueOf(number).length();


Use a while loop to extract each digit using % 10.

Raise the digit to the power of digits using:

Math.pow(rem, digits);


Add the result to a running total (result).

Compare the final result with the original number:

If equal → Armstrong number.

Otherwise → Not an Armstrong number.

🧮 Example Outputs
Example 1:

Input: 153
Output:

153 is an Armstrong number.

Example 2:

Input: 370
Output:

370 is an Armstrong number.

Example 3:

Input: 123
Output:

123 is not an Armstrong number.

▶️ How to Run

Save the file as Armstrong.java

Compile:

javac Armstrong.java


Run:

java Armstrong

💡 Notes

You can modify the number variable to test other numbers.

Works for any positive integer.

Uses:

String.valueOf() to count digits

Math.pow() to raise digits to powers

Simple while loop and if condition for logic
```
public class Armstrong {

    public static void main(String[] args) {
        // Define the number to check
        int number = 153;

        // Store the original number in a temporary variable for later comparison
        int temp = number;

        // Find the total number of digits in the number
        int digits = String.valueOf(number).length();

        // Variable to store the sum of each digit raised to the power of total digits
        int result = 0;

        // Loop until the temporary number becomes 0
        while (temp != 0) {
            // Extract the last digit
            int rem = temp % 10;

            // Add the cube (or nth power) of the digit to result
            result += Math.pow(rem, digits);

            // Remove the last digit
            temp = temp / 10;
        }

        // Check if the computed result equals the original number
        if (result == number) {
            System.out.println(number + " is an Armstrong number.");
        } else {
            System.out.println(number + " is not an Armstrong number.");
        }
    }
}
```
