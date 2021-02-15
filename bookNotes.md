# Summary

### **Chapters**

- <a href="#chapter1">1 - Welcome to Java</a>
	+ <a href="#c1-comments">Comments</a>
	+ <a href="#c1-class-structure">Class structure</a>
		+ <a href="#c1-ordering-elements">Ordering elements in a class</a>
	+ <a href="#c1-main">Main method</a>
	+ <a href="#c1-javac-cli">Javac CLI</a>
		+ <a href="#c1-javac-options">Options you need to know for the exam</a>
	+ <a href="#c1-java-cli">Java CLI</a>
		+ <a href="#c1-possible-running">Possible ways of running programs</a>
		+ <a href="#c1-java-options">Options you need to know for the exam</a>
	+ <a href="#c1-jar-cli">Jar CLI</a>
		+ <a href="#c1-jar-options">Options you need to know for the exam</a>
	+ <a href="#c1-wildcards">Wildcards</a>
	+ <a href="#c1-redundant">Redundant Imports</a>
	+ <a href="#c1-conflict">Conflict Imports</a>
	+ <a href="#c1-formating">Code Formatting on the Exam</a>
	
- <a href="#chapter2">2 - Java Building Blocks
	+ <a href="#c2-creating-objects">Creating Objects & Constructors</a>
		+ <a href="#c2-reading-fields">Reading and Writing Member Fields</a> 
		+ <a href="#c2-initializer-block">Instance Initializer Blocks</a> 
			+ <a href="#c2-initializer-order">Following Order of Initialization</a> 
	+ <a href="#c2-understanding-data-types">Understanding Data Types</a> 
		+ <a href="#c2-primitive-types">Primitive Types</a> 
		+ <a href="#c2-short-char">Signed and Unsigned: short and char</a> 
		+ <a href="#c2-writing-literals">Writing literals</a>
			+ <a href="#c2-literals_underscore">Literals and the Underscore Character</a> 
		+ <a href="#c2-reference-types">Reference Types</a> 
			+ <a href="#c2-primitive-and-reference-types">Distinguishing between Primitives and Reference Types</a> 
	+ <a href="#c2-declaring-variables">Declaring Variables</a> 
		+ <a href="#c2-identifiers">Identifying Identifiers</a> 
		+ <a href="#c2-camel-snake-case">CamelCase and Snake-Case</a> 
		+ <a href="#c2-multiple-variables">Declaring Multiple Variables</a> 
		
	+ <a href="#c2-init-variables">Initializing Variables</a>
		+ <a href="#c2-local-variables">Creating Local Variables</a> 
		+ <a href="#c2-instance-class-variables">Defining Instance and Class Variables</a>   
		+ <a href="#c2-introduce-var">Introducing var</a>   
			+ <a href="#c2-inferences-var">Type Inference of var</a>  
			+ <a href="#c2-warnings-using-var">Things to keep in mind while using var (rules)</a>  
			+ <a href="#c2-var-and-null">var and null</a>  
			+ <a href="#c2-review-var-rules">Review of var Rules</a>  

## Intro

We'll be using [this Book](https://www.amazon.com/gp/product/B08DF4R2V9/ref=ppx_yo_dt_b_d_asin_title_o00?ie=UTF8&psc=1) to study to the certification.

---

<a id="chapter1"/></a>
## _Chapter 1:  Welcome to Java_ 
<a id="c1-comments"/></a>
### Comments: 
* Can be defined in 3 ways in Java

```java
1 - // comment until end of line

2 - /* Multiple
 * line comment
 */
 
3 - /**
 * Javadoc multiple-line comment
 * @author Jeanne and Scott
 */
```
PS: Comments can be defined anywhere in the code

-------
<a id="c1-class-structure"/></a>
###  Class structure
* You can put two classes in the same file. When you do so, at most one of the classes in the file is allowed to be public. If you do have a public class, it needs to match the filename.
* If one class is referring another that IS NOT at the same package, you should `import` specifying the package the class is
* If the class is referring another that IS in the same package, you don't need to `import` it

<a id="c1-ordering-elements"/></a>
#### Ordering elements in a class:

