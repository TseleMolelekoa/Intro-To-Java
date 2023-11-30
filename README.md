# Intro-To-Java
# WEEK 1 
# Day 1


What is java? 

Java is a general-purpose programming language that is class-based, object-oriented, and designed to have as few implementation dependencies as possible. It is intended to let application developers write once, run anywhere (WORA), meaning that compiled Java code can run on all platforms that support Java without the need for recompilation. JAVA was developed by Sun Microsystems Inc and first released in 1991, later acquired by Oracle Corporation. 

 

 

Java Components 

Java Virtual Machine (JVM) 

Generally referred as JVM, it’s the primary function is to execute the bytecode produced by compiler. 

Java Development Kit (JDK) 

This is a complete java development kit that includes JRE (Java Runtime Environment), compilers and various tools like JavaDoc, Java debugger etc. 

Java Runtime Environment (JRE) 

JRE allows you to run java programs, it includes JVM, browser plugins and applets support. When you only need to run a java program on your computer, you would only need JRE. 

 

Main Java features 

Platform Independence: 

Java is designed to be platform-independent, meaning that Java programs can run on any device with a compatible Java Virtual Machine (JVM). 

Object-Oriented Programming (OOP): 

Java is a fully object-oriented programming language, emphasizing concepts such as encapsulation, inheritance, and polymorphism. 

Simple and Easy to Learn: 

Java was designed to be straightforward and easy to learn for programmers. It eliminates complex features such as pointers, operator overloading, and multiple inheritance, making it more accessible for developers. 

Robust and Secure: 

Java incorporates features like strong memory management, exception handling, and a comprehensive set of APIs, which contribute to the robustness and reliability of Java applications. 

Multithreading: 

Java supports multithreading, allowing concurrent execution of multiple threads within a program. 

 

Install Java Development Kit (JDK): 

Visit the Oracle JDK download page or OpenJDK to download and install the latest version of the Java Development Kit (JDK). Follow the installation instructions for your operating system. 

 

Set the JAVA_HOME environment variable: 

On Windows: Right-click on "This PC" or "Computer," select "Properties," click on "Advanced system settings," go to the "Advanced" tab, and click "Environment Variables." Add a new system variable with the name JAVA_HOME and the path to your JDK installation (e.g., C:\Program Files\Java\jdk1.8.0_291). 

Typical Structure of a Java program 

A typical structure of a Java program contains the following elements: 

Package declaration 

Import statements 

Comments 

Class definition 

Attributes 

Methods/Behaviours 

 



# Day 2

DAY 2 

 

What is a variable? 

A variable is a name given to a memory location. It is the basic unit of storage in a program. 

The value stored in a variable can be changed during program execution. 

A variable is only a name given to a memory location; all the operations done on the variable effects that memory location. 

In Java, all the variables must be declared before use. 

How to declare variables? 

type: Type of data that can be stored in this variable. 

name: Name given to the variable. 

It can be assigned values in two ways: 

Variable Initialization 

Assigning value by taking input. 

 

Declaring and initialize variables: 

datatype: Type of data that can be stored in this variable. 

variable_name: Name given to the variable. 

value: It is the initial value stored in the variable. 

Declaring variables examples 

float simpleInterest; - Declaring float variable 

int myAge = 19; - Declaring and Initializing integer variable 

char firstLetter = 'h'; - Declaring and Initializing character variable 

 

 

There are three types of variables in Java: 

 

Local Variables: A variable defined within a block or method or constructor is called local variable. 

Instance Variables: Instance variables are non-static variables and are declared in a class outside any method, constructor or block. 

Static Variables: Static variables are also known as Class variables. 

## Data types in Java: 

1) Primitive data types - A primitive data type specifies the size and type of variable values, and it has no additional methods. 

2)  Non-primitive data types – Arrays and Strings are non-primitive data types, these are the datatypes which have instances like objects. Hence, they are called reference variables. They are primarily classes, arrays, strings or interfaces. 



There are eight primitive data types in Java: 

Byte 

Short 

Int 

Long 

Float 

Double 

Boolean 

 a variable is a named storage location in the computer's memory that holds data that can be manipulated or changed during the execution of a program.  

Variables are used to store information such as numbers, text, or objects that the program needs to work with. 

  

Variables in Java have several characteristics: 

  

1. **Name:** A variable is identified by a name, which is used to refer to it within the program. Variable names must follow specific rules such as starting with a letter, underscore (_), or dollar sign ($) and can contain letters, digits, underscores, and dollar signs. 

  

2. **Data Type:** Every variable in Java has a data type that specifies the kind of data it can hold. Examples of data types include `int` (for integers), `double` (for floating-point numbers), `boolean` (for true/false values), `String` (for text), and many others. Java is a statically typed language, meaning the data type of a variable must be declared before the variable can be used. 

  

3. **Memory Location:** Variables reserve space in the computer's memory to store their values. The size of the memory allocated depends on the data type of the variable. 

  

4. **Value:** A variable can store and hold a value of its declared data type. The value can be changed during the execution of the program. 

  

Here are some examples of variable declarations in Java: 

  

```java 

int age; // Declaration of an integer variable named 'age' 

double temperature; // Declaration of a double variable named 'temperature' 

boolean isStudent; // Declaration of a boolean variable named 'isStudent' 

String name; // Declaration of a String variable named 'name' 

``` 

  

Variables can be assigned initial values upon declaration or later in the program: 

  

