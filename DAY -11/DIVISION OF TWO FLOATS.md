 README 
Copy
Edit
# Java Program: Efficient Division of Two Floats

## 🔍 Description
This Java program calculates and returns the quotient of two `float` numbers using a static method.

## 📌 Method Signature
```java
public static float quotient(float a, float b)
Parameters:

a → Dividend

b → Divisor

Returns: a / b (as a float)

📦 Example
java
Copy
Edit
Input:  a = 18f, b = 6f
Output: 3.0
💡 Concepts Used
Static methods

Float division

Return types

🚀 How to Run
Compile and run:

bash
Copy
Edit
javac Main.java
java Main

```
\class Main {
    public static void main(String[] args) {
        float a = 18f;
        float b = 6f;
        float d = quotient(a, b);
        System.out.println(d); // Output will be: 3.0
    }

    public static float quotient(float a, float b) {
        float s = a / b;
        return s;
    }
}
```
