Decimal to Binary Conversion (Java)
📘 Overview

This Java program converts a given decimal number into its binary equivalent without using built-in methods.
It performs step-by-step division by 2 and constructs the binary number using integer arithmetic.

📂 File

DecimalToBinary.java

💻 Code
public class DecimalToBinary {

    public static void main(String[] args) {
        int number = 10;
        int i = 1;
        int bin = 0;

        while (number != 0) {
            int digit = number % 2;   // Get remainder (binary digit)
            bin = (digit * i) + bin;  // Place digit in correct position
            number /= 2;              // Divide by 2
            i *= 10;                  // Move to next place value
        }

        System.out.println(bin);
    }
}

🧠 Explanation
Step	Operation	Result
1	Take the remainder when dividing by 2 (number % 2)	Gives the next binary digit
2	Multiply by i to place digit at correct position	Builds binary number step by step
3	Divide number by 2 (number /= 2)	Move to next binary digit
4	Multiply i by 10 (i *= 10)	Shift place for next binary digit
5	Repeat until number == 0	Binary number complete
🧩 Example

Input:
number = 10

Process:

10 / 2 → remainder 0
5 / 2  → remainder 1
2 / 2  → remainder 0
1 / 2  → remainder 1


Binary digits (reversed): 1010

Output:

1010

⚙️ Output Examples
Decimal	Binary
2	10
5	101
8	1000
10	1010
15	1111
🧩 Key Concepts Used
Concept	Description
Modulo (%)	Extracts remainder (binary bit)
Integer Division (/)	Reduces number by 2 each iteration
Place Value (×10)	Builds binary result in correct order
Loop (while)	Repeats until number becomes 0
🚀 Optional Enhancement

You can modify the code to allow user input:

import java.util.Scanner;

public class DecimalToBinary {

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter a decimal number: ");
        int number = sc.nextInt();

        int i = 1;
        int bin = 0;
        while (number != 0) {
            int digit = number % 2;
            bin = (digit * i) + bin;
            number /= 2;
            i *= 10;
        }

        System.out.println("Binary: " + bin);
    }
}
