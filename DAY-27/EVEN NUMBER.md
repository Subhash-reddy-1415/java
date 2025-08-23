markdown# Print Even Numbers from 1 to N Using a While Loop

## Description
This Java program reads an integer `N` from the user and prints all even numbers from 1 to `N` using a while loop. The program is designed as part of the "Programming Essentials" module, Topic 2: Looping Constructs.

## Requirements
- Java Development Kit (JDK) 13.0.1 or higher

## How to Run
1. Ensure JDK is installed and configured on your system.
2. Copy the code into a file named `Main.java`.
3. Compile the program using the command: `javac Main.java`
4. Run the program using the command: `java Main`
5. Enter an integer `N` when prompted.

## Code
```java
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int N = scanner.nextInt();
        int i = 2; // Start from 2 since we want even numbers
        while (i <= N) {
            System.out.println(i);
            i += 2; // Increment by 2 to get the next even number
        }
    }
}
Sample Input and Output

Input: 5

Output:
text2
4



Input: 10

Output:
text2
4
6
8
10




Notes

The program only prints even numbers up to the input value N.
Ensure the input is a positive integer for expected results.