```java 

int numberOfStudents = 20; // Declaration and initialization of an integer variable 

temperature = 98.6; // Assigning a value to the 'temperature' variable 

name = "John Doe"; // Assigning a value to the 'name' variable 

``` 

  

It's important to note that variables in Java have a specific scope, which defines where in the program they can be accessed and used. The scope of a variable is typically within the block of code where it is declared. 

 

## Data type  
Defines the value that a variable can take,  

## There's two categories of data types. 

 

### Primitive data type  

A primitive data type specifies the size and type of variable values, and it has no additional methods. 

 

### We have 8 primitive data types in java. 

Data Type 

Size 

Description 

byte 

1 byte 

Stores whole numbers from -128 to 127 

short 

2 bytes 

Stores whole numbers from -32,768 to 32,767 

int 

4 bytes 

Stores whole numbers from -2,147,483,648 to 2,147,483,647 

long 

8 bytes 

Stores whole numbers from -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 

float 

4 bytes 

Stores fractional numbers. Sufficient for storing 6 to 7 decimal digits 

double 

8 bytes 

Stores fractional numbers. Sufficient for storing 15 decimal digits 

boolean 

1 bit 

Stores true or false values 

char 

2 bytes 

Stores a single character/letter or ASCII values 


### Non-primitive data type  

These are the datatypes which have instances like objects. Hence, they are called reference variables. They are primarily classes, arrays, strings or interfaces. 

They are 

String  

Array  



## Operator's in java 

An operator is a character that represents an action. 

 

Java operators can be classified into: 

Arithmetic Operators 

Relational Operators 

Bitwise Operators 

Logical Operators 

Assignment Operators 

Misc Operators 

 

Arithmetic operators  

 

Arithmetic operators are used in mathematical expressions in the same way that they are used in algebra.  

The following table lists the arithmetic operators −Assume integer variable A holds 10 and variable B holds 20, then 

 

Operator 

Description 

Example 

+ (Addition) 

Adds values on either side of the operator. 

A + B will give 30 

- (Subtraction) 

Subtracts right-hand operand from left-hand operand. 

A - B will give -10 

* (Multiplication) 

Multiplies values on either side of the operator. 

A * B will give 200 

/ (Division) 

Divides left-hand operand by right-hand operand. 

B / A will give 2 

% (Modulus) 

Divides left-hand operand by right-hand operand and returns remainder. 

B % A will give 0 

++ (Increment) 

Increases the value of operand by 1. 

B++ gives 21 

-- (Decrement) 

Decreases the value of operand by 1. 

B-- gives 19 

Relational operators – the table below show the relational operators supported by java. 


Operator 

Description 

Example 

== (equal to) 

Checks if the values of two operands are equal or not, if yes then condition becomes true. 

(A == B) is not true. 

!= (not equal to) 

Checks if the values of two operands are equal or not, if values are not equal then condition becomes true. 

(A != B) is true. 

> (greater than) 

Checks if the value of left operand is greater than the value of right operand, if yes then condition becomes true. 

(A > B) is not true. 

< (less than) 

Checks if the value of left operand is less than the value of right operand, if yes then condition becomes true. 

(A < B) is true. 

>= (greater than or equal to) 

Checks if the value of left operand is greater than or equal to the value of right operand, if yes then condition becomes true. 

(A >= B) is not true. 

<= (less than or equal to) 

Checks if the value of left operand is less than or equal to the value of right operand, if yes then condition becomes true. 

(A <= B) is true. 

Bitwise operators – works on bits and performs bit-by-bit operation, assume if a = 60 and b = 13; now in binary format they will be as follows: 

a = 0011 1100 

b = 0000 1101 

a&b = 0000 1100 

a|b = 0011 1101 

a^b = 0011 0001 

~a = 1100 0011 

  

Operator 

Description 

Example 

& (bitwise and) 

Binary AND Operator copies a bit to the result if it exists in both operands. 

(A & B) will give 12 which is 0000 1100 

| (bitwise or) 

Binary OR Operator copies a bit if it exists in either operand. 

(A | B) will give 61 which is 0011 1101 

^ (bitwise XOR) 

Binary XOR Operator copies the bit if it is set in one operand but not both. 

(A ^ B) will give 49 which is 0011 0001 

~ (bitwise compliment) 

Binary Ones Complement Operator is unary and has the effect of 'flipping' bits. 

(~A) will give -61 which is 1100 0011 in 2's complement form due to a signed binary number. 

<< (left shift) 

Binary Left Shift Operator. The left operands value is moved left by the number of bits specified by the right operand. 

A << 2 will give 240 which is 1111 0000 

>> (right shift) 

Binary Right Shift Operator. The left operands value is moved right by the number of bits specified by the right operand. 

A >> 2 will give 15 which is 1111 

>>> (zero fill right shift) 

Shift right zero fill operator. The left operands value is moved right by the number of bits specified by the right operand and shifted values are filled up with zeros. 

A >>>2 will give 15 which is 0000 1111 

Logical operators - The following table lists the logical operators −Assume Boolean variables A holds true and variable B holds false, then: 

  

Operator 

Description 

Example 

&& (logical and) 

Called Logical AND operator. If both the operands are non-zero, then the condition becomes true. 

(A && B) is false 

|| (logical or) 

Called Logical OR Operator. If any of the two operands are non-zero, then the condition becomes true. 

(A || B) is true 

! (logical not) 

Called Logical NOT Operator. Use to reverses the logical state of its operand. If a condition is true then Logical NOT operator will make false. 

!(A && B) is true 