Element | Example | Required? | Where does it go? |
--- | --- | --- | ---
Package declaration | package abc; | No | First line in the file
Import statements | import java.util.* | No | Immediately after the package (if present)
Class declaration | public Class A | Yes | Immediately after the import (if any)
Field declarations | int value; | No | Any top-level element in a class
Method declarations | void method(); | No | Any top-level element in a class
 

-------
<a id="c1-main"/></a>
###  Main method
* The main() method lets the JVM call our code. If it doesn't have, the `java` CLI command will throw an error
* The base signature of main method is:
	
	```java
	// The "public static void main" part is mandatory and should be like this to be considered a main method
	public static void main(String[] args){}
	```	
	
	+ But there are 3 possible ways to change the array parameter
	
	```java
	String[] args
	String args[]
	String... args;
	
	//You can also change the parameter name
	String[] options
	String options []
	String... options;
	```

	+ The args you receive on main starts with 0, if you want to access the first param you should do `args[0]`
	
-------
<a id="c1-javac-cli"/></a>
### JAVAC CLI 
* You use to compile a `.java` file into `.class` file, so it run anywhere using JVM
	
```java
//Compiling one class
javac Zoo.java

//Compiling 2 classes in different packages (folders)
javac packagea/ClassA.java packageb/ClassB.java

//Compiling with Wildcards (It will compite all .java files in both packages)
javac packagea/*.java packageb/*.java
```
<a id="c1-javac-options"/></a>
#### Options you need to know for the exam:

Option | Description | 
--- | --- 
| -cp "classpath" <br/>  -classpath "casspath" <br/> --class-path "classpath" | Location of classes needed to compile the program

-------
<a id="c1-java-cli"/></a>
###  JAVA CLI
* You use to run a `.class` file. 
	
```java
//Example running "Zoo.class"
//You must omit the ".class" part
java Zoo part
```

* While passing parameters to `java` command, If you want an argument with a space to be recognized as one, use quotation marks

 ```java
java Zoo "One Parameter"
```
	
* In Java 11 We can run our java classes without actually having to compile it, This feature is called launching **single-file source-code programs**  (no `.class` files will be generated).
```java
//You must write the `.java` extension
java Zoo.java
```

-------
<a id="c1-possible-running"/></a>
#### Possible ways of running programs

Full Command | Single-file-source-code command | 
--- | --- 
javac HelloWorld.java <br/> java HelloWorld| java HelloWorld.java | 
Produces a class file | Fully in memory
For any program | For programs with one file
Can import code in any available Java library | Can only import code that came with the JDK

<a id="c1-XXX"/></a>
#### Options you need to know for the exam:

Option | Description | 
--- | --- 
| -cp "classpath" <br/>  -classpath "classpath" <br/> --class-path "classpath" | Location of classes needed to compile the program
| -d "dir" | Directory to place generated class files


-------
<a id="c1-jar-cli"/></a>
###  JAR CLI
* A Java archive (JAR) file is like a zip file of mainly Java class files.

* You can specify JAR files using the `cp` parameter
```java
//We can use a wildcard (*) to match all the JARs in a directory.
java -cp "C:\temp\directoryWithJars\*" myPackage.MyClass
```

* In addition to using JARs created by others, we can create our own, here's **you can create a JAR**

```java
jar -cvf myNewFile.jar .
jar --create --verbose --file myNewFile.jar .

//Alternatively, you can specify a directory instead of using the current directory.
jar -cvf myNewFile.jar -C dir .
```

<a id="c1-jar-options"/></a>
#### Options you need to know for the exam:

Option | Description | 
--- | --- 
| -c <br/> --create <br/>  | Creates a new JAR file
| -v <br/> --verbose <br/> | Prints details when working with JAR files
| -f "fileName" <br/> --file "fileName" <br/>  | JAR filename
| -C <br/>   					 | Directory containing files to be used to create the JAR

-------
<a id="c1-wildcards"/></a>
### Wildcards
* Classes in the same package are often imported together. You can use a shortcut to import all the classes in a package.

