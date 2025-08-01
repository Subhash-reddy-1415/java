📘 README: Java Calculator Using Methods
📌 File Name
Calculator.java

📖 Description
This Java program demonstrates the use of different types of methods by performing basic arithmetic operations:

Addition

Subtraction

Multiplication

Division

The program uses all four method types based on argument and return combinations.

🔧 Features Demonstrated
Method	Description
Add()	No arguments, no return value
Sub(int, int)	With arguments, no return value
Mull()	No arguments, returns value
Div(int, int)	With arguments, returns value
🧪 Sample Output
diff
Copy
Edit
30
-10
200
2.0
SUBHASH REDDY
🛠️ How to Run
Save the file as Calculator.java inside a folder named methods

Open terminal/command prompt and compile:

bash
Copy
Edit
javac methods/Calculator.java
Run the program:

bash
Copy
Edit
java methods.Calculator

```
public class Calculator {
    public static void main(String[] args) {
        int a = 10, b = 20;

        Add();          // No arguments, no return
        Sub(a, b);      // With arguments, no return
        Mull();         // No arguments, returns value
        Div(a, b);      // With arguments, returns value

        System.out.println("SUBHASH REDDY");
    }

    public static void Add() {
        int a = 10, b = 20;
        System.out.println(a + b);
    }

    public static void Sub(int a, int b) {
        System.out.println(a - b);
    }

    public static int Mull() {
        int a = 10, b = 20;
        int result = a * b;
        System.out.println(result);
        return result;
    }

    public static double Div(int a, int b) {
        double result = (double) b / a;
        System.out.println(result);
        return result;
    }
}
```
