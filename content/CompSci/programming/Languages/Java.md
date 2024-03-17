---
Credits: 4
Done: false
---
```java
int[] numbers = new int[3];

float num1 = 1.23456f;
float num2 = 2.34567f;
System.out.printf("The first area is %.2f and the second area is %.2f %n", 
num1, num2); //%n to print a new line
```

## Lecture 2: Expressions, Variables, Operators, Assignments, and Statements

### Program Organisation

- File name must be as same as class name
- A Java program needs to start its execution from the main method of some class
### Variable types:
- Local variables: variable declared inside a method
- Parameters: variable that is passed to a method when the method is called/executed.

---

- Primitive vs reference variable
    - Primitive values:
        - 
			```java
        byte //1 byte
        short //2 bytes
        int //4 bytes
        long //8 bytes
        float //4 bytes
        double //8 bytes
        char //2 bytes
        boolean //1 bit
        ```
        
    - Referent variable:
        
        ```java
        Student s1 = new Student();
        ```
        

---

### Statements

- A statement is a complete unit of execution that performs a specific action (end with’;’). For example:
    
    ```java
    System.out.println("This goes down the line!");
    System.out.print("This doesnt!");
    System.out.printf("This for formatted string");
    ```
    
- The System is a class, out is the object of PrintStream class.
    
- The println() is the method of PrintStream class which displays the result and then moves the cursor to the next line
    
- Declaration: `int a = 10;`
    

---

- The if...else Statement
    
    ```java
    int x = 30;        
    if( x == 10 )
    {          
    		System.out.print("Value of X is 10");       
    }
    else if( x == 20 )
    {          
    		System.out.print("Value of X is 20");       
    }
    else if( x == 30 )
    {          
    		System.out.print("Value of X is 30");       
    }
    else
    {          
    		System.out.print("This is else statement");      
    }
    ```
    
- The switch Statement
    
    ```java
    public static void main(String args[])
    { 
    		char grade = args[0].charAt(0); 
    		switch(grade) 
    		{ 
    				case 'A' :  System.out.println("Excellent!"); 
    										break; 
    				case 'B' : 
    				case 'C' :  System.out.println("Well done"); 
    										break; 
    				case 'D' :  System.out.println("You passed"); 
    				case 'F' :  System.out.println("Better try again"); 
    										break; 
    				default :  System.out.println("Invalid grade"); 
    		} 
    		System.out.println("Your grade is " + grade);
    } 
    ```
    

---

- The while Loop
    
    ```jsx
    int x= 10;        
    while( x < 20 )
    {          
    			System.out.print("value of x : " + x );          
    			x++;          
    			System.out.print("\\n");       
    }    
    ```
    
- The do...while Loop
    
    ```java
    int x= 10;        
    do{          
    			System.out.print("value of x : " + x );          
    			x++;          
    			System.out.print("\\n");       
    }while( x < 20 );    
    ```
    
- The for Loop
    
    ```java
    for(int x = 10; x < 20; x = x+1)
    {          
    		System.out.print("value of x : " + x );          
    		System.out.print("\\n");       
    }   
    
    for 
    ```
    
- For each loop:
    
    ```java
    String[] cars = {"Volvo", "BMW", "Ford", "Mazda"};
    for (String i : cars) {
      System.out.println(i);
    }
    ```
    
- Enhanced for loop in Java
    
    ```java
        
    int [] numbers = {10, 20, 30, 40, 50};        
    for(int x : numbers )
    {          
    		System.out.print( x );          
    		System.out.print(",");       
    }       
         
    String [] names ={"James", "Larry", "Tom", "Lacy"};       
    for( String name : names ) 
    {          
    		System.out.print( name );          
    		System.out.print(",");       
    }   
    ```
    

---

- The break Keyword
    
    ```java
    int [] numbers = {10, 20, 30, 40, 50};        
    for(int x : numbers )
    {          
    		if( x == 30 )
    		{      
    				break;          
    		}          
    		System.out.print( x );          
    		System.out.print("\\n");       
    } 
    ```
    
- The continue Keyword
    
    ```java
    int [] numbers = {10, 20, 30, 40, 50};        
    for(int x : numbers )
    {          
    		if( x == 30 )
    		{      
    					continue;          
    		}          
    		System.out.print( x );          
    		System.out.print("\\n");       
    } 
    ```
    

### String Concatenation

```
System.out.println(str1.concat(str2));
System.out.println(str1+str2);
System.out.println(str1 += str2); // all the same
```

### String Methods

```
String s = "hello it is me";
String[] words = s.split(" ");

double length = Double.parseDouble("1.5");
```

### Postfix/Prefix in/decrement

```java
int i = 0;
System.out.println(i++); // 0, postfix print i first then add
System.out.println(++i);  // 2, prefix add first then print i
```

### Java Type Casting

- Java supports two types of casting:

![Screenshot 2023-02-27 at 23.43.08.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/bd65a4f5-db17-4ca7-bc56-43de4911a30a/Screenshot_2023-02-27_at_23.43.08.png)

1. **Widening Casting (Implicit):** done automatically by Java when we assign a value of a smaller data type to a variable of a larger data type. For example:

```
int x = 10;
double y = x; // Implicit casting from int to double
```

1. **Narrowing Casting (Explicit):** done manually by the programmer when we assign a value of a larger data type to a variable of a smaller data type. For example:

```java
double x = 10.5;
int y = (int) x; // Explicit casting from double to int

int a = 100;
byte b = (byte) a; // Explicit casting from int to byte

float c = 3.14f;
int d = (int) c; // Explicit casting from float to int

long e = 1234567890;
int f = (int) e; // Explicit casting from long to int
```

- Parsing:
    - To int: `int j = Interger.parseInt(s);`

### Getting Inputs

- Important to instantiate new Scanner object `Scanner input = new Scanner (System.in);`
    - import the scanner first `import java.util.Scanner;`
    - important to close the object
- Also, close scanner object when done

```java
import java.util.Scanner;
public class MyPrintString 
{
		public static void main(String[] args) 
		{
				Scanner input = new Scanner (System.in);
				System.out.printIn("Enter your name: ");
				String name = input.nextLine();
				System.out.print("How many thieves are watching now? ");
				int numb = input.nextInt ();
				System.out.printIn("The return of " + name + " and the " + numb + " thieves!");
				// closing the scanner object 
				input.close();
		}
}
```

## Lecture 3: Program Structure, Organization, and Modular Programming in Java

### OOP:

- Abstraction: a process of hiding the implementation details from the user
    - Abstract Data Type (ADT): a special data type that is defined by a set of values and a set of operations on that type
    - Encapsulation: a process of binding data and functions together into a single unit such that they are kept both safe from outside interference and misuse
        - Make the instance variables private so that they cannot be accessed directly from outside the class, only through `getter()` and `setter()` methods in the class to set and get the values of the fields
    - Inheritance: a process by which one class takes on the attributes and methods of another
        - super class: the class that child classes are derived from
        - sub class : newly formed class that can override or extend the attributes and methods of parent classes
    - Polymorphism (“many forms”): the ability of programming languages to present the same interface for differing underlying data types.

### Program Structure

```java
public class Person {
    private String name;
    private int age;

    public Person(String name, int age) 
		{
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return this.name;
    }

    public int getAge() {
        return this.age;
    }
}
```

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/57a3484e-554e-4072-a5b4-5c8a15b315bd/Untitled.png)

### Packages

- A Java program is typically organized into packages. A package, written in lowercase, is a collection of related classes
    
    - We declare the package name in which the class is placed
    - It must be defined before any class and interface declaration
    - Only one (1) package statement in a Java program.
    
    ```java
    package vn.vinuni.salary; 
    // package named salary created by a programmer at vinuni.vn
    
    public class Person {
        // ...
    }
    ```
    

### Import

- If we want to use any class of a particular package, we need to import that class.
- The import statement is used to represent the class stored in the other package

```java
import java.util.Scanner;  //it imports the Scanner class only 
import java.util.*; //it imports all the class of the java.util package
```

### Interface

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/71d9498d-be31-4c22-afac-f1d08d1aeaa4/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f5ad4907-0524-4c3e-9b28-267bbcdcfe72/Untitled.png)

- Interface section contains only static constants and abstract method declarations which cannot be instantiated, no constructor
    
- An interface is a completely abstract class that is used to gather related methods (with empty bodies) for two objects to interact
    
- To access the interface methods, the interface need to be implemented by another class with the implements keyword.
    
- When a class implements an interface, it must implement all of the methods declared in the interface!
    
- Interface’s methods with body only with default keyword
    
    ```java
    interface Template1
    {
        default void myMethod()
        {
            System.out.println("yo");
        }
        default void myMethod2()
        {
            System.out.println("yo2");
        }
    		String method3();
    }
    ```
    

## Lecture 4: Strong Typing, Classes, Objects, and Exceptions

### Classes

- A Java program consists of one or more classes. A class is a blueprint for creating objects that have similar attributes and behaviors. For example:

```java
public class Person {
    private String name;
    private int age;

    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }

    public String getName() {
        return this.name;
    }

    public int getAge() {
        return this.age;
    }
}
```

### Class variable (static field)

- Variable that belongs to a class.
    
- The static variables can be get and set in program thru objects
    