The Assignment Operator 

Following are the assignment operator supported by Java language − 

  

Operator 

Description 

Example 

= 

Simple assignment operator. Assigns values from right side operands to left side operand. 

C = A + B will assign value of A + B into C 

 

Java Classes and Objects 

 

A Class is like an object constructor, or a "blueprint” or a factory for creating objects. 

This means without a class no object can be created. 

What is a class in java 

A class can be defined as a template/blueprint that describes the behavior/state that the object of its type support. 

 

Creating a class  

To create a class, use the keyword class 

 

A class is made up of below 

Constructor - is a method called when creating an object from a class 

If we do not explicitly write a constructor for a class, the Java compiler builds a default constructor for that class.  

Some constructors may accept parameter, and some may not. 

 

 

 

Methods 

A class can have any number of methods to access the value of various kinds of methods.  

 

in the example given below run,  

walk and sleep are methods 

Variables/Properties 

Usually these are attributes the describe objects that a created from that class. In the below example name, age and height are variables 

Example of class: 

public class Car { 

    // Attributes or Fields 

    private String brand; 

    private String model; 

    private int year; 

    private double price; 

  

    // Constructor 

    public Car(String brand, String model, int year, double price) { 

        this.brand = brand; 

        this.model = model; 

        this.year = year; 

        this.price = price; 

    } 

  

    // Getters and Setters for the attributes 

    public String getBrand() { 

        return brand; 

    } 

  

    public void setBrand(String brand) { 

        this.brand = brand; 

    } 

  

    public String getModel() { 

        return model; 

    } 

  

    public void setModel(String model) { 

        this.model = model; 

    } 

  

    public int getYear() { 

        return year; 

    } 

  

    public void setYear(int year) { 

        this.year = year; 

    } 

  

    public double getPrice() { 

        return price; 

    } 

  

    public void setPrice(double price) { 

        this.price = price; 

    } 

  

    // Method to display car information 

    public void displayCarInfo() { 

        System.out.println("Car: " + brand + " " + model + " (" + year + ")"); 

        System.out.println("Price: $" + price); 

    } 

  

    // Main method to demonstrate the usage of the Car class 

    public static void main(String[] args) { 

        // Creating an instance of Car class 

        Car myCar = new Car("Toyota", "Camry", 2022, 25000.50); 

  

        // Using setter method to change the price 

        myCar.setPrice(27000.75); 

  

        // Displaying car information using displayCarInfo() method 

        myCar.displayCarInfo(); 

    } 

} 

 

 

 # Day 3 

## OOP  

Certainly! Here's a rewritten version of the information about OOP, its advantages, core features, other features, and example Java classes: 

  

### What is OOP? 

  

Object-Oriented Programming (OOP) is a programming paradigm centered around the concept of "objects." Java, a widely used language, embodies OOP principles. 

  

### Key Concepts in Java OOP: 

  

1. **Class:** 

   - Blueprint or template defining attributes (fields) and behaviors (methods) of objects. 

  

2. **Object:** 

   - Instance of a class representing a specific entity in the program. 

  

3. **Method:** 

   - Function defined within a class representing object behaviors. 

  

4. **Instance Variable:** 

   - Variable defined in a class representing an object's state or properties. 

  

5. **Constructor:** 

   - Special method initializing objects upon creation, sharing the class's name. 

  

### Advantages of OOP: 

  

1. **Modularity and Reusability:** Encapsulation organizes code into self-contained modules for easy reuse. 

   

2. **Code Reusability:** Inheritance permits new classes to inherit properties and behaviors, reducing redundancy. 

   

3. **Abstraction:** Focuses on essential object properties, hiding unnecessary details. 

   

4. **Encapsulation:** Restricts access to certain components, minimizing complexity and improving maintainability. 

   

5. **Flexibility and Extensibility:** Polymorphism allows treating different objects as the same type, promoting generic code. 

   

6. **Modeling Real-World Concepts:** Aligns closely with real-world entities and relationships for effective modeling. 

   

7. **Collaborative Development:** Encourages well-defined interfaces, facilitating teamwork on different system parts. 

   

8. **GUI Development:** Suited for creating graphical user interfaces by representing visual elements as objects. 

  

### Core Features of OOP: 

  

1. **Encapsulation:** Bundles data and methods into a class. 

   

2. **Polymorphism:** Allows treating different types as a common type. 

   

3. **Inheritance:** Enables a class to inherit properties and behaviors from another class. 

   

4. **Abstraction:** Simplifies complex systems by focusing on essential object aspects. 

  

### Other Features Related to OOP: 

  

1. **Coupling:** Measures dependence between classes or modules. 

   

2. **Cohesion:** Measures relationships within modules. 

   

3. **Association:** Represents bidirectional relationships between classes. 

   

4. **Aggregation:** "Whole-part" relationship, allowing parts to exist independently. 

   

5. **Composition:** Stronger form of aggregation where parts cannot exist independently. 

  

### Activity 3: Example Java Classes: 

  

