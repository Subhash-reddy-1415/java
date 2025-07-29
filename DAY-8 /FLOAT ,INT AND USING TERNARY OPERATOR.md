📄 README.md

Copy
Edit
# Athlete Race Comparator

## 📌 Description
This Java program compares the performance of two athletes based on:
- Their weights (in kg)
- Their completion time in a race (in seconds)

The winner is decided by comparing the race times using the **ternary operator**.

---

## 🔧 Concepts Demonstrated
- Use of primitive data types:
  - `float` for weight (precision to 2 decimal places)
  - `double` for time (higher precision)
- String concatenation using `System.out.println()`
- Ternary operator (`?:`) for decision making

---

## 🧪 Output Example

Weight of Athlete 1: 68.45 kg
Weight of Athlete 2: 70.55 kg
Time taken by Athlete 1: 9.8576341234 seconds
Time taken by Athlete 2: 10.0012345678 seconds
Winner of the race: Athlete 1

yaml
Copy
Edit

---

## 🚀 How to Run

1. Save the file as `Main.java`
2. Compile it:
   ```bash
   javac Main.java
Run it:

bash
Copy
Edit
java Main


```
// Class declaration
public class Main {
    public static void main(String[] args) {
        // Declaring and initializing weights of two athletes
        float athlete1Weight = 68.45f;
        float athlete2Weight = 70.55f;

        // Displaying weights
        System.out.println("Weight of Athlete 1: " + athlete1Weight + " kg");
        System.out.println("Weight of Athlete 2: " + athlete2Weight + " kg");

        // Declaring and initializing time taken by athletes to complete the race
        double athlete1Time = 9.8576341234;
        double athlete2Time = 10.0012345678;

        // Displaying time taken
        System.out.println("Time taken by Athlete 1: " + athlete1Time + " seconds");
        System.out.println("Time taken by Athlete 2: " + athlete2Time + " seconds");

        // Using ternary operator to determine the winner (shorter time wins)
        String winner = athlete1Time < athlete2Time ? "Athlete 1" : "Athlete 2";

        // Displaying the winner
        System.out.println("Winner of the race: " + winner);
    }
}
```