- They are common to all instances of that class, i.e., changes made to class variables by one object will reflect in all objects.
    
    - Preferably to use class’s variable
    
    ```java
    class Library {
    		public static int quantity; // static variable
    		static String name = "Ali Baba"; // static variable
    }
    public class ClassVariables {
    		public static void main(String[1 args) 
    		{
    				Library bookObj1 = new Library();
    				Library bookObj2 = new Library ();
    				// accessing class variable via class anme
    				System.out.println (Library.quantity); // 0
    				System.out.println (Library.name); // Ali Baba
    				// changing class variable via class name
    				Library.quantity = 1005;
    				Library.name = "Michael Jackson";
    				// accessing class variable via class name
    				System.out.println (Library.quantity); // 1005
    				System.out.println(Library.name); // Micheal Jackson
    		}
    }
    ```
    

### Object variable (instance fields)

- Variables that belongs to an object
    
    ```java
    Library bookObj1 = new Library();
    Library bookObj2 = new Library ();
    // accessing class variable via book1
    System.out.println (bookObj1.quantity); //0
    System.out.println (bookObj1.name); // Ali Baba
    // changing class variable via book
    bookObj2.quantity = 1005;
    bookObj2.name = "Michael Jackson";
    // accessing class variable via book1
    System.out.println (bookObj1.quantity); // 1005
    System.out.println(bookObj1.name); //Micheal Jackson
    ```
    

### Constant variables

- Constant is used in Java when a static value or a permanent value(never change from the initial value) for a variable has to be implemented
    
    - Use `static` and `final` access modifier to implement
    - Conventionally all capital
    
    ```java
    public static final float PI = 3.14;
    final static String DEPARTMENT = "CECS";
    ```
    

### Abstract class

- Only meant to be inherited (extends), not instantiate
- May or may not contain abstract methods
- Can contain normal methods too
- Inherited classes must implement abstract methods if included

```java
public abstract class Dog
{
		String breed;
}
public class Chihuahua extends Dog
{
		// statements
}
```

### Abstract methods

- Must be empty and be inside an abstract class
- If inherited by a normal class, that class must be override abstract methods
- Abstract class can inherit another abstract class without implementation abstract methods

```java
public abstract class Dog
{
		public abstract void Poop();
		public void Bark()
		{
				System.out.println("Woof");
		}
}
public class Chihuahua extends Dog
{
		public void Poop()
		{
				//implementation
		}
}
public class Main(String[] args)
{
		Chihuahua c = new Chihuahua();
		c.Poop(); // from Chihuahua class
		c.Bark(); // from Chihuahua which is from Bark
}
```

### Objects

- An object is an instance of a class

```java
public class Person
{
		String name, int age;
		public person(String name, int age)
		{
				this.name = name;
				this.age = age;
		}
}
Person person = new Person("John", 30);
```

### Exceptions

- An exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions. In Java, exceptions are handled using try-catch blocks. Common scenarios are:
    
    - Invalid data in the input
    - Cannot open file
    - Network connection
    - JVM run out of memory
- Types of exceptions:
    
    - Checked exceptions (compile time exceptions): checks by the compiler, e.g., network connection, missing file,..
    - Unchecked exceptions (runtime exceptions): occurs at the time of execution, e.g, programming bugs such as logic errors or improper use of an API,..
    - Errors: problems that arise beyond the control of the user or the programmer, e.g., stack overflow, out of memory,…



```java
try 
{
    int x = 5 / 0;
		// or sth studpid
} 
catch (ArithmeticException e) 
{
    System.out.println("Division by zero!");
} finally  // optional
{
		//statements to run whether exception is thrown or not
}
```

- Strong Typing
    
    Strong typing is a programming language feature that ensures that variables are used only in ways that are consistent with their declared types. For example:
    
    ```
    int x = 5;
    String s = "Hello, world!";
    int y = x + s; // This will result in a compile-time error
    
    ```
    
    In this example, the variable `y` is assigned the value of `x + s`, which is not allowed because `x` is an `int` and `s` is a `String`.
    

### Java access-modifiers

![Screenshot 2023-03-01 at 21.47.04.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/12276665-9f91-4535-9755-0a0ec8fe56f7/Screenshot_2023-03-01_at_21.47.04.png)

### “this” keyword

- `this` can be used to:
    1. refer current class instance variable.
        
        ```java
        class Member {
        		String name;
        		int age;
        		Member (String name, int age) 
        		{
        				this.name = name;
        				this.age = age;
        		}
        		public void displayInfo() 
        		{
        			System.out.println
        			(name + "," + age);
        		}
        }
        public class thisKeyword 
        {
        		public static void main (String[] args) 
        		{
        				Member m = new Member ("Ali Baba", 20);
        				m.displayInfo ();
        		}
        }
        ```
        
    2. invoke current class method (implicitly).
        
        ![Screenshot 2023-03-01 at 22.01.07.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/45ca78f8-02a3-4142-a9fb-bbfa5ee5c8ff/Screenshot_2023-03-01_at_22.01.07.png)
        
    3. invoke current class constructor (constructor chaining)
        
        ![Screenshot 2023-03-01 at 22.01.51.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7fdabb09-c1db-4cff-9024-56d24e5c098e/Screenshot_2023-03-01_at_22.01.51.png)
        
    4. be passed as an argument in the method call.
        
    5. be passed as an argument in the constructor call.
        
    6. used to return the current class instance from the method.
        

## Lecture 5: Java Constructors and Inheritance

### Constructors

- A constructor method, same name with class, is a special method that is used to initialize objects, called whenever an instance is created
    
- Default constructor
    
    - It is generated automatically if not implemented
    
    ```java
    public class Person {
        private String name;
        private int age;
    		static int nbOfPersons;
    
        public Person() {
            this.name = name;
            this.age = age;
    				nbOfPersons += 1;
        }
    }
    ```
    
- Parameterized constructor
    
    ```java
    public class Person {
        private String name;
        private int age;
    
        public Person(String name, int age) {
            this.name = name;
            this.age = age;
        }
    }
    ```
    

### Constructor overloading

```java
class Car{
		int year;
		String brand, color; 
		int price;

		Car (String col)
		{
				color = col;
				System.out.printIn("Car is created.");
		}

		Car(int yr, String br)
		{
				year = yr;
				brand = br;
		}

		void displayInfo()
		{
				System.out.printIn("This " + brand + " car is
		}

		void displayColor() 
		{
				System.out.printIn("Your car is " + color);
		}
}
public class MyJavaConstructors {
		public static void main (String[] args) 
		{
				Car firstCar = new Car ("Red");
				firstCar. displayColor ();
				Car secondCar = new Car (2020, "VinFast");
				secondCar.displayInfo();
		}
}
```

- this() reference:
    
    - Must be the first statement inside a constructor
    
    ```java
    String color;
    Car()
    {
    		System.out.printIn("Car is created.");
    }
    Car (String col)
    {
    		this (); //call Car() constructor
    		color = col;
    }
    ```
    

### Initializer blocks

- Multiple static blocks will execute in order

1. Static initialization block: runs when the class is loaded into memory, before any instances of the class are created. This block is used to initialize static variables.
2. Initialization block: runs when an instance of the class is created, before the constructor. This block is used to initialize instance variables.
3. Constructor: runs when an instance of the class is created. It is used to set the initial state of the object and can take parameters to initialize instance variables.

```java
class Temp {
		// 1. static initialization block
		static {
				System.out.print("I am static init block!");
		}
		// 2. initialization block
		{
			System.out.print("I am init block!");
		}
		// default constructor
		Temp () {
				System.out.print("Default constructor");
		}
```

### Inheritance

- Inheritance is a programming technique that allows a class to inherit attributes and methods from another class. Keyword `extends`

![Screenshot 2023-03-01 at 23.15.29.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4ee595e2-e952-4665-9680-a4df6209c6df/Screenshot_2023-03-01_at_23.15.29.png)

```java
class Person 
{
    private String name;
    private int age;
    public Person(String name, int age) {
        this.name = name;
        this.age = age;
    }
}
public class Student extends Person 
{
    private int studentId;
    public Student(String name, int age, int studentId) 
		{
        super(name, age); // invokes parent's constructor
        this.studentId = studentId; 
    }

    public int getStudentId() {
        return this.studentId;
    }
}
```

- Multiple and Hybrid are supported through interface only
    - Multiple inheritance
        
        ```java
        interface SuperClass1 {
        		void Read ();
        }
        
        interface SuperClass2 {
        		void Write();
        }
        
        class Subclass implements Superclass1, Superclass2 {
        		public void Read() {
        				System.out.printIn("Reading...");
        		}
        		public void Write() {
        				System.out.printIn("Writing...");
        		}
        }
        ```
        
    - Hybrid inheritance
        
        ```java
        interface SuperClass1 {
        		void Read ();
        }
        
        interface SuperClass2 {
        		void Write();
        }
        
        class Subclass implements Superclass1, Superclass2 {
        		public void Read() {
        				System.out.println("Reading...");
        		}
        		public void Write() {
        				System.out.println("Writing...");
        		}
        }
        ```
        

## Lecture 6: Static Classes and Members

### Instance variable

- Declared in a class but outside of any block, method or constructor.
- Accessible to all the constructors, blocks and methods in the class.

### Static variable

- A static class is a class that cannot be instantiated and is used only to provide static methods and attributes
- Can be accessed without an object
- Can be reassigned with an object, but it will change the value for all other instances

```java
public class MathUtils {
    public static int add(int x, int y) {
        return x + y;
    }

    public static int subtract(int x, int y) {
        return x - y;
    }
}

MathUtils.add(5,4);
```