```java 

// PurchaseItem Class 

public class PurchaseItem { 

    private String name; 

    private double unitPrice; 

  

    public PurchaseItem(String name, double unitPrice) { 

        this.name = name; 

        this.unitPrice = unitPrice; 

    } 

  

    public double getPrice() { 

        return unitPrice; 

    } 

} 

  

// WeighedItem Class (Subclass of PurchaseItem) 

public class WeighedItem extends PurchaseItem { 

    private double weight; 

  

    public WeighedItem(String name, double unitPrice, double weight) { 

        super(name, unitPrice); 

        this.weight = weight; 

    } 

  

    @Override 

    public double getPrice() { 

        return super.getPrice() * weight; 

    } 

} 

  

// CountedItem Class (Subclass of PurchaseItem) 

public class CountedItem extends PurchaseItem { 

    private int quantity; 

  

    public CountedItem(String name, double unitPrice, int quantity) { 

        super(name, unitPrice); 

        this.quantity = quantity; 

    } 

  

    @Override 

    public double getPrice() { 

        return super.getPrice() * quantity; 

    } 

} 

  

// Usage example 

public class Main { 

    public static void main(String[] args) { 

        WeighedItem banana = new WeighedItem("Banana", 3.00, 1.37); 

        System.out.println(banana.getName() + " @ " + banana.getPrice()); 

  

        CountedItem pens = new CountedItem("Pens", 4.5, 10); 

        System.out.println(pens.getName() + " @ " + pens.getPrice()); 

    } 

} 

``` 

  

These classes demonstrate inheritance and overridden methods to calculate prices for weighed and counted items. 

  

### Additional OOP Concepts: 

  

1. **Coupling:** Degree of dependence between classes or modules. 

   

2. **Cohesion:** Level of relatedness within modules. 

   

3. **Association:** Bidirectional relationship between classes. 

   

4. **Aggregation:** "Whole-part" relationship allowing independent existence. 

   

5. **Composition:** Stronger "whole-part" relationship with dependent existence. 

 

Object-Oriented Programming (OOP) gained popularity over declarative and procedural programming paradigms due to several advantages it offers: 

  

1. **Modularity and Reusability:** 

   - OOP promotes encapsulation, bundling data and functionalities into objects. This modularity enables easier code organization, maintenance, and reuse. Objects can be reused in different parts of the code or in entirely different projects, enhancing efficiency and reducing redundancy. 

  

2. **Code Reusability through Inheritance:** 

   - Inheritance in OOP allows creating new classes based on existing ones, inheriting their attributes and behaviors. This feature minimizes redundant code, promotes code reuse, and helps build hierarchies of related classes. 

  

3. **Abstraction for Simplification:** 

   - OOP emphasizes abstraction, focusing on essential properties and hiding complex implementation details. This approach simplifies the understanding of code and enhances manageability by representing real-world entities as objects with specific behaviors and attributes. 

  

4. **Encapsulation for Better Control:** 

   - Encapsulation restricts access to certain components of an object, allowing developers to control and protect data integrity. By hiding implementation details, encapsulation reduces complexity, improves maintainability, and minimizes unintended interference with the internal workings of a class. 

  

5. **Flexibility and Extensibility through Polymorphism:** 

   - Polymorphism allows objects of different types to be treated as objects of a common type, enabling the creation of generic and flexible code. This feature facilitates the handling of different types uniformly and enhances the adaptability of code to changing requirements. 

  

6. **Modeling Real-World Concepts:** 

   - OOP aligns closely with how we conceptualize real-world entities and relationships, making it easier to map real-world problems into code. The concepts of objects, classes, inheritance, and relationships between objects resemble the relationships between real-world entities, making the code more intuitive and easier to design. 

  

7. **Collaborative Development:** 

   - OOP encourages the creation of well-defined interfaces between different parts of a program. This facilitates teamwork, as different developers can work on distinct modules or classes independently, as long as they adhere to the specified interfaces. 

  

8. **Suitability for GUI Development:** 

   - OOP aligns well with graphical user interface (GUI) development principles. Objects representing visual elements and their interactions in the GUI can be modeled effectively using OOP concepts. 

  

While declarative and procedural programming paradigms have their strengths, the advantages offered by OOP, such as code organization, reusability, abstraction, flexibility, and modeling capabilities, have contributed significantly to its popularity and widespread adoption in software development. 

OOP Core Features 

 

Encapsulation is when object only exposes selected information 

Inheritance one class acquires the methods and properties of another. 

Polymorphism Entities can have more than one form. 

Abstraction hides complex details to reduce complexity. 

 

The core features of Object-Oriented Programming (OOP)  

 

1. **Encapsulation:** 

   - Encapsulation is the bundling of data (attributes) and methods (functions) that operate on the data into a single unit known as a class. It allows the internal workings of an object to be hidden from the outside, providing controlled access to the object's state and behaviors. Encapsulation helps in data protection and promotes the principle of information hiding. 

  

2. **Polymorphism:** 

   - Polymorphism refers to the ability of objects to take on multiple forms. In Java, polymorphism allows objects of different classes to be treated as objects of a common superclass through inheritance. There are two main types of polymorphism: 

     - **Compile-time Polymorphism (Method Overloading):** It involves having multiple methods in the same class with the same name but different parameters. 

     - **Runtime Polymorphism (Method Overriding):** It allows a subclass to provide a specific implementation of a method that is already defined in its superclass.  

  

3. **Inheritance:** 

   - Inheritance is a mechanism that allows a class (subclass or derived class) to inherit properties (attributes and methods) and behaviors from another class (superclass or base class). The subclass can extend or override the functionalities of its superclass. It promotes code reuse, hierarchy establishment, and the creation of a more specialized class from a more generalized one. 

  

4. **Abstraction:** 

   - Abstraction involves simplifying complex systems by modeling classes based on the essential properties and behaviors relevant to the problem. It allows programmers to focus on what an object does rather than how it achieves its functionality. Abstract classes and interfaces are used to achieve abstraction in Java. Abstraction enables the creation of generalized blueprints that can be extended for more specific implementations. 

  