```java
 // imports java.util.Random among other things
import java.util.*;
//Every class in the java.util package is available to this program when Java compiles it.
```
* **==It doesn’t import child packages (is not recursive), fields, or methods;==** it imports only classes. (There is a special type of import called the static import that imports other types, which we’ll learn more about in Chapter 7.)

* Things you *CAN'T* do with WildCards, let's suppose we're trying to import `import java.nio.file.Files`:
```java
import java.nio.*;  // A wildcard only matches class names, not "file.Files"
 
import java.nio.*.*; // Can only have one wildcard and it must be at the end
 
import java.nio.file.Files.*; // You cannot import methods, only class names
```

-------
<a id="c1-redundant"/></a>
### Redundant Imports
* There’s one special package `java.lang`, this package is automatically imported **(we don't need to explicit import it)**. Inside this package we can find the `System` class for example

-------
<a id="c1-conflict"/></a>
### Conflict Imports
* You can face conflict imports when trying to import classes with the same name in different packages
	+ Ex: If you want to use the `Date` class and define 2 imports that have this class it will not compile
	
```java
//Will not compile, compiler doesn't know which date you wanna use
import java.util.*;
import java.sql.*; 

//Compiler still doesn't know which date you wanna use
import java.util.Date;
import java.sql.Date;
```


* There are 2 possible ways to solve it

```java
1 - Explicit declare the one you want to use
import java.util.Date; //Compiler will assume you want this one
import java.sql.*;

2 - Put the full package reference on the code you're using that class
java.sql.Date sqlDate;
```
-------
<a id="c1-formating"/></a>
### Code Formatting on the Exam
Not all questions will include package declarations and imports. Don’t worry about missing package statements or imports unless you are asked about them.

* The following are common cases where you don’t need to check the imports: 
	+ Code that begins with a class name 
	+ Code that begins with a method declaration 
	+ Code that begins with a code snippet that would normally be inside a class or method 
	+ Code that has line numbers that **don’t begin with 1**


<a id="chapter2"/></a>
## _Chapter 2:  Java Building Blocks_ 
<a id="c2-creating-objects"/></a>
### Creating Objects & Constructors: 
* *An object is an instance of a class.* To create an instance of a class, all you have to do is write new before the class name and add parentheses after it.

```java
Park p = new Park();
// "Park" is the class
// "p" is the object
```
First you declare the type that you’ll be creating **(Park)** and give the variable a name **(p)**. This gives Java a place to store a reference to the object. Then you write **new Park()** to actually create the object.

* **Park()** looks like a method since it is followed by parentheses. **It’s called a constructor**, which is a special type of method that creates a new object.We can create our own:

* The name of the constructor matches the name of the class, and there’s no return type.

* We usually use constructor to initialize fields but you can also do it where you declare the fields

```java
//Valid constructor
public class Chick {
	int numEggs = 12;  // initialize on line
	String name;

   public Chick() {
		name = "Duke";  // initialize in constructor
   }
}

//Invalid constructor (has return type)
public void Chick() { }  // NOT A CONSTRUCTOR
```

If the class doesn't have a constructor, the compiler will supply a “do nothing” default constructor.

<a id="c2-reading-fields"/></a>
### Reading and Writing Member Fields
* We can read and write instance variables directly from the caller.

```java
public class Swan {
   int numberEggs;                            // instance variable
   int plusEggs = numberEggs + 1;             // It's also possible
   public static void main(String[] args) {
      Swan mother = new Swan();
      mother.numberEggs = 1;                  // set variable (setting)
      System.out.println(mother.numberEggs);  // read variable (getting)
   }
}
```
<a id="c2-initializer-blocks"/></a>
### Instance Initializer Blocks
* When we're writing code, we usually see braces (`{}`), code between braces is called a `code block`, so if you see braces, the code between them is a `code block`. Code block can be:
	+ Inside a method: These are run when the method is called
	+ Outside a method: These are called **instance initializers**, they are not attached to a method and are run in the order in which they appear in the file.	 

```java
//In this code we have 4 code blocks and only ONE instance initializer
1: public class Bird { //Code-block
2:    public static void main(String[] args) {//Code-block
3:       { System.out.println("Feathers"); } //Codeblock (Inner): NOT instance initializer
4:    }
5:    { System.out.println("Snowy"); } //*Codeblock: Instance initializer*
6: }
```
<a id="c2-initializer-order"/></a>
#### Following Order of Initialization
* We can write a code that initialize fields in multiple places, so we need to pay attention to the order of initialization rules
	+ Fields and instance initializer blocks are run in the order in which they appear in the file.
	+ The constructor runs after all fields and instance initializer blocks have run.

```java
1:  public class Chick {
2:     private String name = "Fluffy";
3:     { System.out.println("setting field"); }
4:     public Chick() {
5:        name = "Tiny";
6:        System.out.println("setting constructor");
7:     }
8:     public static void main(String[] args) {
9:        Chick chick = new Chick();
10:       System.out.println(chick.name); 
11:    } 
12:}

//Output (in Order)
setting field
setting constructor
Tiny
```

* Order matters for the fields and blocks of code. You can’t refer to a variable before it has been defined:

```java
{ System.out.println(name); }  // DOES NOT COMPILE
private String name = "Fluffy";
```

<a id="c2-understanding-data-types"/></a>
### Understanding Data Types
* In java we have two types of data
	+ **Reference types:** refers to an object (an instance of a class). A reference “points” to an object by storing the memory address where the object is located, a concept referred to as a pointer.
	+ **Primitive Types:** A primitive is just a single value in memory, such as a number or character. A primitive is not an object in Java nor does it represent an object. 
	
<a id="c2-primitive-types"/></a>
#### The primitive types
* Java has eight built-in primitive types. These eight data types represent the building blocks for Java objects, because all Java objects are just a complex collection of these primitive data types.

Keyword | Type | Example
--- | --- | ---
| boolean | true or false | true
| byte | 8-bit integral value | 123
| short | 16-bit integral value | 123
| int | 32-bit integral value | 123
| long | 64-bit integral value | 123L
| float | 32-bit floating-point value | 123.25F
| double | 64-bit floating-point value | 123.456
| char | 16-bit Unicode value | 'a'

-> **PS I**: **String** *IS NOT* a Primitive =) 
-> **PS II**: You won’t be asked about the exact sizes of most of these types, although you should know that a byte can hold a value from –128 to 127.