---

### Instance method

- An instance must be created to be used

### Static method

- Call directly from class without an instance `ClassName.StaticMethodName()`

---

### Static class

- Cannot be instantiated and is used only to provide static methods and attributes
- Static methods and attributes can be accessed without creating an instance of the class as long as access is granted
- Can not call instance methods or access instance variable

---

### Nested class

- Non-static nested classes (inner classes):
    
    - Have access to other members of the enclosing class (even if they are declared private)
        
    - Inner class cannot define any static member
        
    - To instantiate an inner class, you must first instantiate the outer class. Then, create the inner object within the outer object.
        
        ```java
        public class MyOuterClass
        {
        		int distance = 200;
        		class MyInnerClass
        		{
        				void printInfo() 
        				{
        						System.out.println(distance+"KM");
        				}
        		}
        		public static void main(String[] args) 
        		{
        				MyOuterClass objOuter = new MyOuterClass();
        				MyOuterClass.MyInnerclass objInner = objOuter.new MyInnerclass();
        				objInner.printInfo();
        		}
        }
        ```
        
- Static nested classes:
    
    - Cannot access to other members of the enclosing class
    - Inner class can be declared private, public, protected, package private while outer class can only be declared public or package private
    
    ```java
    public class MyOuterClass {
        private static String myUni = "VinUniversity";
        static int year = 2020;
        static class MyStaticNestedClass
        {
            private static String location = "Hanoi";
            public void dispInfo() 
            {
                System.out.println (myUni);
                System.out.println (year);
            }
        }
        public static void main(String[] args) 
        {
            MyOuterClass.MyStaticNestedClass obj = new MyStaticNestedClass ();
    				// MyStaticNestedClass obj = new MyStaticNestedClass (); is fine too
            obj.dispInfo();
            System.out.println(MyStaticNestedClass.location);
        }
    }
    ```
    

### Java anonymous inner class

- A local class without a name, which is used to declare and instantiate a class at the same time
- It is often used to create an object that implements an interface or extends an abstract class without having to define a separate class for it
- Often used for GUI applications
- Keyword `@Override`

```java
class Zoo{
		public void animalSound(){
		System.out.printIn("Meow Meow!");
}
public class AnonymousInnerClass {
		public static void main (String[] args) 
		{
				Zoo animal = new Zoo ();
				animal.animalsound();
				Zoo dinosaur = new Zoo (){
						@Override
						public void animalsound() {
						System.out.println("nguuooooooooo!");
		};
		dinosaur.animalsound();
}
```

### Recursion

## Lecture 7: Polymorphism

### Method Overloading

- Like constructor overloading, it create multiple methods with the same name but with different parameters or argument types
- It is performed within class
- When you call an overloaded method, Java matches the method call to the correct method based on the number and types of arguments. To overload, we can change:
    - Number of args
    - Arg datatype
    - Both number of args and arg datatype

```java
public class MyClass {
    public void myMethod(int x) {
        // statements
    }

    public void myMethod(int x, int y) {
        // statements
    }
		public void myMethod(float x, int y) {
        // statements
    }
}
```

### Method Overriding

- When a subclass has the same method signature (name, parameters list, return type) as declared in the parent class, the subclass redefine that method, provide a specialized version
- The overridden method must have the same access modifiers (public, private, protected) and return type as the original method. The subclass can have a more permissive access modifier for the overridden method, but not a more restrictive one.

```java
class Animal {
    public void makeSound() {
        System.out.println("Animal is making a sound");
    }
}

class Dog extends Animal {
    @Override
    public void makeSound() {
        System.out.println("Dog is barking");
    }
}
```

### Static method hiding

- When overriding static methods in inheritance
- If a subclass defines a static method with the same signature as a static method in the parent class, the static method in the parent class is hidden.
- The version getting invoked depends on whether its invoked from superclass or subclass, not the object itself

```java
class Parent {
    static void myMethod() {
        System.out.println("Parent Version");
    }
}

class Child extends Parent {
    static void myMethod() {
        System.out.println("Child Version");
    }
}

public class Main {
    public static void main(String[] args) {
        Parent p = new Child();
        p.myMethod(); // Output: "Parent Version"
    }
}
```

### Types of Polymorphism

There are two types of polymorphism in Java:

- Static polymorphism: resolved at compile time
    - Method Overloading
- Dynamic polymorphism: resolved at runtime
    - Method overriding

### Class vs Abstract Class vs Interface

![Screenshot 2023-03-02 at 16.05.02.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1db613c4-2831-4567-8803-70432794cbb6/Screenshot_2023-03-02_at_16.05.02.png)

In Java, you can create three different types of classes:

- Class: A blueprint for creating objects. It can contain instance variables, constructors, methods, and static variables and methods.
- Abstract class: A class that cannot be instantiated but can be subclassed. It can contain instance variables, constructors, methods, and abstract methods. Abstract classes are useful when you want to provide a common interface for a group of related classes.
- Interface: A collection of abstract methods and constants. It defines a contract that a class must implement. A class can implement multiple interfaces, but can only extend one class. Interfaces are useful when you want to create a common interface for a group of unrelated classes.

## Lecture 8: Lists as Data Structures, Collections, Iterators, and Generics

### Collection interface

- A collection is a group of objects that can be treated as a single unit. In Java, collections are implemented using the `Collection` interface
- Can do searching, sorting, inserting, …
- e.g: java.util.Collection;

![Screenshot 2023-03-04 at 02.48.06.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/83657395-21da-45d0-81d1-8079df0fc43b/Screenshot_2023-03-04_at_02.48.06.png)

March 9, 2023 4:00 PM rewrite properties and methods from each class

```java
List<String> names = new ArrayList<String>();
names.add("Alice");
names.add("Bob");
names.add("Charlie");

Collections.sort(names);
```

|Array|List|ArrayList|
|---|---|---|
|A fixed-size data structure|A dynamic-size data structure|A dynamic-size data structure|
|Can hold only elements of the same data type|Can hold elements of different data types|Can hold elements of different data types|
|Requires explicit memory allocation|Automatically allocates memory|Automatically allocates memory|
|Elements can be accessed using an index|Elements can be accessed using an index|Elements can be accessed using an index|
|Cannot be resized once created|Can be resized dynamically|Can be resized dynamically|
|Can be multidimensional|Can be implemented as a single-dimensional or multidimensional collection|Can be implemented as a single-dimensional or multidimensional collection|
|Basic functionality in java|Part of the Java Collections Framework|Part of the Java Collections Framework|

![Screenshot 2023-05-04 at 15.41.05.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2234d036-63ba-4734-9e3d-6a5443d2d5e1/Screenshot_2023-05-04_at_15.41.05.png)

### Array

- Fixed size static data structure
    
    ```java
    int[] numbers = new int[2];
    number[0] = 10;
    number[1] = 11;
    
    int[] numbersNew = new int[2] {1,2};
    
    int[] scores;
    
    char[] grades = {'A', 'B', 'C'};
    ```
    

### List Interface:

- Found in java.util package, inherited from collection interface
    
- Unlike array, list allows you to add and remove elements after created, even resize the list
    
- `ListIterator interface`: allow us to iterate the list forward and backward
    
- Commonly used list methods:
    
    ```java
    // Create a new list of strings
    List<String> myList = new ArrayList<String>();
    
    // Add elements to the list
    myList.add("apple");
    
    // Add elements from another list to the list
    List<String> anotherList = new ArrayList<String>();
    anotherList.add("grape");
    anotherList.add(1, "orange");
    myList.addAll(anotherList);
    myList.addAll(1, anotherList);
    
    // Check if the list contains a specific element
    if (myList.contains("apple")) {
        System.out.println("The list contains apple.");
    }
    
    // Remove an element from the list
    myList.remove("grape");
    
    // Get the index of an element in the list
    int index = myList.indexOf("apple");
    
    // Check if two lists are equal
    if (myList.equals(anotherList2)) {
        System.out.println("The two lists are equal.");
    }
    ```
    

### ArrayList class `{}`

- `import java.util.ArrayList;`, a part of Collection framework
    
- ArrayList is a data structure that stores a collection of elements of the same type in a particular order as a single variable in Java
    
- A list is a data structure that stores a collection of elements of same type in a particular order as single variable. In Java, lists are implemented using the `List` interface
    
- The Contructor argument can be:
    
    ```java
    // empty
    List<String> names = new ArrayList<String>();
    
    // any collection
    Collection<String> myCollection = new ArrayList<String>();
    List<String> names = new ArrayList<String>(myCollection);
    
    // an int specify nb of items
    List<String> names = new ArrayList<String>(6);
    ```
    
- `List<String> names = new ArrayList<String>();`
    
    ```java
    names.add("Alice");
    names.add("Bob");
    names.add("Charlie");
    
    for (String x : names) 
    {
      System.out.println(x};
    }
    
    name.get(0); // get value at index 0
    ```
    

### Creating a list: `[]`

```java
//Creating a List of type String using ArrayList
List<String> list = new ArrayList<String> ();
//Creating a List of type Integer using ArrayList
List<Integer> list = new ArrayList<Integer>);
//Creating a List of type Book using ArrayList
List<Book> list = new ArrayList<Book>();
//Creating a List of type String using LinkedList
List<String> list = new LinkedList<String> ();

public List<String> write() {}
```

### List view of array

