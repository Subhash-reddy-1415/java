🧾 README — Notification Sender (Java)
📘 Overview

This Java program demonstrates the use of classes, objects, and methods.
The program defines a class Notification that contains a method sender() used to print a success message when called from the Main class.

📂 Files

Main.java

💻 Code
public class Main {
    public static void main(String[] args) {
        new Notification().sender();
    }
}

class Notification {   
    public void sender() {
        System.out.println("Notification send sucessfully.");
    }
}

🧠 Explanation
Step	Description
1	The Main class contains the main() method — the entry point of the program.
2	Inside main(), a new object of the Notification class is created using new Notification().
3	The sender() method is immediately called on the created object.
4	The method prints "Notification send sucessfully." to the console.
🧩 Output
Notification send sucessfully.

⚙️ Key Concepts Used
Concept	Description
Class	Blueprint for creating objects. (Notification and Main)
Object Creation	new Notification() creates a new instance of the class.
Method Calling	.sender() executes the code inside the sender() method.
Access Modifier	public allows methods to be accessed outside their class.
🧩 Alternate Version (Using Object Reference)
public class Main {
    public static void main(String[] args) {
        Notification notification = new Notification();
        notification.sender();
    }
}

class Notification {
    public void sender() {
        System.out.println("Notification send sucessfully.");
    }
}


Output:

Notification send sucessfully.

🧠 Concept Summary

Encapsulation: Logic (printing a message) is wrapped inside a class.

Abstraction: You just call sender() without worrying about internal details.

Object creation and method invocation: Demonstrates Java OOP basics.
