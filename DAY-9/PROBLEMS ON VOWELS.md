📄 README.md

Copy
Edit
# Java Program: Vowel Checker

## ✅ Description
This program checks whether a **hardcoded character** is a vowel or not.

---

## 🧮 Logic Used
- The character is stored in a variable: `char inputChar = 'a';`
- A boolean expression checks whether `inputChar` is any of the vowels (both lowercase and uppercase).
- The result (`true` or `false`) is printed.

---

## 🔤 Vowel Characters Considered
- Lowercase: `a, e, i, o, u`
- Uppercase: `A, E, I, O, U`

---

## 🧪 Sample Output

Is vowel: true

yaml
Copy
Edit

> If `inputChar = 'b'`, then output will be:  
> `Is vowel: false`

---

## 💡 Key Concepts
- **Primitive Data Types:** `char`, `boolean`
- **Logical Operators:** `||` (OR)
- **Hardcoded Input:** The input is set directly in the code, not from user input.

---

## ⚙️ How to Run
1. Save the file as `Main.java`
2. Compile the program:
   ```bash
   javac Main.java
Run the compiled class:

bash
Copy
Edit
java Main



```
// Program to check whether a given character is a vowel or not
public class Main {
    public static void main(String[] args) {
        // Hardcoded character input
        char inputChar = 'a';

        // Check if inputChar is a vowel (both lowercase and uppercase)
        boolean isVowel = (
            inputChar == 'a' || inputChar == 'e' || inputChar == 'i' ||
            inputChar == 'o' || inputChar == 'u' ||
            inputChar == 'A' || inputChar == 'E' || inputChar == 'I' ||
            inputChar == 'O' || inputChar == 'U'
        );

        // Print whether the character is a vowel
        System.out.println("Is vowel: " + isVowel);
    }
}
```