- `Arrays.asList()`and pass the array argument to ArrayList constructor to initialize an arraylist in single line statement
    
    ```java
    // Creating Arrays of String type
    String a[] = new String[] { "A", "B", "C", "D" };
    
    // Getting the list view of Array
    List<String> list = Arrays.asList(a);
    //The list is: [A, B, C, D]
    ```
    
- `List.of()` static factory methods to create immutable lists. Only drawback is that add operation is not supported in these lists
    
    - `import java.util.List;`
    
    ```java
    // Create a list of type String using List
    List<String> myEnemies = List.of("Thomas", "Tu"); // can not use add();
    ```
    

![Screenshot 2023-03-04 at 20.48.34.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/13f1f2d8-11e7-4e16-845b-c36782325de6/Screenshot_2023-03-04_at_20.48.34.png)

### Java Iterator

- Belongs to collection framework
- Traverse a collection of elements, access and remove data elements like a pointer
- Iterator starts before the value, here
- `import java.util.Iterator;`

![Screenshot 2023-03-04 at 18.55.35.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f7764094-ffd6-4098-b6cb-b8f0f1c1f2a3/Screenshot_2023-03-04_at_18.55.35.png)

- Methods:
    - `here.next()` returns the next element moves the iterator after that (after 15)
        
    - `here.remove()` removes the element behind it
        
    - `here.hasNext()` returns true if there is another element after it
        
        ```java
        List<String> names = new ArrayList<String>();
        names.add("Alice");
        names.add("Bob");
        names.add("Charlie");
        
        //Iterator here = names.iterator();
        Iterator<String> here = names.iterator(); // indicates everything is a string
        while (here.hasNext()) 
        {
            String name = here.next();
            System.out.println(name);
        }
        ```
        

### Java ListIterator

<aside> 💡 `Iterator<T> here = names.listIterator();`

</aside>

- extends of Java Iterator
- import `java.util.ListIterator;`
- Methods
    - `here.previous()` returns the previous element of the list
    - `here.previousIndex()` returns the index of the element that the `previous()` will return
    - `set()` replaces the element returned by either next() or previous with the specified element

### LinkedList

- extends Abstract SequencialList implements Deque
    - A linear data structure consisting of a collection of Nodes with any datatype that are not stored in contiguous but random memory locations
    - Helps to build even more complex data structures like Stacks, Queues, Skip Lists, etc.
    - List grows as per the program's demand (no resizing problem) and limited to the available memory space
- Each node is a data field, elements are linked using pointers to the memory address of the next node
- Types of LinkedList:
    1. Singly linked list
    2. Doubly linked list
    3. Circular Linked list

### Singly LinkedList

<aside> 💡 `List<String> linkedList = new LinkedList<String>();`

</aside>

- A class Node which has two attributes: data and next where next is a pointer to the next node. Create another class which has two attributes: head and tail
- First node is head, last is tail which has null pointer

```java
import java.util.LinkedList;
import java.util.List;
import java.util.Iterator;

public class MyLinkedList {
    public static void main(String[] args) {
        List<String> linkedList = new LinkedList<String>();

        linkedList.add("apple");
        linkedList.add("banana");
        linkedList.add("cherry");

        System.out.println(linkedList.get(1)); // "banana"
				linkedList.remove("banana");
				System.out.println(linkedList); // [apple, grape, cherry]

				String first = linkedList.getFirst();
        String last = linkedList.getLast();
    }
}
```

### Linkedlist Iterator

```java
for (String element : linkedList) {
    System.out.println(element);
}

// or
Iterator<String> iterator = linkedList.iterator();
while (iterator.hasNext()) {
    String element = iterator.next();
    System.out.println(element);
}
```

### Convert LinkedList to ArrayList

<aside> 💡 `ArrayList<String> arrayList = new ArrayList<String>(linkedList);`

</aside>

### Convert ArrayList to LinkedList

<aside> 💡 `LinkedList<String> linkedList = new LinkedList<String>(arrayList);`

</aside>

---

### Generics

<aside> 💡 `public class GenericType<T>; private T value`

</aside>

- Generics are a programming language feature that allows types (classes and interfaces) to be parameterized. In Java, generics are implemented using the `<T>` syntax
    
- Allows more than one type of object to be processed
    
- The parameter`T` must be an object type (Integer, Cat), no primitive type like int, double.
    
    ```java
    public class GenericType<T>
    public class GenericType<T extends Number> // only int, float, double, ...
    public class GenericType<T extends Animal> 
    // only Animal and its subclass's object
    {
        private T value;
    
        public GenericType(T value) 
    		{
            this.value = value;
        }
    
        public T getValue() {
            return this.value;
        }
    		void ShowType()
    		{
    				System.out.println(value.getClass().getName());
    		}
    }
    
    GenericType<String> genericVariable = new GenericType<String>("Hello, world!");
    String value = box.getValue();
    ```
    

### Multiple type parameter generic

```java
class Test2<T, U> 
class Test2<T extends Animal, U extends Number> 
{
		T obj1; // An object of type T 
		U obj2; // An object of type U
		// constructor
		Test2(T obj1, U obj2)
		{
				this.obj1 = obj1;
				this.obj2 = obj2;
		}
		// To print objects of T and U
		public void print() 
		{
				System.out.print]n(obj1);
				System.out.printin(obj2);
		}
}
public class GenericExample2 
{
		public static void main (String[] args) 
		{
				Test2<Do, Integer› obj = new Test2<Dog, Integer>(new Dog(), 25);
				obj.print (g);
		}
}
```

---

![Screenshot 2023-03-06 at 10.59.43.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/65fa6f42-9e41-4ae3-8875-cf8a2b2b7be2/Screenshot_2023-03-06_at_10.59.43.png)

## Lecture 9: Stacks

### Stacks (extends Vector)

<aside> 💡 `Stack<String> stack = new Stack<>();`

</aside>

- A stack is a dynamic data structure that stores a collection of elements in Last-In, First-Out or LIFO order
- `push` last-in, `pop` first-out
- Stacks are implemented using the `Stack` class
- Supports:
    - `push(e)`: to add item e onto the stack
    - `pop()`: to remove an item and returns the topmost item of the stack
    - `size()`: returns the number of items in the stack
    - `isEmpty()`: to check if a stack is empty
    - `peek()`: returns the element at the top of the Stack, only show
    - `search(element)`: return the position of the element from tos (1), -1 means not found
    - `indexOf(element)`: return the index of the element from bottom
    - `set(index, element)`
    - `get(index)`
    - `add(index, element)`: too
- throws `EmptyStackException` if empty

```java
Stack myStack = new Stack(); //object type, not recommended
Stack<String> stack = new Stack<>();
stack.push("Alice");
stack.push("Bob");
stack.push("Charlie");

String name = stack.pop();
```

### Converting

```java
Stack<String> stack = new Stack<>();

//Array to Stack
for (int i=0; i<arr.length; i++) {
    stack.push(arr[i]);
}

// List to Stack
for (String element : list) {
    stack.push(element);
}

//create a List from the Stack
List<String> list = new ArrayList<String>(stack);
```

### Error handling with stacks

- Stack underflow: when pop from an empty stack; check by !stack.isEmpty()
- Stack overflow: when push and nb of items reach the stated size, check by !stack.isFull()

---

## Lecture 10: Queue

### Queues (implements Queue)

<aside> 💡 `import java.util.LinkedList; Queue<String> queue1 = new LinkedList<>();`

</aside>

- For LinkedList, elements in the queue are stored internally in a standard linked list data structure
- A queue is a dynamic data structure that stores a collection of elements in First-In, First-Out or FIFO order
- `push` last-in, `pop` first-out
- Queue are implemented using the `LinkedList` class
    - `offer(e)`: enqueue a new element
    - `poll(e)`: dequeue the top element and return it, return null if empty
    - `peek()`: returns the first element of the Queue, only show
    - `isEmpty()`:
    
    - `add(e)`
    - `remove()`: throws exception if empty
    - `element()`:
    - `clear()`: clear the queue

```java
Queue<String> queue = new LinkedList<String>();
Queue<String> queue = new LinkedList<String>(Array.asList(anotherArray);
queue.add("Alice");
queue.add("Bob");
queue.add("Charlie");

String name = queue.remove();
```

### Iterate through queue

```java
Iterator<String> iterator = new queue.iterator();
while( iterator.hasNext())
{
		System.out.println(iterator.next());
}
// or 
for( String i : queue)
{
		System.out.println(i);
}
```

---

### PriorityQueue (extends Queue)

<aside> 💡 `import java.util.PriorityQueue; Queue<Integer> queue2 = new PriorityQueue<>();`

</aside>

- Operates like Queue but each item has a priority
    
- Stored in a binary heap, so order is different if used remove
    
- Only support comparable datatypes
    
- Automatically arranged in order, the lowest element first
    
- Stores its elements internally according to a Comparator passed to the PriorityQueue or according to their natural order
    
- Supports:
    
    - all methods queue has
    
    ```java
    Queue<Integer> queue2 = new PriorityQueue<>(Collections.reverseOrder());
    ```
    

---

### Comparable Interface

- Used to order the objects of the user-defined class
    
- Found in java.lang package and contains only one method named compareTo(Object)
    
- Provides single sorting sequence
    
    ```java
    PriorityQueue <Ingredient> maxHeap = new PriorityQueue<>
    																		(new Comparator<Ingredient>() {
        @Override
        public int compare(Ingredient a, Ingredient b)
        {
            return b.quantity - a.quantity;
        }
    });
    ```
    