These core features provide the foundation for designing and implementing object-oriented systems.  

They enable developers to create modular, reusable, and maintainable code by promoting concepts such as code organization, data protection, code reuse, and flexibility in handling various object interactions and hierarchies. 

 

Features of OOP – Other features 

 

Besides the core features of Object-Oriented Programming (OOP) such as encapsulation, polymorphism, inheritance, and abstraction, there are several other important concepts and principles related to OOP: 

  

1. **Coupling:** 

   - **Definition:** Coupling measures the degree of dependence between classes or modules. It indicates how much one class knows about or relies on another. Low coupling is desirable as it leads to more maintainable and flexible systems. 

   - **Types:** 

     - **Low Coupling:** Classes have minimal knowledge of each other. Changes in one class have minimal impact on others. 

     - **High Coupling:** Classes are closely connected, and changes in one class may require changes in others. 

  

2. **Cohesion:** 

   - **Definition:** Cohesion measures the relatedness and interdependency of elements within a module (like a class or method). High cohesion is desirable as it leads to more maintainable and understandable code. 

   - **Types:** 

     - **High Cohesion:** Elements within a module are closely related and work together towards a common goal. 

     - **Low Cohesion:** Elements within a module have weak relationships and may not contribute to a common goal. 

  

3. **Association:** 

   - **Definition:** Association represents a bidirectional relationship between two classes. It can be a one-to-one, one-to-many, or many-to-many relationship. 

   - **Example:** In a university system, a `Student` class may be associated with a `Course` class through enrollment. 

  

4. **Aggregation:** 

   - **Definition:** Aggregation represents a "whole-part" relationship between classes. It implies that one class (the whole) contains another class (the part), but the part can exist independently. 

   - **Example:** In a car example, a `Car` class may have an aggregation relationship with a `Wheel` class. A `Car` has wheels, and wheels can exist independently. 

  

5. **Composition:** 

   - **Definition:** Composition is a stronger form of aggregation where the part cannot exist independently of the whole. If the whole is destroyed, all its parts are destroyed as well. 

   - **Example:** In a computer example, a `Computer` class may have a composition relationship with a `CPU` class. If the `Computer` is destroyed, the `CPU` is also destroyed. 

  

Understanding these additional concepts in OOP is crucial for designing systems with maintainability, flexibility, and clarity in mind. Properly managing coupling and cohesion helps create systems that are easier to modify and extend, while association, aggregation, and composition allow for more accurate modeling of real-world relationships in code. 

 

 

 

 

 

 

 

Day 4 

Introduction to Decision control 

 

Decision control in Java refers to the programming constructs that allow you to control the flow of execution based on certain conditions or decisions.  

 

There are mainly three decision-making structures in Java: 

  

1. if statement: 

   - The `if` statement evaluates a boolean expression and executes a block of code only if the condition is true. 

    

   Syntax: 

   ```java 

   if (condition) { 

       // Code to be executed if the condition is true 

   } 

   ``` 

  

2. **if-else statement:** 

   - The `if-else` statement allows the program to execute one block of code if the condition is true and another block if the condition is false. 

    

   Syntax: 

   ```java 

   if (condition) { 

       // Code to be executed if the condition is true 

   } else { 

       // Code to be executed if the condition is false 

   } 

   ``` 

  

3. **else-if ladder:** 

   - The `else-if` ladder allows checking multiple conditions one by one. If the condition is true, the corresponding block of code will be executed. If none of the conditions are true, the default else block (if present) will be executed. 

    

   Syntax: 

   ```java 

   if (condition1) { 

       // Code to be executed if condition1 is true 

   } else if (condition2) { 

       // Code to be executed if condition2 is true 

   } else if (condition3) { 

       // Code to be executed if condition3 is true 

   } else { 

       // Default code if no condition is true 

   } 

   ``` 

  

Example: 

  

```java 

int number = 10; 

  

// Example of if statement 

if (number > 0) { 

    System.out.println("Number is positive"); 

} 

  

// Example of if-else statement 

if (number > 0) { 

    System.out.println("Number is positive"); 

} else { 

    System.out.println("Number is not positive"); 

} 

  

// Example of else-if ladder 

if (number > 0) { 

    System.out.println("Number is positive"); 

} else if (number < 0) { 

    System.out.println("Number is negative"); 

} else { 

    System.out.println("Number is zero"); 

} 

``` 

  

These decision control structures help in writing programs that can make choices based on given conditions, allowing for dynamic behavior and more control over the flow of execution in Java programs. 

 

 

If Statement, IF ELSE statement, Nested If Statement 

 

 

 

`if` statement, `if-else` statement, and nested `if` statements in Java: 

  

### 1. If Statement: 

The `if` statement executes a block of code if the condition specified is true. 

  

Syntax: 

```java 

if (condition) { 

    // Code to execute if the condition is true 

} 

``` 

  

Example: 

```java 

int number = 10; 

  

// Example of if statement 

if (number > 0) { 

    System.out.println("Number is positive"); 

} 

``` 

  

### 2. If-Else Statement: 

The `if-else` statement executes one block of code if the condition is true and another block if the condition is false. 

  

Syntax: 

```java 

if (condition) { 

    // Code to execute if the condition is true 

} else { 

    // Code to execute if the condition is false 

} 

``` 

  

Example: 

