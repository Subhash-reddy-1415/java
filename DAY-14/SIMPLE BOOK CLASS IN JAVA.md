📄 README.md
markdown
Copy
Edit
# 📚 Simple Book Class in Java

This Java program defines a simple class called `Book` with a method named `read()`. When invoked, this method prints a message to indicate that the book is currently being read.

## ✅ Objective

- Understand basic object-oriented programming in Java.
- Learn how to define a class, create an object, and invoke its method.

---

## 🧾 Class Structure

### 🔸 `Book` Class
- **Instance Variable:** `String name`
- **Method:** `void read()`
  - Prints the message: `"Book is being read."`

### 🔸 `Main` Class
- Creates an object of class `Book`.
- Sets the `name` of the book.
- Calls the `read()` method.

---

## 💻 Code

```java
class Book {
    String name;

    void read() {
        System.out.println(name + " is being read.");
    }
}

public class Main {
    public static void main(String[] args) {
        Book b1 = new Book();
        b1.name = "Book";
        b1.read(); // Output: Book is being read.
    }
}
🖥️ Sample Output
pgsql
Copy
Edit
Book is being read.
📝 Explanation
Class Definition:
The Book class has a string field name and a method read() that prints a message using the name.

Method read()

It is a void method.

When called, it prints a message that the book is being read.

Creating Objects:

In the main method, an object b1 is created.

b1.name is set to "Book".

Then b1.read() is called to display the message.

🛠️ Requirements
Java 8 or later

Any Java IDE or terminal with JDK installed

📌 How to Run
Save the file as Main.java.

Compile: javac Main.java

Run: java Main

📚 Topics Covered
Class and Object

Instance Variables

Method Definition and Invocation

yaml


// Book.java
public class Book {
    String name;

    // Method to simulate reading the book
    void read() {
        System.out.println(name + " is being read.");
    }
}
// Main.java
public class Main {
    public static void main(String[] args) {
        // Create an object of Book
        Book myBook = new Book();
        
        // Set the book's name
        myBook.name = "Java Programming";

        // Call the read method
        myBook.read(); // Output: Java Programming is being read.
    }
}


