 README 
Copy
Edit
# Java Program: Concatenate Two Strings

## 🔍 Description
This Java program defines a static method to concatenate two strings. It takes two `String` inputs and returns a single string formed by joining them.

## 📌 Method Signature
```java
public static String concatenate(String str1, String str2)
Parameters:

str1: First string

str2: Second string

Returns: Concatenation of str1 + str2

🧪 Example
java
Copy
Edit
Input:  str1 = "Hello, ", str2 = "World!"
Output: Hello, World!
💡 Concepts Used
Static methods

String concatenation using + operator

Return types

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
        String str1 = "Hello, ";
        String str2 = "World!";
        System.out.println(concatenate(str1, str2));
    }

    public static String concatenate(String str1, String str2) {
        return str1 + str2;
    }
}
```