```java 

int number = 10; 

  

// Example of if-else statement 

if (number > 0) { 

    System.out.println("Number is positive"); 

} else { 

    System.out.println("Number is not positive"); 

} 

``` 

  

### 3. Nested If Statement: 

Nested `if` statements contain an `if` statement within another `if` statement. This allows for more complex conditional logic. 

  

Syntax: 

```java 

if (condition1) { 

    // Code to execute if condition1 is true 

    if (condition2) { 

        // Code to execute if condition2 is true 

    } 

} 

``` 

  

Example: 

```java 

int x = 10; 

int y = 5; 

  

// Example of nested if statement 

if (x > 0) { 

    System.out.println("x is positive"); 

    if (y > 0) { 

        System.out.println("y is also positive"); 

    } 

} 

``` 

  

Nested `if` statements can have multiple levels, each level checking a specific condition.  

However, excessive nesting may lead to complex code and reduced readability, so it's essential to use them judiciously. 

 

Switch statement and the Tenary (?) operator 

 

 the `switch` statement and the ternary conditional operator (`? :`) in Java: 

  

### 1. Switch Statement: 

The `switch` statement is used to select one of many code blocks to be executed based on the value of a variable or expression. 

  

**Syntax:** 

```java 

switch (expression) { 

    case value1: 

        // Code to execute if expression equals value1 

        break; 

    case value2: 

        // Code to execute if expression equals value2 

        break; 

    // More cases... 

    default: 

        // Code to execute if expression doesn't match any case 

} 

``` 

  

**Example:** 

```java 

int day = 3; 

String dayName; 

  

// Example of switch statement to get the day name 

switch (day) { 

    case 1: 

        dayName = "Monday"; 

        break; 

    case 2: 

        dayName = "Tuesday"; 

        break; 

    case 3: 

        dayName = "Wednesday"; 

        break; 

    // More cases... 

    default: 

        dayName = "Invalid day"; 

} 

System.out.println("The day is: " + dayName); 

``` 

  

### 2. Ternary Operator (? :): 

The ternary operator `? :` is a concise way to express conditional statements. It evaluates a boolean expression and returns one of two values depending on the result of the evaluation. 

  

**Syntax:** 

```java 

result = (condition) ? valueIfTrue : valueIfFalse; 

``` 

  

**Example:** 

```java 

int x = 10; 

int y = 5; 

  

// Example of using the ternary operator 

String message = (x > y) ? "x is greater than y" : "y is greater than or equal to x"; 

System.out.println(message); 

``` 

  

The ternary operator evaluates the condition `(x > y)`. If the condition is true, it returns `"x is greater than y"`, otherwise, it returns `"y is greater than or equal to x"`. 

  

The `switch` statement allows for multiple conditional cases based on the value of an expression, while the ternary operator provides a concise way to create conditional expressions that return different values based on a condition.  

Both are useful tools for controlling the flow of execution in Java. 

 
# Day 5 JAva Modifiers

Java provides a number of access modifiers to set access levels for classes, variables, methods, and constructors. 
## The four access levels are:
Visible to the package, the default. No modifiers are needed.
Visible to the class only (private).
Visible to the world (public).
Visible to the package and all subclasses (protected).

## Default Access Modifier - No Keyword
Default access modifier means we do not explicitly declare an access modifier for a class, field, method, etc.
A variable or method declared without any access control modifier is available to any other class in the same package. The fields in an interface are implicitly public static final and the methods in an interface are by default public.
### Example
Variables and methods can be declared without any modifiers, as in the following an example:

String version = "1.5.1";
boolean processOrder() {
   return true;
}

## Private Access Modifier - Private
Methods, variables, and constructors that are declared private can only be accessed within the declared class itself.Private access modifier is the most restrictive access level. Class and interfaces cannot be private.
Variables that are declared private can be accessed outside the class, if public getter methods are present in the class. Using the private modifier is the main way that an object encapsulates itself and hides data from the outside world.

### Example
The following class uses private access control

public class Logger {
   private String format;

   public String getFormat() {
      return this.format;
   }

   public void setFormat(String format) {
      this.format = format;
   }
}
The format variable of the Logger class is private, so there's no way for other classes to retrieve or set its value directly. So, to make this variable available to the outside world, we defined two public methods: getFormat(), which returns the value of format, and setFormat(String), which sets its value.

## Public Access Modifier - Public
A class, method, constructor, interface, etc. declared public can be accessed from any other class. Therefore, fields, methods, blocks declared inside a public class can be accessed from any class belonging to the Java Universe.

However, if the public class we are trying to access is in a different package, then the public class still needs to be imported. Because of class inheritance, all public methods and variables of a class are inherited by its subclasses.

### Example
The following function uses public access control:

Public static void main(String[] arguments) {
}
The main() method of an application has to be public. Otherwise, it could not be called by a Java interpreter (such as java) to run the class.

## Protected Access Modifier - Protected
Variables, methods, and constructors, which are declared protected in a superclass can be accessed only by the subclasses in other package or any class within the package of the protected members' class. The protected access modifier cannot be applied to class and interfaces. Methods, fields can be declared protected, however methods and fields in a interface cannot be declared protected. Protected access gives the subclass a chance to use the helper method or variable, while preventing a nonrelated class from trying to use it.

### Example
The following parent class uses protected access control, to allow its child class override openSpeaker() method:
class AudioPlayer {
   protected boolean openSpeaker(Speaker sp) {
      // implementation details
   }
}

