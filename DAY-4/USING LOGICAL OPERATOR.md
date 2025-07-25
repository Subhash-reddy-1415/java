# Java Voting Eligibility Checker 🗳️

This is a simple Java program that checks whether a person is eligible to vote based on their age and country.

---

## 🧾 Description

The program prompts the user to:
- Enter their age (as an integer)
- Enter their country name (as a string)

It then checks if:
- The age is **18 or older**
- The country entered (case-insensitive) is **India**

If both conditions are true, it prints a message saying the user is eligible to vote. Otherwise, it informs the user they are not eligible.

---
```
## 💻 Sample Output

```text
ENTER YOUR AGE=
20
SELECT YOUR COUNTRY=
India
CONGRATES YOU ARE ELEGIBAL FOR VOTING
import java.util.Scanner; // imports Scanner class for user input

class Logical {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in); // creating Scanner object

        System.out.println("ENTER YOUR AGE= ");
        int age = sc.nextInt(); // reads age as an integer
        sc.nextLine(); // consumes the leftover newline

        System.out.println("SELECT YOUR COUNTRY = ");
        String country = sc.nextLine(); // reads country name
        String lower = country.toLowerCase(); // converts to lowercase for case-insensitive check

        // Checks if age is 18 or older AND country is 'india'
        if (age >= 18 && lower.equals("india")) {
            System.out.println("CONGRATES YOU ARE ELIGIBAL FOR VOTING ");
        } else {
            System.out.println("SORRY YOU ARE NOT ELIGIBAL");
        }
    }
}
```
