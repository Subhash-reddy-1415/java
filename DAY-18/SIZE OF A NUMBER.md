Determine the Size Category of a Number
📌 Problem Statement

This Java program reads an integer from the user and classifies it into one of three categories:

Small if the number is less than 10.

Medium if the number is between 10 (inclusive) and 99 (inclusive).

Large if the number is 100 or greater.

The classification is done using an if-else ladder.

📂 File Information

File Name: Main.java

Language: Java

Java Version: OpenJDK 13.0.1

📝 Code Explanation
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in); // Create Scanner object to read input
        int number = scanner.nextInt(); // Read integer from user

        // Check number category
        if (number < 10) {
            System.out.println("Small");
        } else if (number >= 10 && number < 100) {
            System.out.println("Medium");
        } else if (number >= 100) {
            System.out.println("Large");
        }
    }
}
```
⚙️ How It Works

Input Handling

Uses Scanner to read an integer from the user.

Decision Making

If the number is less than 10 → Prints "Small".

If the number is between 10 (inclusive) and 100 (exclusive) → Prints "Medium".

If the number is 100 or more → Prints "Large".

Output

Displays the size category of the given number.

💻 Sample Run

Input

5


Output

Small


Input

50


Output

Medium


Input

150


Output

Large

🚀 Usage

Save the file as Main.java.

Compile:

javac Main.java


Run:

java Main


Enter an integer when prompted.