class StreamingAudioPlayer extends AudioPlayer {
   boolean openSpeaker(Speaker sp) {
      // implementation details
   }
}
If we define openSpeaker() method as private, then it would not be accessible from any other class other than AudioPlayer. If we define it as public, then it would become accessible to all the outside world. But our intention is to expose this method to its subclass only, that's why we have used protected modifier.

## Access Control and Inheritance
The following rules for inherited methods are enforced:
1. Methods declared public in a superclass also must be public in all subclasses.
2. Methods declared protected in a superclass must either be protected or public in subclasses; they cannot be private.
3. Methods declared private are not inherited at all, so there is no rule for them.

Example
In this example, we've created a class with a private variable age and a variable with default scope as name. Using setter/getter method, we're updating age and getting value and name is updated directly.

public class Puppy {
   private int age;
   String name;

   public Puppy() {      
   }

   public void setAge( int age ) {
      this.age = age;
   }

   public int getAge( ) {
      return age;
   }

   public static void main(String []args) {
      Puppy myPuppy = new Puppy();

      // update age variable using method call
      myPuppy.setAge( 2 );

      // update name directly
      myPuppy.name = "Tommy";
      System.out.println("Age: " + myPuppy.getAge() +", name: " + myPuppy.name );
   }
}
Output

Age: 2, name: Tommy
# =====================================================================================================================================week 2====================================================================================================================================================================

# Day 1
## What is Git? 

- **Definition:** A distributed version control system for tracking changes in source code. 

- **Founder:** Linus Torvalds (2005). 

## Key Features 

 

1. **Distributed System** 

   - Full copies for every user. 

   - Enables offline work and collaboration without a central server. 

2. **Snapshots, Not Deltas** 

   - Stores entire project snapshots at each point in time. 

   - Faster operations and data integrity. 

3. **Branching and Merging** 

   - Easy parallel development on separate branches. 

   - Seamless merging of changes. 

4. **Commit Hashing** 

   - Unique hash for each commit. 

   - Guarantees project history integrity. 

5. **Staging Area** 

   - Selective commits for flexibility. 

   - Clear separation of working directory and repository. 

 

## Benefits of Using Git 

 

1. **Version Control** 

   - Detailed history and rollback capabilities. 

   - Facilitates collaborative development. 

 

2. **Speed and Efficiency** 

   - Fast, local operations. 

   - Offline work capabilities. 

3. **Distributed Development** 

   - Reduces reliance on a central server. 

   - Every user has a complete repository. 

 

4. **Traceability and Accountability** 

   - Unique commit hashes for clear tracking. 

   - Records contributor contributions. 

5. **Branching and Merging** 

   - Parallel development and smooth merging. 

   - Supports different development streams. 

 

## Git Ecosystem 

- **GitHub and GitLab** 

  - Hosting platforms with collaboration features. 

  - Issue tracking, pull requests, and more. 

- **Community and Open Source** 

  - Large and active community. 

  - Encourages collaboration. 

 

- **Integration and Compatibility** 

  - Rich set of tools and CI/CD pipeline support. 

  - Flexible for various projects and workflows. 
# Day2
Git is a distributed revision control and source code management system with an emphasis on speed. Git was initially designed and developed by Linus Torvalds for Linux kernel development. Git is a free software distributed under the terms of the GNU General Public License version 2. This tutorial explains how to use Git for project version control in a distributed environment while working on web-based and non web-based applications development. We can  use Git to handle all levels of Java and Non-Java projects. So an exposure to software development life cycle and working knowledge of developing web-based and non web-based applications is a good start to work with GIt tools.Git comes with some tools like Git Bash, Git GUI to provide the interface between machine and user. It supports inbuilt as well as third-party tools.Git comes with built-in GUI tools like git bash, git-gui, and gitk for committing and browsing. It also supports several third-party tools for users looking for platform-specific experience.
Git Package Tools
Git provides powerful functionality tools such as commands, command line, Git GUI. Let's have a glimpse of some essential package tools.
GitBash
Git Bash is an application for the Windows environment. It is used as Git command line for windows. Git Bash provides an emulation layer for a Git command-line experience. Bash is an abbreviation of Bourne Again Shell. Git package installer contains Bash, bash utilities, and Git on a Windows operating system.
Git Bash Commands
Git Bash comes with some additional commands that are stored in the /usr/bin directory of the Git Bash emulation. Git Bash can provide a robust shell experience on Windows. Git Bash comes with some essential shell commands like Ssh, scp, cat, find.

Git Bash also includes the full set of Git core commands like git clone, git commit, git checkout, git push, and more.

Git GUI
Git GUI is a powerful alternative to Git BASH. It offers a graphical version of the Git command line function, as well as comprehensive visual diff tools. We can access it by simply right click on a folder or location in windows explorer. Also, we can access it through the command line by typing below command.
Git facilitates with some built-in GUI tools for committing (git-gui) and browsing (gitk), but there are many third-party tools for users looking for platform-specific experience.

Gitk
gitk is a graphical history viewer tool. It's a robust GUI shell over git log and git grep. This tool is used to find something that happened in the past or visualize your project's history.

Gitk can invoke from the command-line. Just change directory into a Git repository, and type:

$ gitk [git log options]
# According to Tutorialspoint : 
# Version Control System
Version Control System (VCS) is a software that helps software developers to work together and maintain a complete history of their work.
Listed below are the functions of a VCS : 
1. Allows developers to work simultaneously.
2. Does not allow overwriting each other’s changes.
3. Maintains a history of every version.

