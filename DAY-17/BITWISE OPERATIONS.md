README
Program Name
Bitwise Operations on Two Integers

Overview
This Java program reads two integers a and b from the user and performs the following bitwise operations:

Bitwise XOR (^) – Compares each bit of a and b and returns 1 where bits differ, 0 where they are the same.

Left Shift (<<) – Shifts bits of a to the left by one position (equivalent to multiplying by 2).

Right Shift (>>) – Shifts bits of b to the right by one position (equivalent to dividing by 2).

Code
java
Copy
Edit
```
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Read two integers from user
        int a = sc.nextInt();
        int b = sc.nextInt();

        // Bitwise XOR
        int result = a ^ b;
        System.out.println("Bitwise XOR result: " + result);

        // Left Shift
        int resul = a << 1;
        System.out.println("Left Shift result: " + resul);

        // Right Shift
        int resu = b >> 1;
        System.out.println("Right Shift result: " + resu);
    }
}
```
Sample Input / Output
Example:

sql
Copy
Edit
Input:
12
7

Output:
Bitwise XOR result: 11
Left Shift result: 24
Right Shift result: 3
Requirements
Java JDK 8 or higher

Any Java IDE or command-line setup

How to Run
Save the code as Main.java.

Open a terminal in the file location.

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

