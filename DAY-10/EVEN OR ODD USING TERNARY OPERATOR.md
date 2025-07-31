 README.md
markdown
Copy
Edit
# Java Program: Check Even or Odd using Ternary Operator

## ✅ Description
This Java program determines whether a number entered by the user is **even** or **odd** using the **ternary operator**.

---

## 📥 Input
- One integer value (`a`) from the user.

## 📤 Output
- Prints:
  - `"A IS EVEN"` if the number is divisible by 2.
  - `"A IS ODD"` otherwise.

---

## 🔢 Logic Used
The ternary operator:
```java
(condition) ? "if true" : "if false"
In this program:

java
Copy
Edit
(a % 2 == 0) ? "A IS EVEN" : "A IS ODD"
🧪 Sample Run
java
Copy
Edit
ENTER THE VALUE OF A = 4
A IS EVEN

ENTER THE VALUE OF A = 7
A IS ODD
🧠 Concepts Covered
Scanner class for input

Ternary operator (? :)

Modulus operator % to check even/odd

⚙️ How to Compile and Run
bash
Copy
Edit
javac Main.java
java Main


```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Asking the user to enter a number
        System.out.print("ENTER THE VALUE OF A = ");
        int a = sc.nextInt();

        // Using ternary operator to check if the number is even or odd
        System.out.println((a % 2 == 0) ? "A IS EVEN" : "A IS ODD");

        sc.close(); // Closing the scanner
    }
}
```
