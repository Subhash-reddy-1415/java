Java Data Types Example
This repository contains a simple Java program demonstrating the usage of basic data types in Java.
Description
The program showcases the following Java data types:

byte
short
int
long
float
double
char
boolean

Each data type is illustrated with a creative example, printing a message to the console.
How to Run

Ensure you have Java Development Kit (JDK) installed.
Clone this repository: git clone <repository-url>.
Navigate to the project directory: cd <project-directory>.
Compile the code: javac Main.java.
Run the program: java Main.

Output
The program will print a series of messages, each demonstrating the value and usage of a different data type.
Contributing
Feel free to fork this repository and submit pull requests for improvements or additional examples.
License
This project is licensed under the MIT License.



```
public class Main {
    public static void main(String[] args) {
        byte b = 100;
        System.out.println("Byte the squirrel stored " + b + " acorns, each fitting perfectly in its 8-bit paws.");

        short s = 20000;
        System.out.println("Shorty the elf could count up to " + s + " magical mushrooms in the forest.");

        int a = 1000000;
        System.out.println("Int the giant kept track of his vast treasure hoard, numbering " + a + " coins.");

        long l = 1000000000L;
        System.out.println("Longinus the wizard recorded the history of the universe on his " + l + " year-old scroll.");

        float f = 3.14f;
        System.out.println("Floatina the fairy danced on the surface of a pond, measuring its " + f + " foot depth with single-precision.");

        double d = 3.141592653589793;
        System.out.println("Doubleon the dragon soared through the sky, calculating distances with " + d + " double-precision accuracy.");

        char c = 'A';
        System.out.println("Charli the artist painted the letter " + c + " in the kingdom, one Unicode character at a time.");

        boolean t = true;
        System.out.println("The Boolean Guardians, True and False, decided the fate of the kingdom with simple " + t + " or false answers.");
    }
}
```
