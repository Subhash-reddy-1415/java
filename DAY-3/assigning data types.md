# Java Data Types Example

This project demonstrates the use of **basic data types** in Java by assigning values and printing them using the `System.out.println()` method.

## 📌 Description

The `Main` class contains the `main` method which is the entry point of the program. Inside it, different data types are assigned and printed:

### ✅ Data Types Used:
| Data Type | Variable  | Example Value | Description                     |
|-----------|-----------|----------------|---------------------------------|
| `int`     | `a`       | `10`           | Stores integer values           |
| `String`  | `name`    | `"SUBHASH"`    | Stores text (sequence of chars) |
| `float`   | `b`       | `2.1233f`      | Stores decimal numbers (single precision) |
| `double`  | `price`   | `19.90`        | Stores decimal numbers (double precision) |
| `boolean` | `isActive`| `true`         | Stores true/false values        |
| `char`    | `grade`   | `'A'`          | Stores a single character       |

## ▶️ Output

When you run this code, the output will be:

```
public class Main {
    public static void main(String[] args) {
        // Integer data type
        int a = 10;

        // String data type
        String name = "SUBHASH";

        // Float data type (note the 'f' suffix)
        float b = 2.1233f;

        // Double data type
        double price = 19.90;

        // Boolean data type
        boolean isActive = true;

        // Character data type
        char grade = 'A';

        // Printing the values
        System.out.println("Integer value: " + a);
        System.out.println("String value: " + name);
        System.out.println("Float value: " + b);
        System.out.println("Double value: " + price);
        System.out.println("Boolean value: " + isActive);
        System.out.println("Char value: " + grade);
    }
}
