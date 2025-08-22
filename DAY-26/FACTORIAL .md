# Factorial Calculator (Java)

## 📌 Description
This is a simple Java program that calculates the factorial of a number using a **while loop**.  
The program starts with a fixed number (in this case, 5) and computes its factorial.

---

## ⚙️ How It Works
1. Declare an integer variable `number` and assign it a value (e.g., 5).
2. Declare another integer variable `factorial` and initialize it to `1`.
3. Use a **while loop** that runs while `number > 0`:
   - Multiply `factorial` by `number`.
   - Decrement `number` using `--`.
4. Print the result.

---

## 🧮 Example
For `number = 5`:
factorial = 5 × 4 × 3 × 2 × 1 = 120

makefile
Copy
Edit

Output:
Factorial: 120

yaml
Copy
Edit

---

## 🚀 How to Run
1. Save the program in a file named `Main.java`.
2. Compile the program:
javac Main.java

markdown
Copy
Edit
3. Run the program:
java Main

yaml
Copy
Edit

---

## ✅ Expected Output
Factorial: 120

Copy
Edit
```
  public class Main {
    public static void main(String[] args) {
        // Declare number and factorial
        int number = 5; 
        int factorial = 1;

        // While loop to calculate factorial
        while (number > 0) {
            factorial *= number; // multiply factorial by number
            number--;            // decrement number
        }

        // Print the result
        System.out.println("Factorial: " + factorial);
    }
}
```
