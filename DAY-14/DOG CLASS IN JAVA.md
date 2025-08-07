✅ README.md
markdown
Copy
Edit
# Simple Dog Class in Java

## Objective
To create a basic Java program demonstrating:
- Class creation
- Object instantiation
- Method invocation

## Description
This project contains:
- A `Dog` class with a `bark()` method that prints a barking message.
- A `Main` class that creates a `Dog` object and calls its `bark()` method.

## Files
- `Dog.java`: Defines the `Dog` class with a `String` field and `bark()` method.
- `Main.java`: Contains the `main()` method where the program runs.

## How to Compile and Run
```bash
javac Dog.java Main.java
java Main
Output
csharp
Copy
Edit
Dog is barking.
Key Concepts
Object-Oriented Programming

Method declaration and invocation

String field usage in a class

yaml
Copy
Edit
```
// Dog.java
class Dog {
    String pet;

    // Method to simulate the dog barking
    void bark() {
        System.out.println(pet + " is barking.");
    }
}
// Main.java
public class Main {
    public static void main(String[] args) {
        Dog myPet = new Dog();   // Create a Dog object
        myPet.pet = "Dog";       // Assign value to 'pet'
        myPet.bark();            // Call the bark method
    }
}
```
