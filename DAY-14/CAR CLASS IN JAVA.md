✅ README.md
markdown
Copy
Edit
# Simple Car Class in Java

## Description
This Java program demonstrates the concept of a class and object in Java. A class `Car` is defined with a method `drive()` that prints a message when called. An object of the `Car` class is created in the `Main` class and used to invoke the `drive()` method.

## Files
- `Car.java`: Contains the `Car` class with a `vehicle` field and `drive()` method.
- `Main.java`: Contains the `main()` method that creates an object of `Car` and calls `drive()`.

## How to Compile and Run
```bash
javac Car.java Main.java
java Main
Output
csharp
Copy
Edit
Car is being driven.
Concepts Used
Class and Object

Method definition and invocation
```
String variable assignment
// Car.java
class Car {
    String vehicle;

    // Method to simulate driving the car
    void drive() {
        System.out.println(vehicle + " is being driven.");
    }
}
// Main.java
public class Main {
    public static void main(String[] args) {
        Car myCar = new Car();
        myCar.vehicle = "Car";  // Assign name to the vehicle
        myCar.drive();          // Output: Car is being driven.
    }
}


Car is being driven.

```
