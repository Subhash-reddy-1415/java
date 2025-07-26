Assignment Operators in Java
📌 Program Name: Ass.java
📚 Purpose:
This program demonstrates the use of assignment operators in Java by modifying the variable a using different compound assignment forms (+=, -=, *=, etc.) with a second input b.

🧪 Assignment Operators Used:
Operator	Meaning	Description
+=	Add and assign	a += b → a = a + b
-=	Subtract and assign	a -= b → a = a - b
*=	Multiply and assign	a *= b → a = a * b
/=	Divide and assign	a /= b → a = a / b
%=	Modulo and assign	a %= b → a = a % b
&=	Bitwise AND assign	a &= b → a = a & b (bitwise)
`	=`	Bitwise OR assign

💻 How to Run:
Save the code in a file called Ass.java

Open terminal or command prompt.

Compile the code:

bash
Copy
Edit
javac Ass.java
Run the program:

bash
Copy
Edit
java Ass
🧠 Concepts Demonstrated:
Taking input from the user using Scanner

Using compound assignment operators

Performing bitwise operations (&, |) in combination with assignment
import java.util.Scanner;
```
public class Ass {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("ENTER A VALUE = ");
        int a = sc.nextInt();

        System.out.print("ENTER THE B VALUE = ");
        int b = sc.nextInt();

        // Performing assignment operations
        System.out.println("THE RESULT IS A = A + B : " + (a += b));  // a = a + b
        System.out.println("THE RESULT IS A = A - B : " + (a -= b));  // a = a - b
        System.out.println("THE RESULT IS A = A * B : " + (a *= b));  // a = a * b
        System.out.println("THE RESULT IS A = A / B : " + (a /= b));  // a = a / b
        System.out.println("THE RESULT IS A = A % B : " + (a %= b));  // a = a % b
        System.out.println("THE RESULT IS A = A & B : " + (a &= b));  // a = a & b (bitwise AND)
        System.out.println("THE RESULT IS A = A | B : " + (a |= b));  // a = a | b (bitwise OR)
    }
}
```
