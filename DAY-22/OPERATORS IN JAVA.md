# Operators in Java

This project demonstrates the use of **arithmetic**, **relational**, **bitwise**, and **ternary operators** in Java.

---

## 🚀 Features
- Reads three integers from the user.
- Performs:
  - **Arithmetic operations** → Addition, Subtraction, Multiplication, Division, Modulus.
  - **Relational operations** → Compares sums and differences with the third integer.
  - **Bitwise operations** → AND, OR, XOR on two integers.
  - **Ternary operations** → Determines sign of the third integer and checks if product > 100.

---

## 🖥️ Example Input/Output

### Input:
Enter first integer (a): 10
Enter second integer (b): 5
Enter third integer (c): 15

shell
Copy
Edit

### Output:
=== Arithmetic Operations ===
Sum: 15
Difference: 5
Product: 50
Quotient: 2
Modulus: 0

=== Relational Operations ===
Is (a + b) greater than c? false
Is (a - b) equal to c? false

=== Bitwise Operations ===
a & b = 0
a | b = 15
a ^ b = 15

=== Ternary Operations ===
Sign of c: positive
Is (a * b) greater than 100? false

yaml
Copy
Edit

---

## 📂 How to Run
1. Save the file as `OperatorsDemo.java`.
2. Compile using:
javac OperatorsDemo.java

markdown
Copy
Edit
3. Run the program:
java OperatorsDemo

yaml
Copy
Edit

---

## 🛠️ Technologies Used
- Java 13+  
- Scanner class for input  
```
import java.util.Scanner;

public class OperatorsDemo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Input: Read three integers a, b, c
        System.out.print("Enter first integer (a): ");
        int a = sc.nextInt();
        System.out.print("Enter second integer (b): ");
        int b = sc.nextInt();
        System.out.print("Enter third integer (c): ");
        int c = sc.nextInt();

        // Arithmetic operations
        int sum = a + b;
        int difference = a - b;
        int product = a * b;
        int quotient = (b != 0) ? (a / b) : 0; // prevent division by zero
        int modulus = (b != 0) ? (a % b) : 0;

        // Relational operations
        boolean isSumGreater = (a + b) > c;
        boolean isDifferenceEqual = (a - b) == c;

        // Bitwise operations
        int bitwiseAnd = a & b;
        int bitwiseOr = a | b;
        int bitwiseXor = a ^ b;

        // Ternary operations
        String signOfC = (c == 0) ? "zero" : (c > 0 ? "positive" : "negative");
        String isProductGreater = (a * b > 100) ? "true" : "false";

        // Output results
        System.out.println("\n=== Arithmetic Operations ===");
        System.out.println("Sum: " + sum);
        System.out.println("Difference: " + difference);
        System.out.println("Product: " + product);
        System.out.println("Quotient: " + quotient);
        System.out.println("Modulus: " + modulus);

        System.out.println("\n=== Relational Operations ===");
        System.out.println("Is (a + b) greater than c? " + isSumGreater);
        System.out.println("Is (a - b) equal to c? " + isDifferenceEqual);

        System.out.println("\n=== Bitwise Operations ===");
        System.out.println("a & b = " + bitwiseAnd);
        System.out.println("a | b = " + bitwiseOr);
        System.out.println("a ^ b = " + bitwiseXor);

        System.out.println("\n=== Ternary Operations ===");
        System.out.println("Sign of c: " + signOfC);
        System.out.println("Is (a * b) greater than 100? " + isProductGreater);

        sc.close();
    }
}
```