Following are the types of VCS :
1. Centralized version control system (CVCS).
2. Distributed/Decentralized version control system (DVCS).

# Distributed Version Control System
Centralized version control system (CVCS) uses a central server to store all files and enables team collaboration. But the major drawback of CVCS is its single point of failure, i.e., failure of the central server. Unfortunately, if the central server goes down for an hour, then during that hour, no one can collaborate at all. And even in a worst case, if the disk of the central server gets corrupted and proper backup has not been taken, then you will lose the entire history of the project. Here, distributed version control system (DVCS) comes into picture.

DVCS clients not only check out the latest snapshot of the directory but they also fully mirror the repository. If the server goes down, then the repository from any client can be copied back to the server to restore it. Every checkout is a full backup of the repository. Git does not rely on the central server and that is why you can perform many operations when you are offline. You can commit changes, create branches, view logs, and perform other operations when you are offline. You require network connection only to publish your changes and take the latest changes.

DVCS Terminologies
Local Repository
Every VCS tool provides a private workplace as a working copy. Developers make changes in their private workplace and after commit, these changes become a part of the repository. Git takes it one step further by providing them a private copy of the whole repository. Users can perform many operations with this repository such as add file, remove file, rename file, move file, commit changes, and many more.

Working Directory and Staging Area or Index
The working directory is the place where files are checked out. In other CVCS, developers generally make modifications and commit their changes directly to the repository. But Git uses a different strategy. Git doesn’t track each and every modified file. Whenever you do commit an operation, Git looks for the files present in the staging area. Only those files present in the staging area are considered for commit and not all the modified files.

Let us see the basic workflow of Git.

Step 1 − You modify a file from the working directory.

Step 2 − You add these files to the staging area.

Step 3 − You perform commit operation that moves the files from the staging area. After push operation, it stores the changes permanently to the Git repository.

### Git Tutorial
Suppose you modified two files, namely “sort.c” and “search.c” and you want two different commits for each operation. You can add one file in the staging area and do commit. After the first commit, repeat the same procedure for another file.

# First commit
[bash]$ git add sort.c

# adds file to the staging area
[bash]$ git commit –m “Added sort operation”

# Second commit
[bash]$ git add search.c

# adds file to the staging area
[bash]$ git commit –m “Added search operation”

## Blobs
Blob stands for Binary Large Object. Each version of a file is represented by blob. A blob holds the file data but doesn’t contain any metadata about the file. It is a binary file, and in Git database, it is named as SHA1 hash of that file. In Git, files are not addressed by names. Everything is content-addressed.

## Trees
Tree is an object, which represents a directory. It holds blobs as well as other sub-directories. A tree is a binary file that stores references to blobs and trees which are also named as SHA1 hash of the tree object.

## Commits
Commit holds the current state of the repository. A commit is also named by SHA1 hash. You can consider a commit object as a node of the linked list. Every commit object has a pointer to the parent commit object. From a given commit, you can traverse back by looking at the parent pointer to view the history of the commit. If a commit has multiple parent commits, then that particular commit has been created by merging two branches.

## Branches
Branches are used to create another line of development. By default, Git has a master branch, which is same as trunk in Subversion. Usually, a branch is created to work on a new feature. Once the feature is completed, it is merged back with the master branch and we delete the branch. Every branch is referenced by HEAD, which points to the latest commit in the branch. Whenever you make a commit, HEAD is updated with the latest commit.

## Tags
Tag assigns a meaningful name with a specific version in the repository. Tags are very similar to branches, but the difference is that tags are immutable. It means, tag is a branch, which nobody intends to modify. Once a tag is created for a particular commit, even if you create a new commit, it will not be updated. Usually, developers create tags for product releases.

## Clone
Clone operation creates the instance of the repository. Clone operation not only checks out the working copy, but it also mirrors the complete repository. Users can perform many operations with this local repository. The only time networking gets involved is when the repository instances are being synchronized.

## Pull
Pull operation copies the changes from a remote repository instance to a local one. The pull operation is used for synchronization between two repository instances. This is same as the update operation in Subversion.

## Push
Push operation copies changes from a local repository instance to a remote one. This is used to store the changes permanently into the Git repository. This is same as the commit operation in Subversion.

## HEAD
HEAD is a pointer, which always points to the latest commit in the branch. Whenever you make a commit, HEAD is updated with the latest commit. The heads of the branches are stored in .git/refs/heads/ directory.

[CentOS]$ ls -1 .git/refs/heads/
master

[CentOS]$ cat .git/refs/heads/master
570837e7d58fa4bccd86cb575d884502188b0c49
## Revision
Revision represents the version of the source code. Revisions in Git are represented by commits. These commits are identified by SHA1 secure hashes.

## URL
URL represents the location of the Git repository. Git URL is stored in config file.

[tom@CentOS tom_repo]$ pwd
/home/tom/tom_repo

[tom@CentOS tom_repo]$ cat .git/config
[core]
repositoryformatversion = 0
filemode = true
bare = false
logallrefupdates = true
[remote "origin"]
url = gituser@git.server.com:project.git
fetch = +refs/heads/*:refs/remotes/origin/*

Use git merge when you want to keep a clear record of when and where changes were merged. Merging is a safe option and is appropriate for public branches.

Use git rebase when you want to create a more linear and cleaner commit history. This is beneficial for feature branches, but be cautious when rebasing commits that have been pushed to a shared repository, as it rewrites history.


# Day 3
# Day 4
# Day 5