* Some notes about this table:
	+ Each numeric type uses twice as many bits as the smaller similar type. For example, short uses twice as many bits as byte does.
	+ All of the numeric types are signed in Java. This means that they reserve one of their bits to cover a negative range. For example, byte ranges from -128 to 127. Don’t forget, 0 needs to be accounted for too in the range.

<a id="c2-short-char"/></a>
#### Signed and Unsigned: short and char
* Short and Char are closely related, as both are stored as integral types with the same 16-bit length.
	+ The primary difference is that short is signed, which means it splits its range across the positive and negative integers.
	+ char is unsigned, which means range is strictly positive including 0. 
	+ char can hold a higher positive numeric value than short, but cannot hold any negative numbers.

* A **byte is 8 bits**. A bit has two possible values. (These are basic computer science definitions that you should memorize.) 
*2^8* = `2 × 2 = 4 × 2 = 8 × 2 = 16 × 2 = 32 × 2 = 64 × 2 = 128 × 2 = 256`. 
Since 0 needs to be included in the range, Java takes it away from the positive side. Or if you don’t like math, you can just memorize it.

* Floating-point values like double and float are not easy to calculate but don’t worry, for the exam you are not required to know how floating-point values are stored.

<a id="c2-writing-literals"/></a>
#### Writing literals
* When a number is present in the code, it is called a literal. By default, Java assumes you are defining an int value with a numeric literal.
 
 ```java
 long max = 3123456789;  // DOES NOT COMPILE (Java complains the number is out of range.
//However, we don’t have an int. The solution is to add the character L to the number:
long max = 3123456789L;  // now Java knows it is a long
 ```
 
 * We can specify number change the base, the default in java is 0-9 but java allow you to use:
 
Base | Digits| Description | Example | Obs
------- | ------- | ------- | ------- | -------
Octal | 0 - 7 | uses the number 0 as a prefix | 017
Hexadecimal | 0 - 9 and letter A-F/a-f | uses 0x or 0X as a prefix | 0xFF, 0xff, 0XFf | case insensitive, so all examples mean the same value.
Binary | 0 - 1 | uses the number 0 followed by b or B as a prefix | 0b10, 0B10 | case insensitive, so all examples mean the same value.

