Java Integer Comparison Example

This repository contains a Java program that demonstrates the use of boolean variables to compare integer values.

Description

The program declares two integer variables and uses comparison operators (>, <, ==, !=) to evaluate their relationships. The results are stored in boolean variables and printed to the console.

How to Run





Ensure you have Java Development Kit (JDK) installed.



Clone this repository: git clone <repository-url>.



Navigate to the project directory: cd <project-directory>.



Compile the code: javac Main.java.



Run the program: java Main.

Output

The program will output the results of the comparisons, e.g.:

5 > 3 = true
5 < 3 = false
5 == 3 = false
5 != 3 = true
```java
public class Main {
    public static void main(String[] args) {
        int a = 5;
        int b = 3;

        boolean greater_than = a > b;
        boolean less_than = a < b;
        boolean equal_to = a == b;
        boolean not_equal = a != b;

        System.out.println(a + " > " + b + " = " + greater_than);
        System.out.println(a + " < " + b + " = " + less_than);
        System.out.println(a + " == " + b + " = " + equal_to);
        System.out.println(a + " != " + b + " = " + not_equal);
    }
}
```
