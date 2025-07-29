📄 README.md
markdown
Copy
Edit
# NetflixOperations - Java Simulation Program

## 📌 Overview
This Java program simulates global operations data for Netflix. It prints key statistics like:
- Number of countries where Netflix is available
- Total unique titles on the platform
- Total subscriber count
- Total streaming minutes from the past year

The purpose is to practice Java's **primitive data types** and **output formatting** using `System.out.println()`.

---

## 🎯 Features
- Uses appropriate Java primitive types:
  - `byte` for small-range values (number of countries)
  - `short` for mid-range values (titles count)
  - `int` for large-range values (subscriber count)
  - `long` for very large values (streaming minutes)
- Demonstrates clean and formatted string output

---

## 🖥️ Output Example

Netflix is available in 110 countries.
Netflix offers 15000 unique titles worldwide.
Netflix has 200000000 subscribers globally.
Total streaming minutes on Netflix last year: 1000000000000 minutes.

yaml
Copy
Edit

---

## 🧪 How to Run

1. Save the code as `NetflixOperations.java`
2. Compile the file:
   ```bash
   javac NetflixOperations.java
Run the compiled program:

bash
Copy
Edit
java NetflixOperations

```
public class NetflixOperations {
    public static void main(String[] args) {
        // Number of countries where Netflix is available
        byte numberOfCountries = 110;
        System.out.println("Netflix is available in " + numberOfCountries + " countries.");

        // Total number of titles
        short availableTitles = 15000;
        System.out.println("Netflix offers " + availableTitles + " unique titles worldwide.");

        // Number of global subscribers
        int totalSubscribers = 200000000;
        System.out.println("Netflix has " + totalSubscribers + " subscribers globally.");

        // Annual streaming minutes
        long streamingMinutes = 1000000000000L;
        System.out.println("Total streaming minutes on Netflix last year: " + streamingMinutes + " minutes.");
    }
}
```