* Exam tip: We won’t need to convert between number systems on the exam. You’ll have to **recognize valid literal values that can be assigned to numbers.**

<a id="c2-literals_underscore"/></a>
#### Literals and the Underscore Character
* We can have underscores in literal numbers to make them easier to read: `int million2 = 1_000_000;`

* We can add underscores anywhere expect in some places
	
	```java
	//Can't (DOES NOT COMPILE)
	double notAtStart = _1000.00;          // Beginning of a literal
	double notAtEnd = 1000.00_;            // End of a literal
	double notByDecimalBefore = 1000_.00;  // Right before decimal point
	double notByDecimalAfter = 1000._00;   // Right after decimal point

	//Can
	double annoyingButLegal = 1_00_0.0_0;  // Ugly, but compiles
	double reallyUgly = 1__________2;      // Also compiles (you can place multiple underscore characters)
	```

<a id="c2-reference-types"/></a>
### Reference Types
* A reference type refers to an object (an instance of a class). Unlike primitive types that hold their values in the memory where the variable is allocated, references do not hold the value of the object they refer to.

* Examples that declare and initialize reference types.

```java
////variable is a reference of type Date and can only point to a Date object.
java.util.Date today; 

//variable is a reference that can only point to a String object.
String greeting; 
```

* A value is assigned to a reference in one of two ways:

```java
// 1 - A reference can be assigned to a new object using the new keyword.
java.util.Date today = new java.util.Date();
// It will create a new object in memory and assign the "pointer" to our variable


// 2 - A reference can be assigned to another object of the same or compatible type.
java.util.Date randomDate = new java.util.Date();
java.util.Date today = randomDate;
//Here we have 2 references pointing to the same object
```

<a id="c2-primitive-and-reference-types"/></a>
#### Distinguishing between Primitives and Reference Types

Differences | Reference Type | Primitive Type
------- | ------- | -------
Can assign to null | Yes | No
Can be used to call methods | Yes | No
Lower / Upper Case | All classes that come with Java begin with uppercase.</br> Not required but standard for new classes | Have lowercase type names

**PS**: You only call methods from Reference Type assuming the reference is not null, otherwise you'll face a `NullPointer`

```java
int value = null;   // DOES NOT COMPILE (can't assign primitive to null)
String s = null;

4: String reference = "hello";
5: int len = reference.length();
6: int bad = len.length(); // DOES NOT COMPILE (primitive doesn't have methods)
```

<a id="c2-declaring-variables"/></a>
### Declaring Variables
* You can declare variable and assign a value to it, it's called *initializing variables*, it can be done in 2 ways:

```java
// Initialize at a latter point after declaring it
5: zooName = "The Best Zoo";
6: numberAnimals = 100;

// Initialize in the same statement as the declaration.
1: String zooName = "The Best Zoo";
2: int numberAnimals = 100;
```

<a id="c2-identifiers"/></a>
#### Identifying Identifiers
* Java has precise rules about identifier names. An *identifier is the name* of a `variable`, `method`, `class`, `interface`, or `package`. Java has precise rules about identifier names, the rules for variables apply to all of the other types that you are free to name. </br> There are only four rules to remember for legal identifiers:
	+ Identifiers **must begin** with a letter, a $ symbol, or a _ symbol.
	+ Identifiers **can include** numbers but not start with them.
	+ Since Java 9, a single underscore _ is **not allowed** as an identifier.
	+ You **cannot use** the same name as a Java reserved word. A reserved word is special word that Java has held aside so that you are not allowed to use it. </br> **PS:** Java is case sensitive, you can use keywords versions that differ in case.

	We **won’t need to memorize** the full list of reserved words. The exam will only ask you about ones that are commonly used, such as `class` and `for`.</br> (Check the `Table 2.2` on original book to see all reserved words)
	
	```java
	//The following examples are legal: 
	long okidentifier;
	float $OK2Identifier;
	boolean _alsoOK1d3ntifi3r;
	char __SStillOkbutKnotsonice$; 
	
	//These examples are NOT legal: 
	int 3DPointClass;    // identifiers cannot begin with a number
	byte hollywood@vine; // @ is not a letter, digit, $ or _
	String *$coffee;     // * is not a letter, digit, $ or _
	double public;       // public is a reserved word
	short _;             // a single underscore is not allowed
	```
	
	**Exame Tip**: 
	> var is not a reserved word, just a reserved type. It can be used as an identifier except as a class, interface, or enum name.
	
