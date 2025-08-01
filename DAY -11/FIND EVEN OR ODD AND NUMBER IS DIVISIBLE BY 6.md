 README: Java Number Check (Demo.java)
📌 File Name
Demo.java

📖 Description
This Java program performs two number checks using separate static methods:

Checks if an integer is odd or even using the ternary operator

Checks if a number is divisible by 6 using an if-else condition

🔍 Functional Overview
✅ Method 1: checkOdd(int a)
Uses ternary operator to check if the integer a is odd or even.

Prints "Odd" or "Even".

✅ Method 2: divisibleBy3(double y)
Checks if y is divisible by 6.

If y % 6 == 0, prints:
y IS DIVISIBLE BY 6

Else, prints:
y IS NOT DIVISIBLE BY 6

🔢 Sample Code Output
java
Copy
Edit
int x = 11;
double y = 12;
Output:
vbnet
Copy
Edit
Odd
12.0  IS DIVISIBLE BY 6
💡 Concepts Used
Ternary Operator ? :

Modulus operator %

Static method calls

int and double data types

Conditional branching (if-else)

🧪 Sample Test Cases
Input (x, y)	Output
7, 18	Odd
18.0 IS DIVISIBLE BY 6
8, 25	Even
25.0 IS NOT DIVISIBLE BY 6

⚙️ How to Compile and Run
bash
Copy
Edit
javac Demo.java
java Demo
```
public class Demo {

    public static void checkOdd(int a) {
  String result = (a % 2!=0) ? "Odd" : "Even";
  System.out.println(result);
    }
    public static void divisibleBy3(double y) {
    if (y % 6 == 0) {
    	System.out.println(y + "  IS DIVISIBLE BY 6");
    }
    else {
    	System.out.println(y + "  IS NOT DIVISIBLE BY 6");
    }
    }

    public static void main(String[] args) {
    	int x = 11;
    	double y = 12;
    	Demo.checkOdd(x);
    	Demo.divisibleBy3(y);
    }
    
    ```