### User-define comparing queue

### Implementation of queue

- Queue can be implemented by Array, Stack or LinkedList
    - Approach [A]: remove the element at head position, and then one by one shift all the other elements in forward position. There is an overhead of shifting the elements one position forward every time we remove the first element.
    - Approach [B]: remove the element$ from head position and then move head to the next position. The size on Queue is reduced by one space each time

## Lecture 11 & 12: Sorting Algorithms

### Bubble Sort: O(n^2)

- Swap the element to the adjacent if it is bigger
    
    ```java
    public static void bubbleSort(int[] array) 
    {
        int n = array.length;
    		int temp = 0;
        for (int i = 0; i < n - 1; i++) 
    		{
            for (int j = 0; j < n - i - 1; j++) 
    				{
                if (array[j] > array[j + 1]) {
    	              temp = array[j];
                    array[j] = array[j + 1];
                    array[j + 1] = temp;
                }
            }
        }
    }
    ```
    

![Screenshot 2023-03-07 at 10.41.37.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/83581f02-786a-478f-94d5-8c4722488984/Screenshot_2023-03-07_at_10.41.37.png)

### Selection Sort: O(n^2)

- Loop through and find the least element then swap it with the item in front of the sorted

![Screenshot 2023-03-07 at 10.40.33.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ed867815-be18-4fb5-ae81-2e7e6e70176d/Screenshot_2023-03-07_at_10.40.33.png)

```java
public static void selectionSort(int[] array)
{
    int n = array.length;
    for (int i = 0; i < n - 1; i++) {
        int minIndex = i;
        for (int j = i + 1; j < n; j++) {
            if (array[j] < array[minIndex]) {
                minIndex = j;
            }
        }
        int temp = array[minIndex];
        array[minIndex] = array[i];
        array[i] = temp;
    }
}
```

### Insertion Sort: O(n^2)

- Divide to sorted and unsorted parts and insert the next number to the right position
- Green number is key

![Screenshot 2023-03-07 at 10.42.23.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5deab573-bea1-42ba-be70-955a1fda9505/Screenshot_2023-03-07_at_10.42.23.png)

1. Start with the key as 2nd element
2. While bigger than the key, move elements of arr[0..i-1], that are greater than key to one position ahead of their current position

```java
int[] sort()
{
    int n = input.length;
    for (int i = 1; i < n; ++i) { // sorted part
        int key = input[i];
        int j = i - 1; // from 0 to j is sorted part

        while (j >= 0 && input[j] > key) {
            input[j + 1] = input[j];
            j = j - 1;
        }
        input[j + 1] = key;
    }
    return input;
}
```

### Merge Sort: O(nlogn)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/117edd22-70ff-4285-9913-86ba396755c5/Untitled.png)

![Screenshot 2023-03-07 at 12.03.49.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ae335dc6-1cfe-4f1d-94aa-e6889685642f/Screenshot_2023-03-07_at_12.03.49.png)

```java
public static void mergeSort(int[] array, int left, int right) {
    if (left < right) {
        int middle = (left + right) / 2;
        mergeSort(array, left, middle);
        mergeSort(array, middle + 1, right);
        merge(array, left, middle, right);
    }
}

public static void merge(int[] array, int left, int middle, int right) {
    int n1 = middle - left + 1;
    int n2 = right - middle;

    int[] leftArray = new int[n1];
    int[] rightArray = new int[n2];

    for (int i = 0; i < n1; ++i) {
        leftArray[i] = array[left + i];
    }
    for (int j = 0; j < n2; ++j) {
        rightArray[j] = array[middle + 1 + j];
    }

    int i = 0, j = 0;
    int k = left;
    while (i < n1 && j < n2) {
        if (leftArray[i] <= rightArray[j]) {
            array[k] = leftArray[i];
            i++;
        } else {
            array[k] = rightArray[j];
            j++;
        }
        k++;
    }

    while (i < n1) {
        array[k] = leftArray[i];
        i++;
        k++;
    }

    while (j < n2) {
        array[k] = rightArray[j];
        j++;
        k++;
    }
}
```

### Shell sort: O(n(logn)^2)

- Variation of insertion sort
- Divides the original list into smaller sublists
- Each sublist is sorted using insertion sort
- The sublists are combined using insertion sort
- The last iteration sorts the entire list using insertion sort
    - helps reduce complexity

```java
public static void shellSort(int[] array) {
    int n = array.length;

    for (int gap = n / 2; gap > 0; gap /= 2) {
        for (int i = gap; i < n; i += 1) {
            int temp = array[i];
            int j;
            for (j = i; j >= gap && array[j - gap] > temp; j -= gap) {
                array[j] = array[j - gap];
            }
            array[j] = temp;
        }
    }
}

```

### Quick sort: O(n^2)

- Based on the concept of divide-and-conquer, also known as partition-exchange sort
- Divide array into:
    1. Elements less than the pivot element
    2. Pivot element (central element)
    3. Elements greater than the pivot element.

```java
public static void quickSort(int[] array, int low, int high) {
    if (low < high) {
        int pivotIndex = partition(array, low, high);
        quickSort(array, low, pivotIndex - 1);
        quickSort(array, pivotIndex + 1, high);
    }
}

public static int partition(int[] array, int low, int high) {
    int pivot = array[high];
    int i = low - 1;
    for (int j = low; j < high; j++) {
        if (array[j] < pivot) {
            i++;
            int temp = array[i];
            array[i] = array[j];
            array[j] = temp;
        }
    }
    int temp = array[i + 1];
    array[i + 1] = array[high];
    array[high] = temp;
    return i + 1;
}
```

## Lecture 13: Trees and Search Trees

### Trees

- Implemented using the `TreeNode` class
- A tree is a non-linear data structure that consists of nodes connected by edges
- Height, depth of a node

![Screenshot 2023-03-07 at 14.49.24.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/eb815bd9-8992-4ce6-974b-4508d7232a2a/Screenshot_2023-03-07_at_14.49.24.png)

- A node have 1 parent and many children is an internal node
    - Except root node has no parent
        
    - Leaf, external node has no children
        
    - Sibling node
        
        ```java
        public class TreeNode {
            private int value;
            private TreeNode leftChild;
            private TreeNode rightChild;
        
            public TreeNode(int value) {
                this.value = value;
            }
        
            public void insert(int newValue) {
                if (newValue < this.value) {
                    if (leftChild == null) {
                        leftChild = new TreeNode(newValue);
                    } else {
                        leftChild.insert(newValue);
                    }
                } else {
                    if (rightChild == null) {
                        rightChild = new TreeNode(newValue);
                    } else {
                        rightChild.insert(newValue);
                    }
                }
            }
        }
        ```
        

### Binary Tree

- A tree but each node has at most 2 sub trees
- Level $d$ has at most $2^d$ nodes

![Screenshot 2023-03-07 at 15.12.11.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f41fafca-8322-4ea5-b2e2-121a2b27af62/Screenshot_2023-03-07_at_15.12.11.png)

![Screenshot 2023-03-07 at 15.10.28.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6237e741-7d1c-4cf1-9c8a-5eefbbc98cd7/Screenshot_2023-03-07_at_15.10.28.png)

- Full binary tree:
    - Every internal node has exactly two child or more
    - Number of leaf nodes = Number of internal nodes + 1
- Complete binary tree:
    - Every level possible is completely filled
    - All nodes are as far left as possible
- Perfect binary tree:
    - Full and complete
    - All internal nodes has 2 children and all leaf nodes are in the same level
- Balanced binary tree (Height-balanced tree or AVL tree):
    - The $T_L$’s height of any given node is 1 or less difference than its $T_R$’s height
- Degenerate binary tree:
    - Every parent nodes has only 1 child node
    - Height of tree = nb of nodes

### Set interface

- List interface are all indexed collections, while Set objects are not indexed
- Duplicate items are not allowed
- Removal of an object in Set does not require the shift of elements (unlike in ArrayList)

### SortedSet (implements Set)

### TreeSet (implements SortedSet extends AbstractSet)

<aside> 💡 `TreeSet‹Character> myTree = new TreeSet<> ();`

</aside>

- Duplicate items are not allowed
    
- Objects are stored in a sorted and ascending order
    
- Does not allow to insert heterogeneous objects
    
- Methods:
    
    - `add()`
    - `addAll()`
    - `remove()`
    - `headSet(Element e)`: returns values that are greater or equal than `e`
        - `headSet(Element e, bool false)`: returns values are greater than e only
    - `tailSet()`: returns values that are less or equal than `e`
    - `first()`
    - `last()`
    
    ```java
    TreeSet<Character> myTree = new TreeSet<Character> () ;
    myTree.add('B'); 
    myTree.add('Z'); 
    myTree.add('C'); 
    myTree.add('S'); 
    myTree.add('K');
    System.out.println(myTree); // [B, C, K, S, Z] automatically arrange
    System.out.printIn(myTree.tailSet('C')); //
    System.out.printIn(myTree.headSet('C'));
    myTree.add('W');
    myTree.remove ('Z');
    System.out.println(myTree.first ());
    System.out.println(myTree.last ());
    ```
    
    ```java
    public static <T> void printAll(TreeSet<T> set){
        for(T element : set){
            System.out.println(element);
        }
    }
    ```
    

### Binary Tree implementation

