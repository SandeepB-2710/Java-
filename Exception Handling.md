# Java Exception Handling: Multiple Choice Questions  

## 1. What is the primary purpose of Exception Handling in programming?
A) To terminate the program when an error occurs.

B) To notify the user about errors.

C) To handle runtime errors and maintain the normal flow of the program.

D) To compile the program successfully.

<br>

## 2. What constitutes an exception in Java?
A) An error that occurs at compile time.

B) A runtime issue that disrupts the normal flow of the program.

C) A warning message during code compilation.

D) A syntax error in the source code.

<br>

## 3. Why and when do exceptions occur in Java?
A) When the program is syntactically incorrect.

B) When the program tries to access valid resources.

C) When unexpected events occur during runtime, disrupting the normal flow.

D) When the Java compiler encounters an unknown keyword.

<br>

## 4. Which of the following is a common scenario that can lead to exceptions in Java?
A) Trying to declare variables without a data type.

B) Accessing an invalid array index.

C) Writing a program with improper indentation.

D) Declaring multiple classes in a single Java file.

<br>

## 5. One common reason for an exception to occur is when a program attempts to access an element in an array using an index that is out of bounds. This leads to which specific exception?
A) NullPointerException 

B) FileNotFoundException 

C) ArrayIndexOutOfBoundsException 

D) IndexOutOfRangeException 

<br>


## 6. When reading from a file, if the file does not exist or cannot be found at the specified path, the program will throw a:

A) FileNotFoundException 

B) IOException 

C) NullPointerException 

D) ResourceNotFoundException 

<br>


## 7. If no catch block is found to handle an exception, the JVM's default exception handler prints the __________, which shows the sequence of method calls that led to the error.

A) Error log 

B) Exception report 

C) Call graph 

D) Stack trace 

<br>

## Answer Key: Java Exception Handling

| Question Number | Correct Option | Key Technical Term |
| :--- | :--- | :--- |
| **Question 1** | **C** | **Normal Flow** |
| **Question 2** | **B** | **Runtime Issue** |
| **Question 3** | **C** | **Unexpected Events** |
| **Question 4** | **B** | **Invalid Index** |
| **Question 5** | **C** | **ArrayIndexOutOfBoundsException** |
| **Question 6** | **A** | **FileNotFoundException** |
| **Question 7** | **D** | **Stack Trace** |



### Answer Key: Java Exception Handling


<br>


## Detailed Explanations


<br>


## Question 1: 

[C] The primary goal is to handle runtime errors so that the normal flow of the application continues instead of crashing.
<br>
### Question 2: 

[B] An exception is a runtime issue; it differs from compile-time errors which prevent the code from running at all.
<br>
### Question 3: 

[C] Exceptions are triggered by unexpected events during execution, such as invalid user input or resource unavailability.
<br>
### Question 4: 

[B] Accessing an invalid array index is a logical runtime error, whereas the other options are syntax errors caught by the compiler.
<br>
### Question 5: 

[C] The specific Java class for array errors is ArrayIndexOutOfBoundsException.
<br>
### Question 6: 

[A] A FileNotFoundException is specifically thrown when a file stream cannot locate the file on the disk.
<br>
### Question 7: 

[D] A Stack trace provides a snapshot of the call stack, showing exactly where the error originated.



<br>
<br>
<br>



# Java Exceptions: Throw & Throws.

---

##  Key Points to Remember

* **Rethrowing** means a method chooses not to handle the error and instead passes it to another method that can.
* Use **`throw`** to manually create and send an exception when a serious problem is found.
* Use **`throws`** in the method declaration to warn others that an exception might be thrown.
* If you use **`throw`** inside a method, you must either:
    1.  **Catch** the exception using a `try-catch` block, or
    2.  Use **`throws`** to pass the responsibility to the caller.
* A method can only **throw one exception at a time**, and it must be an object of a class that extends `Throwable`.
* When you use **`throws`**, the caller must be ready to handle the exception using `try-catch`.
* **Rethrowing** helps organize your code, making sure problems are handled in the right place.

---

## Real-Life Analogies

### 1. Group Study Doubt
You're asked a tough question in a group study. You try but can't answer it, so you **pass it to your senior**. That's **rethrowing**—you detected the problem but passed it up.

### 2. Fragile Parcel
When you pack a glass item, you don't make it unbreakable, but you **warn the receiver** with a label: *"Handle with care - fragile."* That's exactly what **`throws`** does—it doesn't fix, but warns.

### 3. Fire Alarm System
If there's smoke in a room, a sensor detects it and **triggers the alarm system** instead of trying to stop the fire. That's **`throw`**—detecting the issue and sending it out to someone who can take proper action.

---

## Questions & Answers

**1. What is the difference between `throw` and `throws` in Java?**
> **Answer:** `throw` is used **inside** a method to actually throw an exception. `throws` is used in the **method declaration** to indicate that a method might throw an exception.

**2. Can a method use both `throw` and `throws`?**
> **Answer:** **Yes!** A method can declare that it might throw an exception using `throws` and actually throw one using `throw` inside the method body.

**3. Why should we use `throws`?**
> **Answer:** When you don't want to handle the exception inside the method but want the caller to take responsibility, you use `throws` to warn them.

**4. What happens if you throw an exception and don't handle or declare it?**
> **Answer:** The program will **not compile** (for checked exceptions) or **crash at runtime** (for unchecked exceptions) if no one catches it.

**5. Can we throw multiple exceptions using one `throw` statement?**
> **Answer:** **No.** You can only throw one exception at a time. However, you can declare **multiple exceptions** using `throws` in the method declaration.

---

## Quick Comparison: `throw` vs. `throws`

| Feature | `throw` | `throws` |
| :--- | :--- | :--- |
| **Purpose** | Used to explicitly throw an exception. | Used to declare that a method may throw exceptions. |
| **Location** | Used **inside** the method body. | Used in the **method signature** (declaration). |
| **Syntax** | Followed by an **instance** (e.g., `new Exception()`). | Followed by exception **class names** (e.g., `IOException`). |
| **Quantity** | Can throw only **one** exception at a time. | Can declare **multiple** exceptions separated by commas. |
| **Internal Logic** | Acts like a "jump" statement to transfer control. | Acts like a "warning" to the caller of the method. |

---

## How the Flow Works



To help you visualize how these keywords interact in your code, remember this flow:

1.  **The Method (`throws`):** The method signature shouts, *"Heads up! I might have a problem with IOException."*
2.  **The Condition (`throw`):** Inside the code, an `if` statement checks for a problem. If the problem is true, it executes `throw new IOException();`.
3.  **The Caller (`try-catch`):** The method that called the first one must now either catch that exception or declare its own `throws` to pass it even further up the chain.

---

## Conclusion

In real life, we don't always solve every problem ourselves—sometimes, we ask for help. In Java, rethrowing exceptions works in the same way. When a method faces a problem and cannot fix it, it uses `throw` to send the error, and `throws` to warn that the error might occur. This helps keep your program neat, clear, and well-structured.

Instead of each method handling every problem, exceptions can be passed to a place where they are better understood and can be properly resolved. This way, your code becomes more professional and easier to manage. So remember, just like asking for help in real life, rethrowing in Java is a smart way to make sure problems are handled correctly—not ignored or hidden. Keep practicing, and you'll master it in no time!









