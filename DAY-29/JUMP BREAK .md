# Jump Statements - Break (Java)

## 📌 Description
This program simulates searching for an item in a warehouse.  
The warehouse has items labeled from `1` to `10`.  
We search for the item labeled `6`, and once it is found, the program **stops the search** using a `break` statement.

---

## ⚙️ How It Works
1. Use a **for loop** to iterate from `1` to `10`.
2. Inside the loop:
   - If the current item is equal to `6`:
     - Print `"Item 6 found, stopping the search."`
     - Use `break` to exit the loop immediately.
   - Otherwise, print `"Checking item X"`.
3. Program ends after breaking the loop.

---

## 🧮 Example Output
Checking item 1
Checking item 2
Checking item 3
Checking item 4
Checking item 5
Item 6 found, stopping the search.

yaml
Copy
Edit

---

## 🚀 How to Run
1. Save the program in a file named `Main.java`.
2. Compile:
javac Main.java

markdown
Copy
Edit
3. Run:
```
public class Main {
    public static void main(String[] args) {
        // Loop through items from 1 to 10
        for (int item = 1; item <= 10; item++) {
            
            // Check if the item is 6
            if (item == 6) {
                System.out.println("Item " + item + " found, stopping the search.");
                break; // exit the loop when item 6 is found
            }

            // Print checking message for other items
            System.out.println("Checking item " + item);
        }
    }
}
```
