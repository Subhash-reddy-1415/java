📄 README.md

Copy
Edit
# User Registration Info – Java Program

## 📌 Description

This Java application simulates a **user registration** system for a learning platform. It prints user details such as:

- Name
- Email
- Date of Birth
- Gender
- Employment status

This task demonstrates how to use:
- `String` for text data
- `char` for gender
- `boolean` for employment status

---

## ✅ Subtasks

### Subtask 1 – Gender Storage
- Data type used: `char`
- Values accepted: `'M'`, `'F'`, `'O'`
- Example: `char gender = 'M';`

### Subtask 2 – Employment Status
- Data type used: `boolean`
- Value used: `false` (can also be `true`)
- Example: `boolean isEmployed = false;`

---

## 🔧 How to Run

1. Save the file as `Main.java`
2. Compile:
   ```bash
   javac Main.java
Run:

bash
Copy
Edit
java Main
🧪 Sample Output
vbnet
Copy
Edit
Name: John Doe
Email: john.doe@example.com
Date of Birth: 01/01/1990
Gender: M
Employed: false
📚 Learning Goals
Understand primitive types (char, boolean)

Use System.out.println() for output

Learn basic variable declaration and initialization


// Java program to simulate user registration data
```
public class Main {
    public static void main(String[] args) {
        // Store and display user name
        String name = "John Doe";
        
        // Store and display email
        String email = "john.doe@example.com";

        // Store and display date of birth
        String dob = "01/01/1990";

        // Store and display gender using char data type ('M', 'F', 'O')
        char gender = 'M';

        // Store and display employment status using boolean
        boolean isEmployed = false;

        // Output the user details
        System.out.println("Name: " + name);
        System.out.println("Email: " + email);
        System.out.println("Date of Birth: " + dob);
        System.out.println("Gender: " + gender);
        System.out.println("Employed: " + isEmployed);
    }
}
```
