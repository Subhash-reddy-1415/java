README
Program Name
Ticket Pricing Calculator

Overview
This Java program determines the ticket price based on a person's age group using an if-else ladder.
It prints whether the ticket is free, a child ticket, an adult ticket, or a senior ticket.

Features
Age-based Ticket Pricing

Free Admission: Age < 3

Child Ticket ($10): Age between 3 and 12 (inclusive)

Adult Ticket ($15): Age between 13 and 64 (inclusive)

Senior Ticket ($12): Age 65 and above

Simple Logic Structure

Uses an if-else if-else ladder for clear decision-making.

Code Explanation
java
Copy
Edit
```
public class Main {
    public static void main(String[] args) {
        int age = 12; // Age is set manually

        if(age < 3) {
            System.out.println("Free admission");
        } else if(age >= 3 && age <= 12) {
            System.out.println("Child ticket: $10");
        } else if(age >= 13 && age <= 64) {
            System.out.println("Adult ticket: $15");
        } else {
            System.out.println("Senior ticket: $12");
        }
    }
}
```
Example Output
Example 1:

makefile
Copy
Edit
Input: age = 2
Output: Free admission
Example 2:

makefile
Copy
Edit
Input: age = 12
Output: Child ticket: $10
Example 3:

makefile
Copy
Edit
Input: age = 30
Output: Adult ticket: $15
Example 4:

makefile
Copy
Edit
Input: age = 70
Output: Senior ticket: $12
Requirements
Java JDK 8 or higher

Any Java IDE (Eclipse, IntelliJ IDEA, NetBeans) or Command Prompt

How to Run
Save the file as Main.java

Open a terminal in the folder where the file is saved.

Compile:

bash
Copy
Edit
javac Main.java
Run:

bash
Copy
Edit
java Main
