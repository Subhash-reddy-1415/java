📌 Program Overview
This Java program demonstrates the use of logical operators (&&, ||, ^) with integers and string comparison using .equals().

✅ Features
Accepts two integers from the user.

Uses logical AND, logical OR, and logical XOR to compare the integers.

Accepts two strings (first name and last name).

Compares strings using .equals() to check for an exact match.

🧮 Logical Operators Used
Operator	Name	Description
&&	Logical AND	Returns true if both conditions are true.
`		`
^	Logical XOR	Returns true if only one condition is true.

🔤 String Comparison
Strings are compared using .equals() because == compares memory references, not content.

Example:

java
Copy
Edit
name1.equals("SUBHASH") && name2.equals("REDDYCHARLA")
🧪 Sample Input & Output
sql
Copy
Edit
ENTER A VALUE = 
6
ENTER B VALUE = 
7
LOGICAL AND WITH INTEGERS: true
LOGICAL OR WITH INTEGERS: true
LOGICAL XOR WITH INTEGERS: false
ENTER FIRST NAME = 
SUBHASH
ENTER LAST NAME = 
REDDYCHARLA
YOUR NAME MATCHES: true
import java.util.Scanner;
```
public class Logical {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("ENTER A VALUE = ");
        int a = sc.nextInt();

        System.out.println("ENTER B VALUE = ");
        int b = sc.nextInt();

        System.out.println("LOGICAL AND WITH INTEGERS: " + (a > 5 && b > 5));
        System.out.println("LOGICAL OR WITH INTEGERS: " + (a > 5 || b > 5));
        System.out.println("LOGICAL XOR WITH INTEGERS: " + (a > 5 ^ b > 1));

        sc.nextLine(); // ✅ clear the newline character left after nextInt()

        System.out.println("ENTER FIRST NAME = ");
        String name1 = sc.nextLine();

        System.out.println("ENTER LAST NAME = ");
        String name2 = sc.nextLine();

        System.out.println("YOUR NAME MATCHES: " + (name1.equals("SUBHASH") && name2.equals("REDDYCHARLA")));
    }
}
```
