🚀 Automorphic Number Checker (Java)

This Java program checks whether a given number is an Automorphic number.
A number is automorphic if its square ends with the same digits as the number itself.

📂 File

Automorphic.java

💻 Code Example
public class Automorphic {

    public static void main(String[] args) {
        int number = 25;
        if (isAutomorphic(number)) {
            System.out.println("It's an Automorphic number");
        } else {
            System.out.println("It's not an Automorphic number");
        }
    }

    public static boolean isAutomorphic(int number) {
        int square = number * number;
        while (number != 0) {
            int num = number % 10;
            int squ = square % 10;

            if (num != squ) {
                return false;
            }

            number = number / 10;
            square = square / 10;
        }
        return true;
    }
}

🧠 Explanation

Compute the square of the number.

Compare the last digits of the number and its square using modulus (% 10).

Continue dividing both by 10 until all digits of the number are checked.

If all digits match → Automorphic.

✅ Example Output
It's an Automorphic number

⚙️ Test More Examples
Input	Output
5	Automorphic
6	Automorphic
25	Automorphic
7	Not Automorphic
76	Automorphic
🧩 Key Concepts Used
Concept	Description
Modulus operator (%)	Extracts the last digit
Looping (while)	Iteratively compares digits
Conditional (if)	Checks equality of digits
Mathematical logic	Compares digits of number and square
