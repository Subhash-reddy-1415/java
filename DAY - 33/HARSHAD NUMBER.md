Harshad Number Program in Java

This program checks whether a given number is a Harshad Number (also known as a Niven Number).
A Harshad number is an integer that is divisible by the sum of its digits.



harshad_number.java

💻 Code
public class harshad_number {

    public static void main(String[] args) {
        int number = 18;
        int temp = number;
        int result = 0;

        // Step 1: Calculate sum of digits
        while (temp != 0) {
            int rem = temp % 10;
            result += rem;
            temp = temp / 10;
        }

        // Step 2: Check divisibility
        if (number % result == 0) {
            System.out.println("NUMBER IS A HARSHAD NUMBER");
        } else {
            System.out.println("NUMBER IS NOT A HARSHAD NUMBER");
        }
    }
}

✅ Sample Output
NUMBER IS A HARSHAD NUMBER

⚙️ Explanation

Step 1: Extract each digit using % 10 and calculate the sum of digits.

Step 2: Divide the number by the sum of its digits.

If the remainder is 0, the number is a Harshad Number.
Otherwise, it is not.

Example:
For 18:
Sum of digits = 1 + 8 = 9
Since 18 % 9 == 0, → 18 is a Harshad Number

🎯 Usage

Save the file as harshad_number.java

Compile it using:

javac harshad_number.java


Run the program using:

java harshad_number

🧮 Example Tests
Number	Sum of Digits	Divisible?	Result
18	9	✅	Harshad Number
21	3	✅	Harshad Number
19	10	❌	Not Harshad Number
