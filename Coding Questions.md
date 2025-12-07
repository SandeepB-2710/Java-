# Coding Questions (Encapsulation)



---

## Program 1: Rectangle Area Calculator Program

**Problem Statement:**
Create a Rectangle class with private fields for length and width. Provide public methods to access and modify these fields, and calculate the area.

**Detailed Instructions:**
1. Create the Rectangle class with private fields:
   * length (double)
   * width (double)
2. Create public getter and setter methods for both fields.
3. In the setter methods, ensure that the length and width are not set to negative values. If a negative value is provided, set the field to 0.0.
4. Create a public method `calculateArea()` that returns the area of the rectangle.

**Demonstrate Encapsulation**

**Problem Statement:**
Create a Rectangle object and demonstrate the use of encapsulation by accessing and modifying its fields through public methods.

**Detailed Instructions:**
In the `main()` method:
1. Create a Rectangle object named `rect1`.
2. set the length to 5.0 and width 3.0.
3. Display the initial rectangle details and area.
4. Set the length to 7.0 and width to -2.0 (which should be set to 0.0 due to the validation in the setter).
5. Display the final rectangle details and area.

---

## Program 2: Student Information Management Program

**Problem Statement:**
Create a Student class with private fields for roll number, name, and age. Provide public methods to access and modify these fields.

**Detailed Instructions:**
1. Create the Student class with private fields:
   * rollNumber (int)
   * name (String)
   * age (int)
2. Create public getter methods for all fields.
3. Create public setter methods for name and age.
4. In the setter method for age, ensure that the age is not set to a negative value (using if-else block). For else part, display a message "Invalid age. Age must be positive."

**Demonstrate Encapsulation**

**Problem Statement:**
Create a Student object and demonstrate the use of encapsulation by accessing and modifying its fields through public methods.

**Detailed Instructions:**
In the `main()` method:
1. Create a Student object named `student1`
2. Set the values using setter methods:
   * Roll number = 101
   * Name = "Alice"
   * Age = 20
3. Display the initial student details.
4. Change the student's name to "Alicia".
5. Try to set an invalid age (-5) for the student.
6. Set a valid age (21) for the student.
7. Display the final student details.

---

## Program 3: Temperature Converter

**Problem Statement:**
Create a Temperature class with a private field for temperature in Celsius. Provide public methods to set the temperature in Celsius and get it in both Celsius and Fahrenheit.

**Detailed Instructions:**
1. Create the Temperature class with a private field:
   * celsius (double)
2. Create public getter and setter methods for the Celsius temperature.
3. Create a public method `getFahrenheit()` that returns the temperature in Fahrenheit `(celsius * 9/5) + 32`.

**Demonstrate Encapsulation**

**Problem Statement:**
Create a Temperature object and demonstrate the use of encapsulation by accessing and modifying its temperature through public methods.

**Detailed Instructions:**
In the `main()` method:
1. Create a Temperature object named `temp1`
2. Set the temperature to 25.0 degrees Celsius.
3. Display the initial temperature in both Celsius and Fahrenheit.
4. Set the temperature to 30.0 degrees Celsius.
5. Display the final temperature in both Celsius and Fahrenheit.
