 README: Your Own Cute Coffee Shop ☕
📌 Overview
This Java project simulates a simple coffee shop system that displays orders for coffee and cookies using methods with and without parameters and with different return types. It demonstrates Java basics like:

Static methods

Method overloading

Method return types (void, String)

System.out.println() for displaying output

✅ Features Implemented
Coffee Order (Default)

Method: orderCoffee()

Return Type: void

Function: Prints "Ordered a default coffee."

Coffee Order (Custom Type)

Method: orderCoffee(String type)

Return Type: void

Function: Prints "Ordered a <type> coffee."

Cookie Order (Default)

Method: orderCookie()

Return Type: String

Function: Returns "Ordered a default cookie."

Cookie Order (Custom Type)

Method: orderCookie(String type)

Return Type: String

Function: Returns "Ordered a <type> cookie."

💡 Sample Output
java
Copy
Edit
Ordered a default coffee.
Ordered a Espresso coffee.
Ordered a default cookie.
Ordered a Chocolate Chip cookie.
🧠 What You Learn
How to define and use methods with different signatures

How to use method overloading

Difference between methods that return values and methods that just perform actions

String concatenation and return in Java

📂 File Structure
Only one file is needed:

css
Copy
Edit
Main.java
🚀 How to Run
Compile the code:

bash
Copy
Edit
javac Main.java
Run the program:

bash
Copy
Edit
java Main
```
public class Main {

    // Method 1: No parameter, no return type
    public static void orderCoffee() {
        System.out.println("Ordered a default coffee.");
    }

    // Method 2: Parameter, no return type
    public static void orderCoffee(String type) {
        System.out.println("Ordered a " + type + " coffee.");
    }

    // Method 3: No parameter, returns String
    public static String orderCookie() {
        return "Ordered a default cookie.";
    }

    // Method 4: Parameter, returns String
    public static String orderCookie(String type) {
        return "Ordered a " + type + " cookie.";
    }

    public static void main(String[] args) {
        // Calling coffee methods
        orderCoffee();                      // Default coffee
        orderCoffee("Espresso");            // Custom coffee

        // Calling cookie methods
        String cookieOrder1 = orderCookie();                       // Default cookie
        System.out.println(cookieOrder1);

        String cookieOrder2 = orderCookie("Chocolate Chip");       // Custom cookie
        System.out.println(cookieOrder2);
    }
}
```
