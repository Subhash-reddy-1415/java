✅ README.md
# Sum of Squares Program

## 📌 Description
This Java program calculates the sum of the squares of the first 20 natural numbers.  
In other words, it computes:



1² + 2² + 3² + ... + 20²


and displays the result.

---

## 🛠️ How It Works
1. A `for` loop runs from `1` to `20`.
2. In each iteration, the square of the current number `i` is calculated using `i * i`.
3. The square is then added to a running total (`sum`).
4. After the loop finishes, the total sum is printed to the console.

---

## ▶️ Example Output


The sum of squares of the first 20 natural numbers is: 2870


---

## 🚀 How to Run

1. Save the code into a file named `K.java`.
2. Open a terminal/command prompt and navigate to the directory containing `K.java`.
3. Compile the program:
   ```sh
   javac K.java


Run the program:

java K

📚 Formula (for verification)

The sum of squares of the first n natural numbers can also be calculated using the formula:

Sum = n(n + 1)(2n + 1) / 6


For n = 20:

Sum = 20 × 21 × 41 / 6 = 2870


This matches the program’s output ✅
```
// Program to calculate the sum of squares of the first 20 natural numbers

public class K {
    public static void main(String[] args) {
        int sqr;  // variable to store square of each number
        int sum = 0; // variable to accumulate the sum of squares

        // Loop from 1 to 20
        for (int i = 1; i <= 20; i++) {
            sqr = i * i;      // calculate square of i
            sum = sum + sqr;  // add square to the running sum
        }

        // Print the result
        System.out.println("The sum of squares of the first 20 natural numbers is: " + sum);
    }
}
```
