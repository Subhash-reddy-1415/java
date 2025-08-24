# Multiplication Table Printer (Java)

## 📌 Description
This program prints the multiplication table of a given number using a **do-while loop**.  
Here, the number is fixed as `5`, and the table is printed from `5 × 1` to `5 × 10`.

---

## ⚙️ How It Works
1. Declare an integer variable `number` and assign it a value (e.g., 5).
2. Declare another integer variable `multiplier` and initialize it to `1`.
3. Use a **do-while loop**:
   - Print the multiplication in this format:  
     ```
     number * multiplier = result
     ```
   - Increment `multiplier` by 1.
   - Repeat until `multiplier <= 10`.
4. End the loop when multiplier becomes `11`.

---

## 🧮 Example
For `number = 5`:

Output:
5 * 1 = 5
5 * 2 = 10
5 * 3 = 15
5 * 4 = 20
5 * 5 = 25
5 * 6 = 30
5 * 7 = 35
5 * 8 = 40
5 * 9 = 45
5 * 10 = 50

yaml
Copy
Edit

---

## 🚀 How to Run
1. Save the code in a file named `Main.java`.
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

## ✅ Expected Output
5 * 1 = 5
5 * 2 = 10
5 * 3 = 15
5 * 4 = 20
5 * 5 = 25
5 * 6 = 30
5 * 7 = 35
5 * 8 = 40
5 * 9 = 45
5 * 10 = 50

Copy
Edit
```
public class Main {
    public static void main(String[] args) {
        int number = 5;       // the number whose table we want
        int multiplier = 1;   // start from 1

        // do-while loop to print table from 1 to 10
        do {
            System.out.println(number + " * " + multiplier + " = " + (number * multiplier));
            multiplier++;  // increment multiplier
        } while (multiplier <= 10);
    }
}
```