- Adding element
- Finding element:
- Delete element:

### Binary tree applications

- Mathematical: using binary tree to represent math expressions
    
    - The nodes are the operators
- Boolean:
    
    - (True or false) and not false

![Screenshot 2023-03-07 at 17.40.46.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/40602deb-21a6-48c0-bd37-f1c23021c793/Screenshot_2023-03-07_at_17.40.46.png)

- Huffman tree:
    - 0010100:
        - if 0 turn left, if 1 turn right until see a character and repeat

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/94ea0123-3c20-47e4-b4e8-cf0e2925da70/Untitled.png)

### Binary Search Trees

- Binary tree with ordered and sorted nodes
- Binary search trees are implemented using the `TreeSet` and `TreeMap` classes

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/80ade646-75ed-4bcc-9381-4e48060b3240/Untitled.png)

- Operation:
    - `Insert(E e`): Add an element to the BST by not violating the BST properties
    - `Delete(E e)`: Remove a given node from the BST. The node can be the root node, non-leaf, or leaf node. Search the location of the given element in the BST
    - `Search(E e)`: Checks if the tree contains the specified key.

```java
Set<String> names = new TreeSet<String>();
names.add("Alice");
names.add("Bob");
names.add("Charlie");

String first = names.first();
```

### Algorithm for searching a BST: O(n)

- if( left node and right node are null)
    - return notfound
- else if(search = node)
    - return node pos
- else if(search < node)
    - return recursive with leftnode
- else:
    - return recurve with rightnode

```java
class Node {
    int key;
    String name;

    Node leftChild;
    Node rightChild;

    Node(int key, String name) {
        this.key = key;
        this.name = name;
    }

    public String toString() {
        return name + " has the key " + key;
    }
}
public class BinaryTree {
    Node root;

    public void addNode(int key, String name) {
        Node newNode = new Node(key, name);
        if (root == null) {
            root = newNode;
        } else {
            Node focusNode = root;
            Node parent;
            while (true) {
                parent = focusNode;
                if (key < focusNode.key) {
                    focusNode = focusNode.leftChild;
                    if (focusNode == null) {
                        parent.leftChild = newNode;
                        return;
                    }
                } else {
                    focusNode = focusNode.rightChild;
                    if (focusNode == null) {
                        parent.rightChild = newNode;
                        return;
                    }
                }
            }
        }
    }

    public Node findNode(int key) {
        Node focusNode = root;
        while (focusNode.key != key) {
            if (key < focusNode.key) {
                focusNode = focusNode.leftChild;
            } else {
                focusNode = focusNode.rightChild;
            }
            if (focusNode == null)
                return null;
        }
        return focusNode;
    }

    public static void main(String[] args) {

        BinaryTree theTree = new BinaryTree();
        theTree.addNode(50, "Boss");
        System.out.println(theTree.findNode(75));
    }
}
```

## Lecture 14: Balanced Trees and Algorithms for Tree Traversal

### Balanced Trees ( height-balanced true) (AVL tree)

- Normal BST might become degenerate after inserting many items like 1,2,3,4,5 in order which hurts performance (from O(logn) to O(n))
    
- AVL is a self-balanced tree is a tree data structure in which the total left subtrees and right subtrees of any node differ in height by at most one
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7322c8c3-90df-454e-b50a-4834948e9ebb/Untitled.png)
    
    ![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/07af1947-fb7b-4182-b191-d65b13363007/Untitled.png)
    

### Red-black tree:

- An BST with rules:
    1. The root is black
    2. The children of a red node are black
    3. There are no two adjacent red nodes (A red node cannot have a red parent or red child)
    4. Every path from the root to a null node has the same number of black nodes.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cf46ae5b-2817-4c8d-a5ab-d144dcbd71ae/Untitled.png)

### Algorithms for Tree Traversal

- Tree traversal refers to the process of visiting each node in a tree data structure exactly once
- Tee traversal is implemented using recursion
- Includes:
    1. Preorder: visit root node first, traverse $𝑇_𝐿$, and traverse $T_R$
    2. Inorder: traverse $𝑇_𝐿$, visit root node, and traverse $𝑇_R$
    3. Postorder: traverse $𝑇_𝐿$, traverse $𝑇_R$, and visit root node last

```java
public void preorderTraverseTree(Node focusNode) {
    if (focusNode != null) {
        System.out.println(focusNode);
        preorderTraverseTree(focusNode.leftChild);
        preorderTraverseTree(focusNode.rightChild);
    }
}

public void inOrderTraverseTree(Node focusNode) {
    if (focusNode != null) {
        inOrderTraverseTree(focusNode.leftChild);
        System.out.println(focusNode);
        inOrderTraverseTree(focusNode.rightChild);
    }
}

public void postOrderTraverseTree(Node focusNode) {
    if (focusNode != null) {
        postOrderTraverseTree(focusNode.leftChild);
        postOrderTraverseTree(focusNode.rightChild);
        System.out.println(focusNode);
    }
}
```

## Lecture 15 & 16: Heaps and Priority Queues

### Binary heap

- A binary heap is a complete binary tree, meaning it is filled a equally as possible
    
- The root node of the heap is the maximum ( max heap) or minimum element (min heap)
    
- The value of each parent node is less than or equal to its child nodes
    
- Not necessarily a BST
    
- Every subtree is a heap
    
- Root element is at arr[0]
    
- For any `i`th root:
    
    - its parent is at index `(i-1)/2`
    - its left child is at `i*2+1`
    - its right child is at `i*2+2`

![Screenshot 2023-03-09 at 00.06.33.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/19c7458f-7a7c-48c8-a128-aa1045f7a46d/Screenshot_2023-03-09_at_00.06.33.png)

|0|1|2|3|4|
|---|---|---|---|---|
|20|26|58|22|38|

### Inserting an element E to a max heap

1. Insert to the next free index (if length(arr) is 8 then index for next element is 8)
2. While (index is not 0 and value > value of parent)
    1. Swap with the parent
    2. `heapify()`

### Removing root from the heap

- Swap the root with the last item in the heap (LIH), remove the LIH
- While item LIH has child, and item LIH is larger than either of its child
    - Swap item LIH with its smaller child
    - Heapify LIH down the heap.
- Until the heap property is restored

### Heapify()

- Initialize the root as largest, heapify down the tree

```java
void heapify(int root)
{
    int min = root;
    if(root*2+1 < numElem && array[root*2+1] < array[min])
    {
        min = root*2+1;
    }
    if(root*2+2 < numElem && array[root*2+2] < array[min])
    {
        min = root*2+2;
    }
    if(min != root)
    {
        Swap(root, min);
        heapify(min);
    }
}
```

### Building a heap from array

- To build a heap from array, find the position of the last non-leaf and perform heapify of each non-leaf upward direction

![Screenshot 2023-03-09 at 00.31.48.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4516f1da-1228-439d-8125-9d38b5554bb5/Screenshot_2023-03-09_at_00.31.48.png)

Last non leaf = Parent of last node = ((n-1)-1)/2

```java
static void buildHeap (int arr[], int n)
{
		int lastNonLeaf = (n / 2) - 1;
		for (int i = lastNonLeaf; i >= 0; i--) //heapify 39, 28, 20, 8, 18, 66
		{
				heapify(arr, n, i);
		}
}
```

### Implement heap with Priority Queues

- Priority queues are implemented using heap structure

```java
import java.uti1. Collections;
import java.util.PriorityQueue;

class HeapDemo3 
{
		static PriorityQueue‹Integer› maxHeap = new 
								PriorityQueue‹Integer›(); // minHeap
								PriorityQueue‹Integer›(Collections.reverseOrder ()); // maxHeap

		public static void printElements () {
				System.out.print("Max-Heap : ");
				for (Integer x : maxHeap) {
						System.out.print(x + " ");
				}
				System.out.println();
		}

		public static void main(String[] args) {
				maxHeap.add(19); 
				maxHeap.add (99);
				maxHeap.add (39); 
				maxHeap.add (49); 
				maxHeap.add (79); 
				maxHeap.add (69);
				printElements ();
				System.out.println("\\nAfter removing " + maxHeap.peek ());
				maxHeap.remove(maxHeap.peek ());
				printElements();
		}
}
```

### Heap sort algorithm: O(n log n)

- To sorts an array by first constructing a binary heap from its elements
    
- Then repeatedly extracts the highest (or lowest) element from the heap until the heap is empty
    
- Each extracted element is added to the sorted list
    
- The heap is re-built after each element is extracted
    
- Heap sort algorithm:
    
    - Build a heap
    - Repeat until the heap is empty
        - Heapify down the heap
        - Extract the root element (the largest/smallest element)
        - Replace with the last item in heap
    
    ```java
    public void sort(int arr[])
    {
        int n = arr.length;
        // Build heap (rearrange array)
        for (int i = n / 2 - 1; i >= 0; i--)
            heapify(arr, n, i);
        // One by one extract an element from heap
        for (int i = n - 1; i >= 0; i--) {
            // Move current root to end
            int temp = arr[0];
            arr[0] = arr[i];
            arr[i] = temp;
    
            // call max heapify on the reduced heap
            heapify(arr, i, 0);
        }
    }
    ```
    

---

## Lecture 17: Introduction to Graphs

### Graphs: $G=(V,E)$

- Collection of vertices (nodes) and edges (links) that connect pairs of vertices

