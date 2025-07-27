 Java Program: Unary Operators with Pre/Post Increment & Decrement
📌 Program Name: Main.java
📚 Purpose:
This program helps in understanding the behavior of unary increment (++) and decrement (--) operators in both prefix (pre) and postfix (post) forms by evaluating complex expressions and tracing variable values step by step.

🧠 Concepts Covered:
Operator	Name	Description
a++	Post-Increment	Use value, then increment a
++a	Pre-Increment	Increment a, then use value
a--	Post-Decrement	Use value, then decrement a
--a	Pre-Decrement	Decrement a, then use value

💻 Program Flow:
The user is asked to input a value for variable a.

Various expressions are computed using pre and post increment/decrement operators.

After each expression, the result and current value of a are printed for clarity.

🧪 Sample Input:
java
Copy
Edit
ENTER THE A VALUE = 5
✅ Expected Output:
java
Copy
Edit
RESULT OF A = 6
RESULT OF B = 5
RESULT OF A = 9
RESULT OF C = 22
RESULT OF A = 15
RESULT OF D = 23
RESULT OF A = 13
RESULT OF E = 28
🔍 Expression Breakdown:
int b = a++;

b = 5, then a = 6

int c = a++ + ++a + a++;

Use: 6 + 8 + 8 = 22, then a = 9

int d = ++a + ++a + ++a - a++ - a++ + ++a;

d = 10 + 11 + 12 - 12 - 13 + 15 = 23, then a = 15

int e = a-- + --a + a++ - --a;

e = 15 + 13 + 13 - 13 = 28, then a = 13

🧠 What You Learn:
How Java evaluates expressions involving both pre and post increment/decrement.

Why order of evaluation affects the final result.

The difference between using and updating a variable’s value.

🛠️ How to Compile and Run:
Save the file as Main.java

Open terminal or command prompt

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
import java.util.Scanner;
```
class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Get input from the user
        System.out.print("ENTER THE A VALUE = ");
        int a = sc.nextInt();  // Let's say user enters: 5

        // POST-INCREMENT: assigns 'a' to 'b', then increments 'a'
        int b = a++;           // b = 5, a becomes 6
        System.out.println("RESULT OF A = " + (a));  // 6
        System.out.println("RESULT OF B = " + (b));  // 5

        // a is currently 6
        // Evaluate: a++ + ++a + a++
        // a++ → use 6, then a = 7
        // ++a → a = 8, use 8
        // a++ → use 8, then a = 9
        // c = 6 + 8 + 8 = 22
        int c = a++ + ++a + a++;  
        System.out.println("RESULT OF A = " + (a));  // 9
        System.out.println("RESULT OF C = " + (c));  // 22

        // a is currently 9
        // Evaluate: ++a + ++a + ++a - a++ - a++ + ++a
        // ++a → a = 10, use 10
        // ++a → a = 11, use 11
        // ++a → a = 12, use 12
        // a++ → use 12, then a = 13
        // a++ → use 13, then a = 14
        // ++a → a = 15, use 15
        // d = 10 + 11 + 12 - 12 - 13 + 15 = 23
        int d = ++a + ++a + ++a - a++ - a++ + ++a;
        System.out.println("RESULT OF A = " + (a));  // 15
        System.out.println("RESULT OF D = " + (d));  // 23

        // a is currently 15
        // Evaluate: a-- + --a + a++ - --a
        // a-- → use 15, then a = 14
        // --a → a = 13, use 13
        // a++ → use 13, then a = 14
        // --a → a = 13, use 13
        // e = 15 + 13 + 13 - 13 = 28
        int e = a-- + --a + a++ - --a;
        System.out.println("RESULT OF A = " + (a));  // 13
        System.out.println("RESULT OF E = " + (e));  // 28
    }
}
```
