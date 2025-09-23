✅ README.md
# Reverse Number Program

## 📌 Description
This Java program reverses the digits of a given number.  
For example:


Input: 1234
Output: 4321


---

## 🛠️ How It Works
1. The program initializes a number (e.g., `1234`).
2. It uses a `while` loop to repeatedly extract the last digit using **modulus (`%`)**.
3. The extracted digit is added to the reversed number (`rev_number`) after shifting its digits.
4. The original number is reduced by removing the last digit (`/ 10`).
5. The process continues until the original number becomes `0`.

---

## ▶️ Example Output


Reverse of a number: 4321


---

## 🚀 How to Run

1. Save the code into a file named `Main.java`.
2. Open a terminal/command prompt and navigate to the file’s directory.
3. Compile the program:
   ```sh
   javac Main.java


Run the program:

java Main

code:
```

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int number = sc.nextInt();   // take user input

        int rev_number = 0;

        while (number != 0) {
            int div = number % 10;
            rev_number = rev_number * 10 + div;
            number = number / 10;
        }

        System.out.println("Reversed number: " + rev_number);
    }
}
```
