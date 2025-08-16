# Java Program – Logical Conditions with User Input

## 📌 Overview
This program takes **four integer inputs** from the user:
- Sam’s number
- Tina’s number
- Raj’s number
- Mira’s number

It then checks three logical conditions and prints whether each condition is `true` or `false`.

---

## 🧮 Conditions Checked

1. **Condition 1**:  
   Is the average of **Sam’s and Tina’s numbers** greater than the average of **Raj’s and Mira’s numbers**?  
   ```java
   condition1 = ((sam + tina) / 2.0) > ((raj + mira) / 2.0);
Condition 2:
Is the product of Sam’s and Raj’s numbers not equal to the sum of Tina’s and Mira’s numbers?

java
Copy
Edit
condition2 = ((sam * raj) != (tina + mira));
Condition 3:
Is the sum of all four numbers divisible by the difference between Sam’s and Tina’s numbers?

java
Copy
Edit
condition3 = ((sam + tina + raj + mira) % (sam - tina) == 0);
▶️ How to Run
Save the program as Main.java.

Open terminal and navigate to the folder containing the file.

Compile the program:

bash
Copy
Edit
javac Main.java
Run the program:

bash
Copy
Edit
java Main
Enter four integers when prompted.

🖥️ Example Input & Output
Input
Copy
Edit
10
20
15
25
Output
pgsql
Copy
Edit
Is the average of Sam's and Tina's numbers greater than the average of Raj's and Mira's numbers? false
Is the product of Sam's and Raj's numbers not equal to the sum of Tina's and Mira's numbers? true
Is the sum of all four numbers divisible by the difference between Sam's and Tina's numbers? true
```
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int sam = sc.nextInt();
        int tina = sc.nextInt();
        int raj = sc.nextInt();
        int mira = sc.nextInt();

        // Condition 1: Compare averages
        boolean condition1 = ((sam + tina) / 2.0) > ((raj + mira) / 2.0);

        // Condition 2: Product vs sum
        boolean condition2 = ((sam * raj) != (tina + mira));

        // Condition 3: Divisibility check
        boolean condition3 = ((sam + tina + raj + mira) % (sam - tina) == 0);

        // Output
        System.out.println("Is the average of Sam's and Tina's numbers greater than the average of Raj's and Mira's numbers? " + condition1);
        System.out.println("Is the product of Sam's and Raj's numbers not equal to the sum of Tina's and Mira's numbers? " + condition2);
        System.out.println("Is the sum of all four numbers divisible by the difference between Sam's and Tina's numbers? " + condition3);
    }
}
```
