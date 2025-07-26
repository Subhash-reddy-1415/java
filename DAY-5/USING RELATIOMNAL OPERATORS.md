Relational Operators in Java
📌 Program Name: Rel.java
📚 Purpose:
This Java program demonstrates the use of relational operators by comparing two user-input integers. It evaluates equality, inequality, and magnitude relationships between the two values.

🛠️ Features:
Takes two integer inputs from the user (a and b)

Uses the following relational operators:

== (equal to)

> (greater than)

< (less than)

>= (greater than or equal to)

<= (less than or equal to)

Displays the result of each comparison as a boolean (true or false)

💡 Relational Operators Used:
Operator	Meaning
==	Equal to
>	Greater than
<	Less than
>=	Greater than or equal to
<=	Less than or equal to

🧪 Sample Input/Output:
Input:

nginx
Copy
Edit
ENTER A NUMBER= 
15
ENTER B NUMBER= 
10
Output:

vbnet
Copy
Edit
A IS EQUAL TO B = false
A IS GREATER THAN B = true
A IS LESS THAN B = false
A IS GREATER THAN OR EQUAL TO B = true
A IS LESS THAN OR EQUAL TO B = false
💻 How to Run:
Save the code in a file named Rel.java

Compile the program:

bash
Copy
Edit
javac Rel.java
Run the compiled program:

bash
Copy
Edit
java Rel
🧠 Concepts Learned:
Using Scanner for user input

Applying relational operators in decision making

Printing dynamic results using System.out.println()
```
import java.util.Scanner;

public class Rel {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        System.out.println("ENTER A NUMBER= ");
        int a = sc.nextInt();
        
        System.out.println("ENTER B NUMBER= ");
        int b = sc.nextInt();

        System.out.println("A IS EQUAL TO B = " + (a == b));
        System.out.println("A IS GREATER THAN B = " + (a > b));
        System.out.println("A IS LESS THAN B = " + (a < b));
        System.out.println("A IS GREATER THAN OR EQUAL TO B = " + (a >= b));
        System.out.println("A IS LESS THAN OR EQUAL TO B = " + (a <= b));
    }
}
```
