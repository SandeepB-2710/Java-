# Java Exception Handling: Multiple Choice Questions  

## 1. What is the primary purpose of Exception Handling in programming?
A) To terminate the program when an error occurs.

B) To notify the user about errors.

C) To handle runtime errors and maintain the normal flow of the program.

D) To compile the program successfully.

## 2. What constitutes an exception in Java?
A) An error that occurs at compile time.

B) A runtime issue that disrupts the normal flow of the program.

C) A warning message during code compilation.

D) A syntax error in the source code.

## 3. Why and when do exceptions occur in Java?
A) When the program is syntactically incorrect.

B) When the program tries to access valid resources.

C) When unexpected events occur during runtime, disrupting the normal flow.

D) When the Java compiler encounters an unknown keyword.

## 4. Which of the following is a common scenario that can lead to exceptions in Java?
A) Trying to declare variables without a data type.

B) Accessing an invalid array index.

C) Writing a program with improper indentation.

D) Declaring multiple classes in a single Java file.

## 5. One common reason for an exception to occur is when a program attempts to access an element in an array using an index that is out of bounds. This leads to which specific exception?
A) NullPointerException 

B) FileNotFoundException 

C) ArrayIndexOutOfBoundsException 

D) IndexOutOfRangeException 


## 6. When reading from a file, if the file does not exist or cannot be found at the specified path, the program will throw a:

A) FileNotFoundException 

B) IOException 

C) NullPointerException 

D) ResourceNotFoundException 


## 7. If no catch block is found to handle an exception, the JVM's default exception handler prints the __________, which shows the sequence of method calls that led to the error.

A) Error log 

B) Exception report 

C) Call graph 

D) Stack trace 





### Answer Key: Java Exception Handling



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


### Detailed Explanations


Question 1: [C] The primary goal is to handle runtime errors so that the normal flow of the application continues instead of crashing.

Question 2: [B] An exception is a runtime issue; it differs from compile-time errors which prevent the code from running at all.

Question 3: [C] Exceptions are triggered by unexpected events during execution, such as invalid user input or resource unavailability.

Question 4: [B] Accessing an invalid array index is a logical runtime error, whereas the other options are syntax errors caught by the compiler.

Question 5: [C] The specific Java class for array errors is ArrayIndexOutOfBoundsException.

Question 6: [A] A FileNotFoundException is specifically thrown when a file stream cannot locate the file on the disk.

Question 7: [D] A Stack trace provides a snapshot of the call stack, showing exactly where the error originated.



