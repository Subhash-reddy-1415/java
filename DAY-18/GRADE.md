📌 Overview

The Grade-o-Matic program evaluates and assigns a grade to a student based on their score.
It uses Java's if-else conditional statements to determine the grade according to predefined score ranges.

🛠 Features

Score Initialization: Sets a student's score in the program.

Grade Evaluation: Checks the score range and assigns the appropriate grade.

Custom Messages: Displays feedback based on performance.

📄 Code Explanation
1. Score Declaration
int score = 85;


An integer variable score stores the student's marks.

Here, 85 is assigned as an example value.
```
import java.util.Scanner;

public class GradeOMatic {
    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);

        // Asking user for score
        System.out.print("Enter the student's score (0-100): ");
        int score = sc.nextInt();

        // Grade Evaluation
        if(score >= 90 && score <= 100){
            System.out.println("Grade A: Excellent");
        }
        else if(score >= 80 && score <= 89){
            System.out.println("Grade B: Very Good");
        }
        else if(score >= 70 && score <= 79){
            System.out.println("Grade C: Good");
        }
        else if(score >= 60 && score <= 69){
            System.out.println("Grade D: Needs Improvement");
        }
        else if(score >= 0 && score < 60){
            System.out.println("Grade F: Fail");
        }
        else{
            System.out.println("Invalid score! Please enter a value between 0 and 100.");
        }

        sc.close();
    }
}
```


if statement: Checks if score is between 90 and 100 (inclusive) → Grade A.

else if statements: Check for other ranges:

80–89 → Grade B

70–79 → Grade C

60–69 → Grade D

else statement: Covers all other scores → Grade F.

📊 Example Output

If score = 85:

Grade B: Very Good

🚀 How to Run

Save the code as Main.java.

Compile the program:

javac Main.java


Run the program:

java Main