<a id="c2-camel-snake-case"/></a>
#### Styles: CamelCase and Snake-Case 
* Camel Case: The first letter of each word is capitalized.
	+ Method and variable names are written in camelCase with the first letter being lowercase. 
	+ Class and interface names are written in camelCase with the first letter being uppercase. Also, don’t start any class name with $, as the compiler uses this symbol for some files.
* Snake Case: Uses an underscore (_) to separate words, often entirely in lowercase.
	+ Static final values and ENUM values tend to be written with snake_case

<a id="c2-multiple-variables"/></a>
#### Declaring Multiple Variables
* You can also declare and initialize multiple variables in the same statement.
	+ Declare: When you define the variable (**without assign** a value to it)
	+ Initialize: When you assign a value to it

```java
//Declaring 4 variables AND Initializing 2 variables
   String s1, s2;
   String s3 = "yes", s4 = "no";
```

* Things to keep in mind while declaring / initializing multiple variables

```java
1 - //Each snippet separated by a comma is a little declaration of its own
int i1, i2, i3 = 0;
//Three variables were declared BUT the initialization of i3 only applies to i3. It doesn’t have anything to do with i1 or i2 despite being in the same statement.


2 - // The shortcut to declare multiple variables in the same statement is legal only when they share a type.
int num, String value; // DOES NOT COMPILE
```

* Examples

```java
4: boolean b1, b2; // LEGAL
5: String s1 = "1", s2; //LEGAL
6: double d1, double d2; //ILEGAL: If you want to declare multiple variables in the same statement, they must share the same type declaration and not repeat it.
7: int i1; int i2; // LEGAL
8: int i3; i4; // ILEGAL: Missing i4 type, since we have ";" it's a completely different statement
```

<a id="c2-init-variables"/></a>
### Initializing Variables
* Before you can use a variable, it needs a value. Some types of variables get this value set automatically, and others require the programmer to specify it.

<a id="c2-local-variables"/></a>
#### Creating Local Variables
• A **local variable** is a variable defined within a constructor, method, or initializer block. Local variables *do not have a default value* and must be initialized before use.
```java
4: public int notValid() {
5:    int y = 10; // Initializing
6:    int x;      // Not Initializing
7:    int reply = x + y; // DOES NOT COMPILE (because we didn't initialize x)
8:    return reply;
9: }

//Compiler error:
Test.java:7: variable x might not have been initialized
```

* The important thing is initialize the variable before using it, you can do it when declaring or doing it in a latter point in the code. 

* If there's a flow where the variable can be used without being initialized, the compiler will identify it

```java
public void testMethod(boolean checkValue){
	int checkValue;
	if(checkValue) {
		checkValue = 1;
	}
	
	System.out.println(checkValue); //DOES NOT COMPILE

	// Compile identifies there's a flow that the variable might not be initialized (if the code does not enter the if)
}
```

* Initialization rules also apply to constructors and methods. In other words, they are like local variables and need to initialized before the method/constructor is called using them as parameters.

```java
public void test() {
   int answer;
   anotherMethod(answer);  // DOES NOT COMPILE (var not initilized)
}
```

**Exame Tip**: 
> Be wary of any local variable that is declared but not initialized in a single line. This is a common place on the exam that could result in a “Does not compile” answer. You are not required to initialize the variable on the same line it is defined, but be sure to check to make sure it’s initialized before it’s used on the exam.

<a id="c2-instance-class-variables"/></a>
#### Defining Instance and Class Variables
* Variables that are not local variables are defined either as instance variables or as class variables.


