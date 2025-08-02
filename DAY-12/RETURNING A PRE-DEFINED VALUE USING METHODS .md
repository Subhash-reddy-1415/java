 README for This Exercise

Copy
Edit
# Java Program: Returning a Predefined Boolean Value

## 🔍 Description
This Java program defines a static method `getBooleanValue()` that returns a predefined boolean value `true`. It uses a simple comparison operation between two integers and returns the result.

## 📌 Method Signature
```java
public static boolean getBooleanValue()
Returns: true if the first number is greater than the second, otherwise false.

🧪 Example
java
Copy
Edit
Input:  a = 3, b = 2
Output: true
💡 Concepts Used
Boolean data type

Comparison operators (>)

Static method returning a boolean

🚀 How to Run
Compile and run:

bash
Copy
Edit
javac Main.java
java Main
🧠 Learning Outcome
Learn how to return a boolean from a method

Understand comparison and boolean logic in Java
```
class Main {
    public static void main(String[] args) {
        boolean value = getBooleanValue();
        System.out.println(value);
    }

    public static boolean getBooleanValue() {
        int a = 3;
        int b = 2;
        boolean c = a > b;
        return c;
    }
}
```