![Screenshot 2023-03-10 at 00.38.22.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/40428e36-ac6f-4d46-8d23-ab3aff2d14b3/Screenshot_2023-03-10_at_00.38.22.png)

### Directed vs undirected graph

- Undirected graph
    
    - Edges have no direction
    
    ![Screenshot 2023-05-04 at 15.37.02.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fe734f83-4ee0-441b-aef2-266b98f29e09/Screenshot_2023-05-04_at_15.37.02.png)
    
    - An ordered pair $(u,v)$ where $u$ is adjacent (neighbourhood) to $v$ and vice versa
    - Degrees: number of neighbours a node have
    - Handshaking theorem: $2m=\sum\limits_{v\in V}{\text{deg} }(v)$
        - Sum of degrees is twice number of edges

![Screenshot 2023-05-04 at 20.24.54.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/85d45971-d3fc-4249-9715-dfd7204250f2/Screenshot_2023-05-04_at_20.24.54.png)

$\scriptsize V=\{a,b,c,d,e\}\\ E=\{(a,b),(a,d),(a,e),(b,b),(b,c)..\}\\ deg(a)=4, N (a)=\{b,d,e\}\\ deg(b)=6,N(b)=\{a,b,c,d,e\}$

- Directed graph (digraph):
    
    - Edges have direction
    
    ![Screenshot 2023-05-04 at 15.37.02.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fe734f83-4ee0-441b-aef2-266b98f29e09/Screenshot_2023-05-04_at_15.37.02.png)
    
    - An ordered pair $(u,v)$ where $u$ is source and $v$ is destination
    - Degrees: $|E|=\sum\limits_{v\in V}\text{deg}^-(v)=\sum\limits_{v\in V}\text{deg}^+(v)$
        - In-degree ($\text {deg}^-(v)$): nb of edges terminate at $v$
        - Out-degree ($\text{deg}^+(v)$): nb of edges start at $v$

![Screenshot 2023-05-04 at 20.05.58.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/575ba7fd-da64-45d3-b180-db9f114435bf/Screenshot_2023-05-04_at_20.05.58.png)

$\scriptsize V=\{0,1,2,3,4\}\\ E=\{(0,1),(1,2),(1,4),(2,3),(3,1)..\}\\ \text{deg}^-(3)=2, \text{deg}^+(3)=2$

### Complete graph

- $𝐾_𝑛$, is the simple graph that contains exactly one edge between each pair of distinct vertices

![Screenshot 2023-03-10 at 00.47.12.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/979789e6-f773-4a4f-80b7-1877435df2f6/Screenshot_2023-03-10_at_00.47.12.png)

### A cycle

- $C_n$ for $n\ge 3$ consists of n vertices $V=\{v_0, v_1,...,v_n\}$ and edges $E=\{(v_0,v_1),...,(v_{n-1},v_n)\}$

![Screenshot 2023-03-10 at 00.48.11.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cddc8736-ab4a-489b-b577-7664a73a8f45/Screenshot_2023-03-10_at_00.48.11.png)

- A cycle $C_n$ for $n\ge3$ consist of $n$ vertices and edges

![Screenshot 2023-05-04 at 22.52.28.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a41e6dea-9f08-419a-b2ea-2d95c7ccbf73/Screenshot_2023-05-04_at_22.52.28.png)

### Path and cycle

- A vertex is adjacent if there exists an edge to it (from other vertices)
    
- Path: a sequence of vertices in which each successive vertex is adjacent to its predecessor
    
    - Simple path: no repeated vertices
        
        ![Screenshot 2023-05-04 at 23.08.32.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/45aab37d-f287-4c99-9782-e901722f598e/Screenshot_2023-05-04_at_23.08.32.png)
        
    - Cycle: simple path but last vertex same as first for every vertices
        
        ![Screenshot 2023-05-04 at 23.11.23.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0647e9d5-134a-4873-9856-7160d4b34c0d/Screenshot_2023-05-04_at_23.11.23.png)
        

### Connected graph

- If there is a path in an undirected graph that connected every vertex to every other vertices
    
- Connected
    

![Screenshot 2023-05-04 at 23.26.44.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f594a8b8-5fca-4a41-8be6-1d7245ab2d07/Screenshot_2023-05-04_at_23.26.44.png)

![Screenshot 2023-05-04 at 23.25.23.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ae91d205-1317-4a45-9433-228b0f7edc31/Screenshot_2023-05-04_at_23.25.23.png)

### Directed Acyclic Graph (DAG):

- A DAG is a directed graph that has no cycle and with at least one node with no targets
    
- A directed graph can be DAG if it can be topologically ordered, by arranging the vertices as a linear ordering that is consistent with all edge direction
    
- Checking if a graph is a DAG:
    
    1. If the graph has no nodes, stop. The graph is acyclic
    2. If the graph has no leaf, stop. The graph is cyclic
    3. Choose a leaf of the graph. Remove this leaf and all arcs going into the leaf to get a new graph. Repeat
- No
    

![Screenshot 2023-05-04 at 23.38.27.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d0903466-9414-48bf-941c-d206afdbcf53/Screenshot_2023-05-04_at_23.38.27.png)

- Yes

![Screenshot 2023-05-04 at 23.30.25.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1b38a888-8b08-4b3a-b77e-326b8f7f7157/Screenshot_2023-05-04_at_23.30.25.png)

### Coloring

- Assignment of colors to the vertices of a graph that no two adjacent vertices have the same color
    - while minimize the number of colors (chromatic number)
- Method to color a graph (with vertices order decided):
    1. Choose the first vertex and color it with color 0
    2. Choose next vertex and color it with lowest numbered color that has not been colored on any vertices adjacent to it.
        1. If all adjacent vertices are colored with this color, assign new color
    3. Repeat step 3 until all vertices are colored

Chromatic number = 3

![Screenshot 2023-05-04 at 23.42.43.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/88e586c4-5382-4278-93d3-5d2f65f2de38/Screenshot_2023-05-04_at_23.42.43.png)

### Planar Graphs

- A graph that can be drawn on a plane without any edges crossing each other
- Kuratowski’s theorem: a graph is planar if and only if it doesn’t not contain a copy of $K_5$ or $K_{3,3}$

![Screenshot 2023-05-05 at 15.45.09.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ee573ec1-7791-4248-8bcc-c53138ded748/Screenshot_2023-05-05_at_15.45.09.png)

![Screenshot 2023-05-05 at 15.45.47.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5df42552-fab8-4fb1-baa9-1d0144732a01/Screenshot_2023-05-05_at_15.45.47.png)

### Bipartite Graphs

- A graph whose vertices can be colored only using 2 colors

![Screenshot 2023-05-05 at 16.26.25.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a4325a82-1716-4849-a9aa-a473ffd22323/Screenshot_2023-05-05_at_16.26.25.png)

- A complete bipartite graph $K_{m,n}$:
    - A graph that has its vertex set partitioned into two subsets $V_1$ (size m) and $V_2$(size n) such that there is every edge from $V_1$ to $V_2$

![Screenshot 2023-05-05 at 16.31.01.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/762d3fe6-c6c2-4b70-aabb-aa95118c223b/Screenshot_2023-05-05_at_16.31.01.png)

## Lecture 18: Graph presentation

### Adjacency matrix

- A square matrix used to represent a finite graph
- Is always symmetric for undirected graph

![Screenshot 2023-05-05 at 16.47.09.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0e1ab3bd-7e78-48e7-88ba-3d5449032fe9/Screenshot_2023-05-05_at_16.47.09.png)

$\displaystyle \text{Adj}[i][j]=\begin{cases} 1 &\text{if } (i,j)\in E \\ 0 &\text{else } \end{cases}$

### Adjacency list

- A representation of graph as an array of linked list, each linked list represents the list of vertices it can go to
- The edge between 2 vertices is denoted by a pointer from source vertex to destination vertex

![Screenshot 2023-05-05 at 16.54.57.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e79ac24e-3408-4ac0-bb4b-30ec99e75599/Screenshot_2023-05-05_at_16.54.57.png)

Null pointer if it is the last node

### Topological Sort

- The order of a DAG in such that for every directed edge `(u, v)`, node `u` comes before node `v` in the ordering
- Algorithm:
    1. Find a vertex with no incoming edge and put it in the final order
        1. Usually the one with lowest priority is chosen
    2. Delete all its out going edge
    3. Repeat 1 & 2
- There are many possible outcomes for a topological sort

![Screenshot 2023-05-09 at 23.29.46.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/92f17021-5589-4518-90c0-89746327b44a/Screenshot_2023-05-09_at_23.29.46.png)

![Screenshot 2023-05-09 at 23.29.55.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3e801805-b78b-4708-ae84-2d70af821f07/Screenshot_2023-05-09_at_23.29.55.png)

- Topological sorting can be used to find a valid sequence of tasks that must be completed in order to satisfy dependencies between them.

## Lecture 19: Shortest Path Algorithms

### Dijkstra's Algorithm: $O(n^2)$

- Used for finding shortest path in weighted directed and undirected graphs with non-negative weighted edges
- Algorithm:
    - An boolean array of unvisited nodes {F, T, …, T}
    - An array of cost for each vertex {0, inf,…, inf}
    - While unvisited vertices have T
        - Take the smallest cost vertex, update visited vertices set
        - examine each of its unvisited vertices
            - Calculate distance of each neighbor vertex from stat
            - if new distance less than in the cost, update it

### Spanning trees