Variable | Value | Example
------- | ------- | -------
Instance | Defined within a specific instance of an Object</br>Each instance can have different values on the "same" attribute | String name;
Class    | Defined on the class level and shared among all instances of the class.</br>They're part of the class, not the instance. All instances will have the same value for that attribute | **static** String name;

A variable is a class variable if it has the static keyword in its declaration.

* Instance and class variables *do not require you to initialize them*. As soon as you declare these variables, they *are given a default value*.

**Exame Tip**: 
> You’ll need to memorize everything in this table except the default value of char.

Variable Type | Default initialization value
------- | -------
boolean | false
byte, short, int, long | 0
float, double | 0.0
char | '\u0000' (NUL)
All object references (everything else) | null

<a id="c2-introduce-var"/></a>
#### Introducing var
* Starting in Java 10, you have the option of using the keyword var instead of the type for local variables under certain conditions. </br>The formal name of this feature is **local variable type inference**.

> You can only use this feature for **local variables**.

```java
public class VarKeyword {
	//Does not work for instance variables
   var tricky = "Hello"; // DOES NOT COMPILE
   
   public void myMethod(){
   	//Works fine because they're local variables
   	var myVariable = "Mine";
   	var mySecondVariable = 2;
   }
}

```

<a id="c2-inferences-var"/></a>
#### Type Inference of var
* Java will inference the variable type based on the variable value **BUT** the type of var can’t change at runtime, ex:

```java
7:  public void reassignment() {
8:     var number = 1;
9:     number = 2;
10:    number = "tree";  // DOES NOT COMPILE
11: }
```

* Another example

```java
var apples = (short)10;
// byte can be automatically promoted to a short, because a byte is small enough that it can fit inside of short.
apples = (byte)5;

// One million is well beyond the limits of short.
// The compiler treats the value as an int (we're changing the type)
apples = 1_000_000;  // DOES NOT COMPILE
```

We’ll cover numeric promotion and casting in Chapter 3
> For now, we just need to know that the value for a var can change after it is declared but the type never does.

<a id="c2-warnings-using-var"/></a>
#### Things to keep in mind while using var (rules)
* While declaring a var you **and MUST initialize** it in the same line

```java
// DOES NOT COMPLITE
var size;
size = 1;

// COMPILES
var size = 1;

// Line breaks are considered to be on the same line (as long we don't have ";")
var size
	= 2;
```

* Java does **NOT allow var** in multiple variable declarations.

```java
var a = 2, b = 3;  // DOES NOT COMPILE
```
The multiple variable declarations *syntax is right* considered what we saw in the past, *but var is not allowed* to do it.

* Java does **NOT allow var** to infer the type of `null`. **It's allowed ONLY IF** you specify the Type

```java
var n = null;         // DOES NOT COMPILE

var n = (String)null; //COMPILES
```
Java creators didn't allow only `null` because it could be any reference type (object).

* Java does **NOT allow var** in: `method parameters` (signature), `constructors` (signature), `instance variables` and `class variables` *because they're NOT LOCAL variables*.

```java
public int addition(var a, var b) {  // DOES NOT COMPILE
   return a + b;
}
```

<a id="c2-var-and-null"/></a>
#### var and null
* While a var cannot be initialized with a null value without a type, it can be assigned a null value after it is declared

```java
//String can be null so we're not changing types, and we can assign null because compiler knows we're dealing with a String
var a = "myData";
a = null; //COMPILES

// We can't assign to null because compiler knows we're dealing with a primitive (int), and primitives cannot point to null
var b = 4;
b = null;  // DOES NOT COMPILE
```

<a id="c2-review-var-rules"/></a>
#### Review of var Rules
* A var is used as a local variable in a constructor, method, or initializer block. 
* A var cannot be used in constructor parameters, method parameters, instance variables, or class variables. 
* A var is always initialized on the same line (or statement) where it is declared. 
* The value of a var can change, but the type cannot. 
* A var cannot be initialized with a null value without a type. 
* A var is not permitted in a multiple-variable declaration. 
* A var is a reserved type name but not a reserved word, meaning it can be used as an identifier except as a class, interface, or enum name.

**Exame Tip**:
> Since var is new to Java since the last exam, expect to see it used frequently on the exam.



