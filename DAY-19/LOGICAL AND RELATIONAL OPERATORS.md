README – Java Program for Logical and Relational Operations
1. Overview

This program takes four integer inputs from the user and performs different logical and relational checks on them. It uses Scanner for input and prints boolean results (true or false) based on the given conditions.

2. Features

The program checks:

Condition 1: Is the sum of the first two numbers greater than the product of the third and fourth numbers?

Condition 2: Is the difference between the first and second numbers equal to the sum of the third and fourth numbers?

Condition 3:

Is the first number positive?

Is the second number negative?

Is the product of the third and fourth numbers a multiple of 10?

3. Code Flow

Import java.util.Scanner for reading user input.

Read four integers: a, b, c, and d.

Compute three boolean conditions:

boolean condition1 = (a + b) > (c * d);
boolean condition2 = (a - b) == (c + d);
boolean condition3 = a > 0 && b < 0 && (c * d) % 10 == 0;


Display the results of each condition with descriptive messages.

4. Example

Input:

5
-2
3
4


Step-by-step Check:

Condition 1: (5 + -2) > (3 * 4) → 3 > 12 → false

Condition 2: (5 - -2) == (3 + 4) → 7 == 7 → true

Condition 3: 5 > 0 && -2 < 0 && (3 * 4) % 10 == 0 → true && true && false → false

Output:

Is the sum of the first two numbers greater than the product of the third and fourth numbers? false
Is the difference between the first and second numbers equal to the sum of the third and fourth numbers? true
Is the first number positive, the second number negative, and the product of the third and fourth numbers a multiple of 10? false

5. How to Run

Save the program as Main.java.

Compile:

javac Main.java


Run:

java Main

6. Notes

Works for both positive and negative integers.

Division/modulus checks use integer math.

Multiple conditions are combined using logical AND (&&) and equality/relational operators.
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Input section
        System.out.print("Enter first number (a): ");
        int a = sc.nextInt();

        System.out.print("Enter second number (b): ");
        int b = sc.nextInt();

        System.out.print("Enter third number (c): ");
        int c = sc.nextInt();

        System.out.print("Enter fourth number (d): ");
        int d = sc.nextInt();

        // Condition 1: sum of first two > product of last two
        boolean condition1 = (a + b) > (c * d);

        // Condition 2: difference of first two == sum of last two
        boolean condition2 = (a - b) == (c + d);

        // Condition 3: first positive, second negative, product of last two multiple of 10
        boolean condition3 = (a > 0) && (b < 0) && ((c * d) % 10 == 0);

        // Output results
        System.out.println("\nIs the sum of the first two numbers greater than the product of the third and fourth numbers? " + condition1);
        System.out.println("Is the difference between the first and second numbers equal to the sum of the third and fourth numbers? " + condition2);
        System.out.println("Is the first number positive, the second number negative, and the product of the third and fourth numbers a multiple of 10? " + condition3);

        sc.close();
    }
}
```
