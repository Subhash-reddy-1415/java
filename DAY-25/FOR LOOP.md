Counting Down with a For Loop
This Java program reads an integer N from the user and prints the numbers from N down to 1, each on a new line, using a for loop.

How to Run
Ensure you have Java (OpenJDK 13.0.1 or later) installed.

Compile the code using javac Main.java.

Run the program using java Main.

Enter an integer when prompted.

Sample Input
5
Sample Output
5
4
3
2
1
Notes
The program uses the Scanner class to read user input.

A for loop is used to iterate from N down to 1.
```
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int N = scanner.nextInt();
        // Iterate from N down to 1 and print each number
        for (int i = N; i > 0; i--) {
            System.out.println(i);
        }
        scanner.close();
    }
}
```