- A subset of a connected graph that covers all vertices with minimum number of edges, number of vertices -1 , $|e'|=n-1$
    - There are more than 1 possible spanning tree, max $n^{n-2}$
- Has no cycle

![Screenshot 2023-05-10 at 12.19.30.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/920ded28-d44b-498e-9c60-333ae5036c25/Screenshot_2023-05-10_at_12.19.30.png)

![Screenshot 2023-05-10 at 12.19.58.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d95e39fa-24d2-494e-85d5-cb5ff64235d9/Screenshot_2023-05-10_at_12.19.58.png)

### Minimum spanning trees (SMT)

- A subset of a weighted graph with smallest weight combines from all edges
    - If all edges have distinct weight, there is only 1 possible MST

![Screenshot 2023-05-10 at 12.31.05.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/167dd6ed-4dd2-4039-b6f0-7e55f2d7a544/Screenshot_2023-05-10_at_12.31.05.png)

![Screenshot 2023-05-10 at 12.31.24.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e592f0f0-3041-4bcc-bccb-35998572a565/Screenshot_2023-05-10_at_12.31.24.png)

### Prim's Algorithm

- Greedy algorithm that finds the MST of a graph
- Algorithm:
    1. Create a boolean array to keep track of visited nodes and initialize all nodes as unvisited.
    2. Create an array to store the parent node for each node in the minimum spanning tree.
    3. Create an array to store the key (minimum weight) of each node and initialize all keys as positive infinity.
    4. Choose any node as the starting node (let's say node 0). Mark it as visited and set its key to 0.
    5. Repeat the following steps until all nodes are visited: a. From the set of unvisited nodes, choose the node with the minimum key value. b. Mark the chosen node as visited. c. Update the keys of adjacent unvisited nodes if their weight is smaller than the current key. d. Set the parent of each updated node as the chosen node.
    6. Build the minimum spanning tree using the parent array.
    7. Calculate the total cost of the minimum spanning tree.

### Kruskal's Algorithm O(E.logn)

- Greedy algorithm that finds the MST of a graph
- The algorithm starts by sorting the edges of the graph by weight. The algorithm then adds the edges with the smallest weight until all vertices are connected
- Algorithm:
    - Sort all the edges in non-decreasing order of the weights
    - Pick the smallest edge that doesnt form a cycle with the MST, include to MST, else remove
    - Repeat until there are n - 1 edges in mst

``` python
function Kruskal(Graph):
		Initialize an empty set of edges, MST
		Sort all the edges in the graph in non-decreasing order of their weights

		for each vertex v in Graph:
		    Create a new disjoint set with v as its representative

		for each edge (u, v) in sorted edges:
				// Check if u and v belong to different disjoint sets
		    if find(u) != find(v):  
		        Add (u, v) to MST
						
						// Merge the disjoint sets containing u and v		
		        Union(find(u), find(v))  
		return MST
```

## Lecture 21: Introduction to Hashing

### Hash table

- Efficient data structure that allows direct access by any index type
    - Like ,lookup table, dictionary with (key, value) pair
        - Key: index into hash table
        - Value: information being looked up
- Hashing algorithm: have many hashing functions

### Hash Functions

- Takes an input (or "key") and returns a fixed-size output (or "hash value") called bucket array

![Screenshot 2023-05-17 at 20.15.56.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/78ee6315-5935-4db7-a8f3-9e4c9a175796/Screenshot_2023-05-17_at_20.15.56.png)

![Screenshot 2023-05-17 at 20.19.38.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fe7ef64e-fd57-4c7b-8fb2-1c7cd7894314/Screenshot_2023-05-17_at_20.19.38.png)

### Collision:

- More than 1 key to map into a single index
    
- Choose better has function that distributes entries uniformly though out the hash table
    
- Solution:
    
    - Open hashing (separate chaining):
        - Keys with same hash code are linked by linked list from the first cell
            - Easy, wont overload, commonly used when not known the nb of keys and their frequency
            - Required linked list, can be unbalanced and need to search for item in linked list
    
    ![Screenshot 2023-05-17 at 20.23.27.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/eb61feed-a38d-46ea-a938-a5615e505df5/Screenshot_2023-05-17_at_20.23.27.png)
    
    - Close hashing (open addressing):
        
        - All keys are stored in the hash table in empty slot
        - Size of the table must be greater than or equal to nb of keys
        
        1. Linear Probing: if $\text{index}=\text{key} \ \% \ \text{prime}$ is occupied, assign to the next free index
        2. Quadratic Probing: if $\text{index}=\text{hash code}+i^2$, every fail $i+=1$
        3. Double Hashing:
            - $\#_1(key)=\text{key}\ \% \ n$
            - $\#_2(key)=\text{prime}-(key\% \text{prime})$
            - Double hash $=[\#_1(key)+ i.\#_2(key)]\ \% \ n$, every fail $i+= 1$
            - $n$ is table size and prime must be smaller than table size

## Lecture 22: Hashing and Maps in Java

### HashSet: (implements Set interface)

- Every element added is hashed so there is no particular order
- Doesn’t have any particular order
- HashSet uses HashMap for storing its object

![Screenshot 2023-06-03 at 13.49.13.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b541747d-ad0e-4531-93cc-1d5f633fbcb4/Screenshot_2023-06-03_at_13.49.13.png)

- $\displaystyle \text{Load Factor} = \frac{ \text{\# of stored entries in the table}}{\text{size of the has table}}$
    - Measures how full of the hashset tis allowed to get before its capacity is automatically increased

```java
Set<String> animals = new HashSet<>();
animals.add("Dog");
animals.add("Cat");
String[] otherNames = new String[];
animals.addAll(otherNames);
animals.remove("Dog");
// animals.remove(0) means remove element of value 0
animals.size();
animals.isEmpty();
animals.clear();
animals.contains("Dog") // return true or false
Iterator<String> i = names.iterator();
```

---

### Map

- Associative array: ordered pairs (by key) whose entries are known as key and value
- An object that maps keys to values
- Key must be unique, values can be duplicate
- HashMap: ordered of entries is based on hash codes
- LinkedHashMap: Preserves the insertion order
- TreeMap: sorted by the keys or comparator

```java
Map<Key,Value> M = new HashMap<K,V>();
```

![Screenshot 2023-06-03 at 13.50.08.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0bc19474-d327-4535-998b-76b91957b290/Screenshot_2023-06-03_at_13.50.08.png)

![Screenshot 2023-06-03 at 13.51.22.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5cc6fc47-855d-4d04-8e87-0db5505330ae/Screenshot_2023-06-03_at_13.51.22.png)

- Generic map in Java:
    - Entries in the map are indexed by keys
    - Methods:
        - size(): return number of entries in M
        - isEmpty():
        - get(k): return the value v of k, otherwise null
        - put(k,v): add entry if k is new, otherwise replace value v
        - remove(k)
        - keySet(): returns iterable collection contains all keys
        - values(): returns iterable collection contains all values (might contains repeated value)
        - entrySet(): return iterable collection contain all key-value

```java
// order based on hashcode
Map<String, Integer> myScore = new HashMap<String, Integer>();
// order based on insertion order
Map<String, Integer> myScore = new LinkedHashMap<String, Integer>();
// order based on sorted keys order
Map<String, Integer> myScore = new TreeMap<String, Integer>();
myScore.put("Midterm", 16); // Midterm maps to myScore.get("Midterm")
myScore.put("Final", 20);
myScore.put("Lab", 13);
myScore.put("Quiz", 9);

//loop over keys then search for values
for(String s : myScore.keySet())
{
		Integer score = myScore.get(s);
}

for(Map.Entry<String,Integer> entry : myScore.entrySet)
{
		System.out.println( entry.getKey() + " : " + entry.getValue());
}
```

### Bloom filtering:

- A space-efficient probabilistic data structure that tells whether an item maybe in the set or not in the set
- Uses many hash functions and set the element in the bucket to true
- The output might be false positive (it is not there but output said there might be) but never false negative (any element is 0 means it is not in the set)

![Screenshot 2023-06-03 at 14.46.33.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6084d41f-886f-406a-bc5d-baff3d2747f3/Screenshot_2023-06-03_at_14.46.33.png)

### Cuckoo hashing:

- Cuckoo hashing: a form of open addressing in which each non-empty cell of a hash table contains a key or key–value pair.
- Requires 2 hash functions and 2 hash table
- Hash1 the element and insert until there is conflict, replace in hash1 table and hash2 the original conflicting element, put in hash2 table. If there is conflict in hash2 table, replace it in hash2 table and hash1 the original conflicting element.
- wIf there is infinite loop, replace hashing function

---

## Breath first search BFS

- Keep a queue to keep track of nodes to visit
- If there is node from child, add

```java
// Breadth-First Search (BFS) pseudocode
void bfs(Node root) {
    if (root == null)
        return;

    Queue<Node> queue = new LinkedList<>();
    queue.add(root);
    while (!queue.isEmpty()) {
        Node current = queue.poll();
        System.out.print(current.data + " ");
        if (current.left != null)
            queue.add(current.left);
        if (current.right != null)
            queue.add(current.right);
    }
}
```

## Depth first search DFS

- Keep visiting children until there is none left

```java
// Depth-First Search (DFS) pseudocode
void dfs(Node node) {
    if (node == null)
        return;

    dfs(node.left);
    System.out.print(node.data + " ");
    dfs(node.right);
}
```