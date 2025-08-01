 README for This Exercise
markdown
Copy
Edit
# Java Program: Division of Two Float Numbers

## 🔍 Description
This Java program defines a static method to calculate and return the quotient of two float values. It demonstrates method creation and floating-point arithmetic.

## 📌 Method Signature
```java
public static float quotient(float a, float b)
Parameters:

a: Dividend (float)

b: Divisor (float)

Returns: Result of division a / b as a float.

🧪 Example
java
Copy
Edit
Input:  a = 18f, b = 6f
Output: 3.0
💡 Concepts Used
Static methods

Float data type

Division and return statements

🚀 How to Run
Compile and run:

bash
Copy
Edit
javac Main.java
java Main
```
class Main {
    public static void main(String[] args) {
        float a = 18f;
        float b = 6f;
        float d = quotient(a, b);
        System.out.println(d);
    }

    public static float quotient(float a, float b) {
        float s = a / b;
        return s;
    }
}
```
