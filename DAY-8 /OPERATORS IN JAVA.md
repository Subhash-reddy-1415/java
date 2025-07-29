📄 README.md

Copy
Edit
# OperatorsDemo - Java Program

## 📌 Overview
`OperatorsDemo` is a simple Java program that demonstrates the usage of **all types of operators** in Java through user inputs. It covers:

- Arithmetic Operators
- Relational Operators
- Logical Operators
- Bitwise Operators
- Assignment Operators
- Unary Operators
- Ternary Operator

This program helps beginners understand how each operator behaves through examples and clear output.

---

## 🧾 How It Works

1. The program prompts the user to enter two integers `a` and `b`.
2. It performs operations on these values using different operator types.
3. Results are printed in a clean, categorized format.

---

## 🧮 Operator Categories Demonstrated

### ✅ 1. Arithmetic Operators
- `+`, `-`, `*`, `/`, `%`  
  → Basic mathematical operations.

### ✅ 2. Relational Operators
- `==`, `!=`, `>`, `<`, `>=`, `<=`  
  → Used to compare values.

### ✅ 3. Logical Operators
- `&&`, `||`, `!`  
  → Used in boolean logic expressions.

### ✅ 4. Bitwise Operators
- `&`, `|`, `^`, `~`, `<<`, `>>`  
  → Works at the bit level.

### ✅ 5. Assignment Operators
- `=`, `+=`, `-=`, `*=`, `/=`, `%=`  
  → Used to assign values to variables.

### ✅ 6. Unary Operators
- `++`, `--` (both prefix and postfix)  
  → Increments/decrements variable values.

### ✅ 7. Ternary Operator
- `(condition) ? true-value : false-value`  
  → Shorthand `if-else` logic to choose between two values.

---

## 🖥️ Example Output

ENTER THE A VALUE = 10
ENTER THE B VALUE = 5

--- Arithmetic Operators ---
Addition (a + b): 15
Subtraction (a - b): 5
...

--- Ternary Operator ---
Maximum of a and b: 10

yaml
Copy
Edit

---

## 🧑‍💻 How to Run

1. Save the file as `OperatorsDemo.java`
2. Compile:
   ```bash
   javac OperatorsDemo.java
Run:

bash
Copy
Edit
java OperatorsDemo 
```

import java.util.Scanner;

public class OperatorsDemo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Input section
        System.out.print("ENTER THE A VALUE = ");
        int a = sc.nextInt();
        System.out.print("ENTER THE B VALUE = ");
        int b = sc.nextInt();

        System.out.println("\n--- Arithmetic Operators ---");
        System.out.println("Addition (a + b): " + (a + b));
        System.out.println("Subtraction (a - b): " + (a - b));
        System.out.println("Multiplication (a * b): " + (a * b));
        System.out.println("Division (a / b): " + (a / b));
        System.out.println("Modulus (a % b): " + (a % b));

        System.out.println("\n--- Relational Operators ---");
        System.out.println("a == b: " + (a == b));
        System.out.println("a != b: " + (a != b));
        System.out.println("a > b: " + (a > b));
        System.out.println("a < b: " + (a < b));
        System.out.println("a >= b: " + (a >= b));
        System.out.println("a <= b: " + (a <= b));

        System.out.println("\n--- Logical Operators ---");
        System.out.println("(a > 0 && b > 0): " + (a > 0 && b > 0));
        System.out.println("(a > 0 || b < 0): " + (a > 0 || b < 0));
        System.out.println("!(a > b): " + !(a > b));

        System.out.println("\n--- Bitwise Operators ---");
        System.out.println("a & b: " + (a & b));
        System.out.println("a | b: " + (a | b));
        System.out.println("a ^ b: " + (a ^ b));
        System.out.println("~a: " + (~a));
        System.out.println("a << 1: " + (a << 1));
        System.out.println("a >> 1: " + (a >> 1));

        System.out.println("\n--- Assignment Operators ---");
        int x = a;
        System.out.println("x = " + x);
        x += b;
        System.out.println("x += b: " + x);
        x -= b;
        System.out.println("x -= b: " + x);
        x *= b;
        System.out.println("x *= b: " + x);
        x /= b;
        System.out.println("x /= b: " + x);
        x %= b;
        System.out.println("x %= b: " + x);

        System.out.println("\n--- Unary Operators ---");
        int unary = a;
        System.out.println("Initial value: " + unary);
        System.out.println("Post-increment (unary++): " + (unary++));
        System.out.println("After post-increment: " + unary);
        System.out.println("Pre-increment (++unary): " + (++unary));
        System.out.println("Post-decrement (unary--): " + (unary--));
        System.out.println("After post-decrement: " + unary);
        System.out.println("Pre-decrement (--unary): " + (--unary));

        System.out.println("\n--- Ternary Operator ---");
        int max = (a > b) ? a : b;
        System.out.println("Maximum of a and b: " + max);

        sc.close();
    }
}
```
