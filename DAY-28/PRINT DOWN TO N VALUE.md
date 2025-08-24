# Countdown Timer Using While Loop (Java)

## 📌 Description
This program reads an integer `N` from the user and prints all the numbers from `N` down to `1` using a **while loop**.

---

## ⚙️ How It Works
1. Import `Scanner` class to read input.
2. Take an integer `N` as input from the user.
3. Use a **while loop**:
   - Condition: run while `N >= 1`.
   - Print the current value of `N`.
   - Decrement `N` by 1 after each iteration.
4. Loop continues until `N` becomes `0`.

---

## 🧮 Example
### Input:
5

shell
Copy
Edit

### Output:
5
4
3
2
1

yaml
Copy
Edit

---

## 🚀 How to Run
1. Save the code as `Main.java`.
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

## ✅ Sample Outputs
Input: `3`  
Output:
3
2
1

makefile
Copy
Edit

Input: `7`  
Output:
7
6
5
4
3
2
1
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Read input number
        int N = scanner.nextInt();

        // Countdown from N to 1
        while (N >= 1) {
            System.out.println(N);
            N--; // decrement by 1
        }
    }
}
```
