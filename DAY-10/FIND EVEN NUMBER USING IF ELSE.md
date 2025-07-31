📄 README.md
markdown
Copy
Edit
# Java Program: Check Even or Odd

## ✅ Description
This Java program checks whether a number entered by the user is **even** or **odd**.

---

## 📥 Input
- Takes one integer input from the user.

## 📤 Output
- Displays whether the entered number is **EVEN** or **ODD**.

---

## 🔢 Logic Used
- If the number is divisible by 2 (`a % 2 == 0`), it is even.
- Otherwise, it is odd.

---

## 🧪 Sample Run
ENTER THE VALUE OF A = 10
10 IS AN EVEN NUMBER

ENTER THE VALUE OF A = 7
7 IS AN ODD NUMBER

yaml
Copy
Edit

---

## 🧠 Concepts Covered
- User Input using `Scanner`
- Conditional Statements (`if-else`)
- Modulus Operator `%` for checking divisibility

---

## ⚙️ How to Compile and Run
```bash
javac Main.java
java Main


```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Taking input from the user
        System.out.print("ENTER THE VALUE OF A = ");
        int a = sc.nextInt();

        // Check whether the number is even or odd
        if (a % 2 == 0) {
            System.out.println(a + " IS AN EVEN NUMBER");
        } else {
            System.out.println(a + " IS AN ODD NUMBER");
        }

        sc.close(); // Close the scanner
    }
}
```
