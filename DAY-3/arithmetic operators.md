# Java Arithmetic Operators Example

This simple Java program demonstrates the use of **arithmetic operators** such as addition, subtraction, multiplication, division, and modulus with two integers.

---

## 📌 Description

The program defines two integer variables `a` and `b`, performs five basic arithmetic operations, and prints the results:

### 🔢 Operators Used:

| Operator | Symbol | Description         | Example      |
|----------|--------|---------------------|--------------|
| Addition | `+`    | Adds two numbers    | `a + b`      |
| Subtract | `-`    | Subtracts numbers   | `a - b`      |
| Multiply | `*`    | Multiplies numbers  | `a * b`      |
| Divide   | `/`    | Divides numbers     | `b / a`      |
| Modulus  | `%`    | Remainder of divide | `b % a`      |

---

## 💻 Code

```java
public class Main {
    public static void main(String[] args) {
        int a = 10;
        int b = 20;

        // Arithmetic operations
        int sum = a + b;
        int difference = a - b;
        int product = a * b;
        int quotient = b / a;
        int remainder = b % a;

        // Output results
        System.out.println("Sum: " + sum);
        System.out.println("Difference: " + difference);
        System.out.println("Product: " + product);
        System.out.println("Quotient: " + quotient);
        System.out.println("Remainder: " + remainder);
    }
}
```
public class Main {
    public static void main(String[] args) {
        int a = 10;
        int b = 20;

        // Arithmetic operations
        int sum = a + b;           // Addition
        int difference = a - b;    // Subtraction
        int product = a * b;       // Multiplication
        int quotient = b / a;      // Division (note: integer division)
        int remainder = b % a;     // Modulus (remainder)

        // Display results
        System.out.println("Sum: " + sum);
        System.out.println("Difference: " + difference);
        System.out.println("Product: " + product);
        System.out.println("Quotient: " + quotient);
        System.out.println("Remainder: " + remainder);
    }
}
```
