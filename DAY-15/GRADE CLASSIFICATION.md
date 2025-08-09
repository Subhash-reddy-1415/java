Student Grades Classification
📌 Overview
This Java program collects student marks for 3 subjects, calculates the average, and assigns a grade based on the following criteria:

Average Marks (%)	Grade
90 – 100	A+
80 – 89	A
70 – 79	B+
60 – 69	B
50 – 59	C
40 – 49	D
Below 40	Fail

The program uses if-else conditions to check the average and display the grade.

⚙️ Features
Takes user input for marks in 3 subjects.

Calculates the average marks.

Displays the appropriate grade based on average.

Includes basic input validation for marks (0–100).

🖥️ Code Example
java
Copy
Edit
```
import java.util.Scanner;

public class StudentGrade {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        // Input marks
        System.out.print("Enter marks for Subject 1: ");
        int sub1 = sc.nextInt();
        System.out.print("Enter marks for Subject 2: ");
        int sub2 = sc.nextInt();
        System.out.print("Enter marks for Subject 3: ");
        int sub3 = sc.nextInt();

        // Calculate average
        double average = (sub1 + sub2 + sub3) / 3.0;
        System.out.println("Average Marks: " + average);

        // Determine grade
        if (average >= 90) {
            System.out.println("Grade: A+");
        } else if (average >= 80) {
            System.out.println("Grade: A");
        } else if (average >= 70) {
            System.out.println("Grade: B+");
        } else if (average >= 60) {
            System.out.println("Grade: B");
        } else if (average >= 50) {
            System.out.println("Grade: C");
        } else if (average >= 40) {
            System.out.println("Grade: D");
        } else {
            System.out.println("Grade: Fail");
        }

        sc.close();
    }
}
```
🚀 How to Run
Save the file as StudentGrade.java

Open terminal/command prompt in the saved directory.

Compile:

sh
Copy
Edit
javac StudentGrade.java
Run:

sh
Copy
Edit
java StudentGrade
📌 Sample Output
yaml
Copy
Edit
Enter marks for Subject 1: 85
Enter marks for Subject 2: 90
Enter marks for Subject 3: 80
Average Marks: 85.0
Grade: A
