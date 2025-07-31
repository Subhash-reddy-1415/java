README: Leap Year Checker in Java
📌 Program Name
LeapYearChecker.java

📖 Description
This Java program determines whether a given year is a leap year or not using standard leap year rules.

📅 Leap Year Rules
A year is considered a leap year if:

It is divisible by 400
OR

It is divisible by 4 but not divisible by 100

💡 Example
Year	Result
2024	Leap Year
1900	Not a Leap Year
2000	Leap Year
2023	Not a Leap Year

💻 Code
```t
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("ENTER THE YEAR: ");
        int year = sc.nextInt();

        if ((year % 400 == 0) || (year % 4 == 0 && year % 100 != 0)) {
            System.out.println(year + " IS A LEAP YEAR");
        } else {
            System.out.println(year + " IS NOT A LEAP YEAR");
        }
    }
}
```
🧪 Sample Input & Output
Input:

yaml
Copy
Edit
ENTER THE YEAR: 2020
Output:

css
Copy
Edit
2020 IS A LEAP YEAR
🛠️ How to Run
Save the code in a file named Main.java

Compile using:

css
Copy
Edit
javac Main.java
Run using:

css
Copy
Edit
java Main
