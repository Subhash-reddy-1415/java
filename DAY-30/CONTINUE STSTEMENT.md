# Continue Statement - Skipping Multiples of 3 (Java)

## 📌 Description
This program calculates the sum of numbers from **1 to 10**, but **skips numbers that are multiples of 3** using the `continue` statement.

---

## ⚙️ How It Works
1. Initialize `sum = 0`.
2. Use a `for` loop from `1` to `10`.
3. Inside the loop:
   - If the number is divisible by 3 (`i % 3 == 0`):
     - Print `"Number i is skipped."`
     - Use `continue` to skip adding it.
   - Otherwise:
     - Add the number to `sum`.
     - Print `"Number i is added. Current sum: X"`.
4. After the loop, print the **final sum**.

---

## 🧮 Example Output
Number 1 is added. Current sum: 1
Number 2 is added. Current sum: 3
Number 3 is skipped.
Number 4 is added. Current sum: 7
Number 5 is added. Current sum: 12
Number 6 is skipped.
Number 7 is added. Current sum: 19
Number 8 is added. Current sum: 27
Number 9 is skipped.
Number 10 is added. Current sum: 37
Final sum: 37

yaml
Copy
Edit

---

## 🚀 How to Run
1. Save the program in a file named `Main.java`.
2. Compile:
javac Main.java

markdown
Copy
Edit
3. Run:
java Main

yaml
Copy
Edit

---

## ✅ Key Concept
- The `continue` statement is used to **skip the current iteration** of a loop and jump to the next iteration.
```
public class Main {
    public static void main(String[] args) {
        int sum = 0; // variable to store sum

        // Loop from 1 to 10
        for (int i = 1; i <= 10; i++) {
            
            // Skip multiples of 3
            if (i % 3 == 0) {
                System.out.println("Number " + i + " is skipped.");
                continue; // skip this iteration
            }

            // Add number to sum
            sum += i;
            System.out.println("Number " + i + " is added. Current sum: " + sum);
        }

        // Print final sum
        System.out.println("Final sum: " + sum);
    }
}
```
