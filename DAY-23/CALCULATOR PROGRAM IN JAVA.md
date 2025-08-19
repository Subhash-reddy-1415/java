📘 Calculator Program in Java
📌 Overview

This project is a simple calculator program in Java that performs basic arithmetic operations (+, -, *, /) using a switch statement.

It demonstrates:

Use of variables

Use of switch-case

Handling of division by zero

Clean and readable Java structure

🛠 Features

Addition

Subtraction

Multiplication

Division (with zero-check)

📂 Code Example
```
public class Main {
    public static void main(String[] args) {
        double num1 = 10.5;
        double num2 = 2.5;
        char operator = '+'; // Change to -, *, /

        switch (operator) {
            case '+':
                System.out.println("Result: " + (num1 + num2));
                break;
            case '-':
                System.out.println("Result: " + (num1 - num2));
                break;
            case '*':
                System.out.println("Result: " + (num1 * num2));
                break;
            case '/':
                if (num2 != 0) {
                    System.out.println("Result: " + (num1 / num2));
                } else {
                    System.out.println("Error: Division by zero not allowed.");
                }
                break;
            default:
                System.out.println("Invalid operator");
        }
    }
}
```
▶️ How to Run

Save the file as Main.java

Open terminal/command prompt in that folder

Compile the code:

javac Main.java


Run the program:

java Main

📊 Sample Output
Result: 13.0

🔮 Future Enhancements

Take input from user (using Scanner) instead of hardcoding values

Add more operations (modulus %, power ^, square root √)

Create a menu-driven calculator
