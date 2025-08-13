README
Program Name
Simple Operations in Java

Overview
This Java program takes two integers (a and b) from the user and performs the following operations:

Modulus (%)
Calculates the remainder when a is divided by b.
Example: 11 % 6 = 5

Pre-Increment (++a)
Increases the value of a by 1 before using it in an expression.

Pre-Decrement (--b)
Decreases the value of b by 1 before using it in an expression.

Bitwise AND (&)
Compares each bit of a and b; sets the result bit to 1 if both bits are 1.

Bitwise OR (|)
Compares each bit of a and b; sets the result bit to 1 if at least one bit is 1.

Code
java
Copy
Edit
```
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Read input
        int a = sc.nextInt();
        int b = sc.nextInt();

        // Modulus
        int result = a % b;
        System.out.println("Modulus result: " + result);

        // Pre-Increment
        result = ++a;
        System.out.println("Increment result: " + result);

        // Pre-Decrement
        int resu = --b;
        System.out.println("Decrement result: " + resu);

        // Bitwise AND
        int res = a & b;
        System.out.println("Bitwise AND result: " + res);

        // Bitwise OR
        int re = a | b;
        System.out.println("Bitwise OR result: " + re);
    }
}
```
Example Execution
Input:

Copy
Edit
12
7
Output:

sql
Copy
Edit
Modulus result: 5
Increment result: 13
Decrement result: 6
Bitwise AND result: 4
Bitwise OR result: 15
Requirements
Java JDK 8 or later

Any Java compiler or IDE

How to Run
Save the file as Main.java

Compile:

bash
Copy
Edit
javac Main.java
Run:

bash
Copy
Edit
java Main
Enter two integers when prompted.
