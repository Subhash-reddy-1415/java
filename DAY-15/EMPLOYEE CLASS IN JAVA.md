 README.md

# Simple Employee Class in Java

## Objective
To demonstrate the basics of Object-Oriented Programming in Java:
- Creating a class
- Defining and calling methods
- Using object fields

## Description
This program defines an `Employee` class with:
- A `String` field `name`
- A `work()` method that prints "`name` is working."

In the `Main` class, we:
1. Create an object of `Employee`
2. Assign a value to `name`
3. Call the `work()` method to display the message

## How to Compile and Run
```bash
javac Employee.java Main.java
java Main
Sample Output
csharp
Copy
Edit
Employee is working.
Key Concepts
Class definition

Object instantiation

Method declaration and invocation

Field assignment

```
// Employee.java
class Employee {
    String name;

    // Method to display working message
    void work() {
        System.out.println(name + " is working.");
    }
}
// Main.java
public class Main {
    public static void main(String[] args) {
        Employee employee1 = new Employee();  // Create Employee object
        employee1.name = "Employee";          // Assign value
        employee1.work();                     // Call method
    }
}
```
