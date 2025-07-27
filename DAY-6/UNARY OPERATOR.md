 Unary Operators in Java
📌 Program Name: Uni.java
📚 Purpose:
This Java program demonstrates the use of unary increment (++) and decrement (--) operators, both in prefix and postfix forms.

🧠 Unary Operators Covered:
Operator	Description	Syntax
++a	Pre-increment: increments, then uses the value	Prefix
a++	Post-increment: uses the value, then increments	Postfix
--a	Pre-decrement: decrements, then uses the value	Prefix
a--	Post-decrement: uses the value, then decrements	Postfix

💻 How the Program Works:
Takes one integer input a from the user.

Applies and prints the result of:

Post-increment (a++)

Pre-increment (++a)

Post-decrement (a--)

Pre-decrement (--a)

🧪 Sample Input/Output:
Input:

java
Copy
Edit
ENTER THE A VALUE = 5
Output:

pgsql
Copy
Edit
POST INCREMENT 5
PRE-INCREMENT 7
POST DECREMENT 7
PRE-DECREMENT 5
Explanation:

Operation	Before Value	Printed Value	After Value
a++	5	5	6
++a	6	7	7
a--	7	7	6
--a	6	5	5

💻 How to Run the Program:
Save the file as Uni.java

Open terminal and compile:

bash
Copy
Edit
javac Uni.java
Run the program:

bash
Copy
Edit
java Uni
✅ Concepts Practiced:
Using Scanner class for user input

Understanding post and pre unary increment/decrement

Printing expressions with operator evaluation
```
import java.util.Scanner;
public class Uni {
    public static void main(String[] args) {
          Scanner sc = new Scanner(System.in);
          System.out.print("ENTER THE A VALUE = ");
          int a = sc.nextInt();                 // User inputs 'a'
          System.out.println("POST INCREMENT "+(a++));  // Prints current a, then a = a + 1
          System.out.println("PRE-INCREMENT "+(++a));   // First a = a + 1, then print
          System.out.println("POST DECREMENT "+(a--));  // Prints current a, then a = a - 1
          System.out.println("PRE-DECREMENT "+(--a));   // First a = a - 1, then print
      }
}
```
