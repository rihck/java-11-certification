# Summary

### **Chapters**

- <a href="#chapter1">1 - Welcome to Java</a>
	+ <a href="#c1-comments">Access modifiers</a>
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
	
	+ <a href="#c2-managing-var-scope">Managing Variable Scope</a>
		+  <a href="#c2-limiting-var-scope">Limiting, Nesting and Tracing Scope</a>
		+  <a href="#c2-apply-var-scope-class">Applying Scope to Classes</a>
		+  <a href="#c2-reviewing-var-scope">Reviewing Scope</a>

	+  <a href="#c2-destroying-objects">Destroying Objects</a>
		+  <a href="#c2-garbage-collection">Understanding Garbage Collection</a>
		+  <a href="#c2-eligible-garbage-collection">Eligible for Garbage Collection</a>
		+  <a href="#c2-calling-gc">Calling System.gc()</a>
		+  <a href="#c2-tracing-eligibility">Tracing Eligibility</a>
		+  <a href="#c2-objects-and-references">Objects vs. References</a>
		+  <a href="#c2-gc-finalize">Calling finalize()</a>

- <a href="#chapter3">3 - Operators
	+  <a href="#c3-operators">Understanding Java Operators</a>
		+  <a href="#c3-operator-procedence">Order of operator precedence</a>
	
	+  <a href="#c3-applying-op">Applying Unary Operators</a>
		+  <a href="#c3-increment-decrement">Increment and Decrement Operators</a>
		
	+  <a href="#c3-binary-operators">Working with Binary Arithmetic Operators</a>
		+  <a href="#c3-adding-parentheses">Adding Parentheses</a>
		+  <a href="#c3-division-module-operators">Division and Modulus Operators</a>
		+  <a href="#c3-numeric-promotion">Numeric Promotion</a>
	
	+  <a href="#c3-assigning-values">Assigning Values</a>
		+  <a href="#c3-casting-values">Casting Values</a>
		+  <a href="#c3-reviewing-primitive">Reviewing Primitive Assignments</a>
		+  <a href="#c3-compound-assignment">Compound Assignment Operators</a>
		+  <a href="#c3-assignment-operator-return">Assignment Operator Return Value</a>
		
	+  <a href="#c3-comparing-values">Comparing Values</a>
		+  <a href="#c3-equality-operators">Equality Operators</a>
		+  <a href="#c3-relational-operators">Relational Operators</a>
		+  <a href="#c3-instanceof-operator">instaceof Operator</a>
		+  <a href="#c3-logical-operator">Logical Operators</a>
		+  <a href="#c3-short-circuit-operators">Short-Circuit Operators</a>
		+  <a href="#c3-ternary-operators">Ternary Operator</a>


- <a href="#chapter4">4 - Making Decisions
	+  <a href="#c4-creation-decision">Creating Decision-Making Statements</a>
		+ <a href="#c4-if-statement">The if Statement</a>  
		+ <a href="#c4-else-statement">The else Statement</a>
		+ <a href="#c4-switch-statement">The switch Statement</a>
	
	+ <a href="#c4-writing-while-loops">Writing while Loops</a>
		+ <a href="#c4-while-statement">While statement</a>
		+ <a href="#c4-do-while-statement">The do/while Statement</a>
		
	+ <a href="#c4-cont-for-loops">Constructing for Loops</a>
		+ <a href="#c4-for-loops">The for Loop</a>
		+ <a href="#c4-scenarios-using-loops">Scenarios while using for loop</a>
		+ <a href="#c4-for-each-loop">The for-each Loop</a>
		
	+ <a href="#c4-flow-with-branching">Controlling Flow with Branching</a>
		+ <a href="#c4-nested-loops">Nested Loops</a>
		+ <a href="#c4-optional-labels">Adding Optional Labels</a>
		+ <a href="#c4-break-statement">The break Statement</a>
		+ <a href="#c4-continue-statement">The continue Statement</a>
		+ <a href="#c4-return-statement">The return Statement</a>
		+ <a href="#c4-unreachable-code">Unreachable Code</a>
		+ <a href="#c4-reviewing-branching">Reviewing Branching</a>

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

---
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
 

---
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
	
---
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

---
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

---
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
| -cp "classpath" <br/>  -classpath "classpath" <br/> --class-path "classpath" | Location of classes needed to compile the program (**folders where your classes are located**)
| -d "dir" | Directory to place generated class files


---
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

---
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

---
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

---
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
* *An object is an instance of a class.* To create an instance of a class, all you have to do is write new before the class name and add parentheses after it. Ex:
	+ First you declare the type that you’ll be creating `Park` 
	+ Give the variable a name `p`. This gives Java a place to store a reference to the object. 
	+ Then you write `new Park()` to actually create the object.
	
```java
Park p = new Park();
// "Park" is the class
// "p" is the object
```

* Some Notes
	+ `Park()` looks like a method since it is followed by parentheses. **It’s called a constructor**, which is a special type of method that creates a new object. We can create our own.
	+ The name of the constructor matches the *name of the class, and there’s no return type*.
	+ We usually use constructor to initialize fields but you can also do it where you declare the fields

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

> If the class doesn't have a constructor, the compiler will supply a “do nothing” default constructor.

---
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

---
<a id="c2-initializer-blocks"/></a>
### Instance Initializer Blocks
* When we're writing code, we usually see braces (`{}`), code between braces is called a `code block`, so if you see braces, the code between them is a `code block`. Code block can be:
	+ *Inside a method:* These are run when the method is called
	+ *Outside a method:* These are called **instance initializers**, they are not attached to a method and are run in the order in which they appear in the file.	 

```java
//In this code we have 4 code blocks and only ONE instance initializer
1: public class Bird { //Code-block
2:    public static void main(String[] args) {//Code-block
3:       { System.out.println("Feathers"); } //Codeblock (Inner): NOT instance initializer
4:    }
5:    { System.out.println("Snowy"); } //*Codeblock: Instance initializer*
6: }
```

---
<a id="c2-initializer-order"/></a>
#### Following Order of Initialization
* We can write a code that initialize fields in multiple places, so we need to pay attention to the order of initialization rules
	+ *Fields and instance initializer blocks* are run in the order in which they appear in the file.
	+ *The constructor* runs after all fields and instance initializer blocks have run.

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

---
<a id="c2-understanding-data-types"/></a>
### Understanding Data Types
* In java we have two types of data
	+ **Reference types:** refers to an object (an instance of a class). A reference “points” to an object by storing the memory address where the object is located, a concept referred to as a pointer.
	+ **Primitive Types:** A primitive is just a single value in memory, such as a number or character. A primitive is not an object in Java nor does it represent an object. 
	
---
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

**PS**: **String** *IS NOT* a Primitive :no_entry_sign:

:bangbang: **Exam Tip:**
> You won’t be asked about the exact sizes of most of these types, although you should know that a byte can hold a value from –128 to 127.

* Some notes about this table:
	+ Each numeric type uses twice as many bits as the smaller similar type. For example, short uses twice as many bits as byte does.
	+ All of the numeric types are signed in Java. This means that they reserve one of their bits to cover a negative range. For example, byte ranges from -128 to 127. Don’t forget, 0 needs to be accounted for too in the range.

---
<a id="c2-short-char"/></a>
#### Signed and Unsigned: short and char
* Short and Char are closely related, as both are stored as integral types with the same 16-bit length.
	+ The primary difference is that short is signed, which means it splits its range across the positive and negative integers.
	+ char is unsigned, which means range is strictly positive including 0. 
	+ char can hold a higher positive numeric value than short, but cannot hold any negative numbers.

* A **byte is 8 bits**. A bit has two possible values. (These are basic computer science definitions that you should memorize.) 
```java
2^8 = 2 × 2 = 4 × 2 = 8 × 2 = 16 × 2 = 32 × 2 = 64 × 2 = 128 × 2 = 256 
```
Since 0 needs to be included in the range, Java takes it away from the positive side. Or if you don’t like math, you can just memorize it.

* Floating-point values like double and float are not easy to calculate but don’t worry, for the exam you are not required to know how floating-point values are stored.

---
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

:bangbang: **Exam Tip:**
> We won’t need to convert between number systems on the exam. You’ll have to *recognize valid literal values that can be assigned to numbers.*

---
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

---
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

---
<a id="c2-primitive-and-reference-types"/></a>
#### Distinguishing between Primitives and Reference Types

? | Reference Type | Primitive Type
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
* Java has precise rules about identifier names. An *identifier is the name* of a `variable`, `method`, `class`, `interface`, or `package`. Java has precise rules about identifier names, the rules for variables apply to all of the other types that you are free to name.
* There are only four rules to remember for legal identifiers:
	+ Identifiers **must begin** with a letter, a $ symbol, or a _ symbol.
	+ Identifiers **can include** numbers but not start with them.
	+ Since Java 9, a *single* underscore _ is **not allowed** as an identifier.
	+ You **cannot use** the same name as a Java reserved word. A reserved word is special word that Java has held aside so that you are not allowed to use it. </br> **PS:** Java is case sensitive, you can use keywords versions that differ in case.

	We **won’t need to memorize** the full list of reserved words. The exam will only ask you about ones that are commonly used, such as `class` and `for`.</br> (Check the `Table 2.2` on original book to see all reserved words)
	
	```java
	//The following examples are legal: 
	long okidentifier;
	float $OK2Identifier;
	boolean _alsoOK1d3ntifi3r;
	char __SStillOkbutKnotsonice$;
	int var; 
	
	//These examples are NOT legal: 
	int 3DPointClass;    // identifiers cannot begin with a number
	byte hollywood@vine; // @ is not a letter, digit, $ or _
	String *$coffee;     // * is not a letter, digit, $ or _
	double public;       // public is a reserved word
	short _;             // a single underscore is not allowed
	```
	
:bangbang: **Exam Tip:**
> var is not a reserved word, just a reserved type. It can be used as an identifier except as a class, interface, or enum name.
	
---
<a id="c2-camel-snake-case"/></a>
#### Styles: CamelCase and Snake-Case 
* *Camel Case*: The first letter of each word is capitalized.
	+ Method and variable names are written in camelCase with the first letter being lowercase. 
	+ Class and interface names are written in camelCase with the first letter being uppercase. Also, don’t start any class name with $, as the compiler uses this symbol for some files.
* *Snake Case*: Uses an underscore (_) to separate words, often entirely in lowercase.
	+ Static final values and ENUM values tend to be written with snake_case

---
<a id="c2-multiple-variables"/></a>
#### Declaring Multiple Variables
* You can also declare and initialize multiple variables in the same statement.
	+ **Declare**: When you define the variable (**without assign** a value to it)
	+ **Initialize**: When you assign a value to it

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
//LEGAL
4: boolean b1, b2;
5: String s1 = "1", s2;
6: int i1; int i2;

//ILEGAL
7: double d1, double d2; //If you want to declare multiple variables in the same statement, they must share the same type declaration and not repeat it.

8: int i3; i4; // Missing i4 type, since we have ";" it's a completely different statement
```

---
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
	// Compiler identifies there's a flow that the variable might not be initialized (if the code does not enter the if)
}
```

* Initialization rules also apply to constructors and methods. In other words, they are like local variables and need to initialized before the method/constructor is called using them as parameters.

```java
public void test() {
   int answer;
   anotherMethod(answer);  // DOES NOT COMPILE (var not initilized)
}
```

:bangbang: **Exam Tip:**
> Be wary of any local variable that is declared but not initialized in a single line. This is a common place on the exam that could result in a “Does not compile” answer. You are not required to initialize the variable on the same line it is defined, but be sure to check to make sure it’s initialized before it’s used on the exam.

---
<a id="c2-instance-class-variables"/></a>
#### Defining Instance and Class Variables
* Variables that are not local variables are defined either as instance variables or as class variables.


Variable | Value | Example
------- | ------- | -------
Instance | Defined within a specific instance of an Object</br>Each instance can have different values on the "same" attribute | String name;
Class    | Defined on the class level and shared among all instances of the class.</br>They're part of the class, not the instance. All instances will have the same value for that attribute | **static** String name;

A variable is a class variable if it has the static keyword in its declaration.

* Instance and class variables *do not require you to initialize them*. As soon as you declare these variables, they *are given a default value*.

:bangbang: **Exam Tip:**
> You’ll need to memorize everything in this table except the default value of char.

<a id="c2-default-initialization"/></a>

Variable Type | Default initialization value
------- | -------
boolean | false
byte, short, int, long | 0
float, double | 0.0
char | '\u0000' (NUL)
All object references (everything else) | null

---
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

---
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

---
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

* Java does **NOT allow var** in: `method parameters` (signature), `constructors` (signature), `instance variables` and `class variables`.
```java
public int addition(var a, var b) {  // DOES NOT COMPILE
   return a + b;
}
```

---
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

---
<a id="c2-review-var-rules"/></a>
#### Review of var Rules
*  A var can be used as a local variable in a constructor, method, or initializer block. 
*  A var *cannot be used* in constructor parameters, method parameters, instance variables, or class variables. 
*  A var is *always initialized* on the same line (or statement) where it is declared. 
*  The *value of a var* can change, but the *type cannot*. 
*  A *var cannot* be initialized with a null value without a type. 
*  A *var is not permitted* in a multiple-variable declaration. 
*  A var *is a reserved type name but not a reserved word*, meaning it can be used as an identifier except as a class, interface, or enum name.

:bangbang: **Exam Tip:**
> Since var is new to Java since the last exam, expect to see it used frequently on the exam.

---
<a id="c2-managing-var-scope"/></a>
### Managing Variable Scope
* Remember that the variable scope is based on the code-block it's defined. Blocks can contain other blocks.

<a id="c2-limiting-var-scope"/></a>
#### Limiting, Nesting and Tracing Scope
```java
16: public void eatIfHungry(boolean hungry) {
17:    if (hungry) {
18:       int bitesOfCheese = 1;
19:       {
20:          var teenyBit = true;
21:          System.out.println(bitesOfCheese); //COMPILES
22:       }
23:    }
24:    System.out.println(teenyBit);  // DOES NOT COMPILE (variable out of scope)
25: }
```

* Let's trace the method above and define what are the escopes

Line | First line in block | Last line in block | Obs
------- | ------- | ------- | -------
Method | 16 | 25 | as *hungry* is method parameter, it can be accessed inside all the method scope
if | 17 | 23 | *bitesOfCheese* only exist on IF scope
{ | 19 | 22 | *teenyBit* only exist on "*{ }*" scope

Variables declared inside in a scope will exist only in there, but remember *that smaller contained blocks can reference variables defined in the larger scoped blocks* BUT **not vice versa**

:bangbang: **Exam Tip:**
> You’ll want to practice this skill a lot! Identifying blocks and variable scope needs to be second nature for the exam.

---
<a id="c2-apply-var-scope-class"/></a>
#### Applying Scope to Classes
* When we're talking about variable scopes in classes we have:
	+ *Instance Variables*: They are available as soon as they are defined and _last for the entire lifetime of the object itself_.
	+ *Class Variables (static)*: They go into scope when declared like the other variable types. However, they _stay in scope for the entire life of the program._

```java
1:  public class Mouse {
2:     final static int MAX_LENGTH = 5; //Class variable
3:     int length;                      //Instance variable

4:     public void grow(int inches) { //"inches" scope -> Method
5:        if (length < MAX_LENGTH) { //"newSize" scope -> IF
6:           int newSize = length + inches;
7:           length = newSize;
8:        }
9:     }
10: }
```

---
<a id="c2-reviewing-var-scope"/></a>
#### Reviewing Scope
*  Local variables: In scope from declaration to end of block 
*  Instance variables: In scope from declaration until object eligible for garbage collection 
*  Class variables: In scope from declaration until program ends

---
<a id="c2-destroying-objects"/></a>
### Destroying Objects
Java provides a garbage collector to automatically look for objects that aren’t needed anymore.

* All **Java objects are stored** in your program *memory’s heap*. The heap, which is also referred to as the free store, represents a large pool of unused memory allocated to your Java application. The heap may be quite large, depending on your environment, but there is always a limit to its size.

---
<a id="c2-garbage-collection"/></a>
#### Understanding Garbage Collection
* *Garbage collection* refers to the process of automatically freeing memory on the heap by deleting objects that are no longer reachable in your program.

---
<a id="c2-eligible-garbage-collection"/></a>
#### Eligible for Garbage Collection
* *Eligible for garbage collection* refers to an object’s state of no longer being accessible
* When the object actually is discarded is not under your control, but for the exam, *we you will need to know* at any given moment which objects are eligible for garbage collection.
* As a programmer, what we can do to limit out-of-memory problems is to *make sure objects are eligible for garbage collection once they are no longer needed*. It is the JVM’s responsibility to actually perform the garbage collection.

---
<a id="c2-calling-gc"/></a>
#### Calling System.gc()
Java includes a built-in method to help support garbage collection that can be called at any time `System.gc();`

* It only suggests JVM to run the GC, but it JVM is free to ignore the request.
* It's not guaranteed that JVM will try to run your request

---
<a id="c2-tracing-eligibility"/></a>
#### Tracing Eligibility
The JVM waits patiently and monitors each object until it determines that the code no longer needs that memory. An object will remain on the heap until it is no longer reachable. It's not reachable when:

*  The object no longer has any references pointing to it. 
*  All references to the object have gone out of scope.

**PS:** Check the book on `Page 66` for more visual examples.

---
<a id="c2-objects-and-references"/></a>
#### Objects vs. References
* *Object*: Sits on the heap and does not have a name. Therefore, you have no way to access an object except through a reference.
* *Reference*: reference is a variable that has a name and can be used to access the contents of an object. A reference can be assigned to another reference, passed to a method, or returned from a method.

**PS:** References may or may not be created on the heap, all references are the same size no matter they data type.

---
<a id="c2-gc-finalize"/></a>
#### finalize()
:bangbang: **Exam Tip:**
> This topic is no longer on the exam.

* Java allows objects to implement a method called finalize(), the garbage collector would call the finalize() method once.
* Just remember that finalize() can run zero or one times. It cannot run twice.


---

<a id="chapter3"/></a>
## _Chapter 3:  Operators_ 
<a id="c3-operators"/></a>
### Understanding Java Operators: 
In java we have 3 types of operators: `unary, binary, and ternary`, we'll see how to apply them, and the order in which they should be applied.

* Java operators are not necessarily evaluated from left-to-right order.

```java
int cookies = 4;

//Evaluated from right to left given the specific operators involved
double reward = 3 + 2 * --cookies; 
System.out.print("Result: " + reward); //Output: 9.0
```

---
<a id="c3-operator-procedence"/></a>
#### Order of operator precedence

Operator | Symbols and examples
------- | -------
Post-unary operators | `expression++, expression--`
Pre-unary operators | `++expression, --expression`
Other unary operators | `-, !, ~, +, (type)`
Multiplication/division/modulus | `*, /, %`
Addition/subtraction | `+, -`
Shift operators | `<, >, <=, =>, instaceof`
Equal to/not equal to | `==, !=`
Logical operators | `&, ^, PIPE`
Short-circuit logical operators | `&&, PIPE PIPE`
Ternary operators | `boolean expression ? expression1:expression2`
Assignment operators | `=, +=, -=, *=, /=, %=, &=, ^=, PIPE=, <<=, >>=, >>>=`

**PS: PIPE means `|`,** MD format did not let me put in this way above because it's inside a table that uses `|` as column separator

:bangbang: **Exam Tip:**
> You won’t be tested on some operators, like the shift operators.

---
<a id="c3-applying-op"/></a>
### Applying Unary Operators
Requires exactly one operand, or variable, to function. They often perform simple tasks, such as increasing a numeric variable by one or negating a boolean value.

Operator | Description
------- | -------
`!` | Inverts a boolean’s logical value
`+` | Indicates a number is positive, although numbers are assumed to be positive in Java unless accompanied by a negative unary operator
`-` | Indicates a literal number is negative or negates an expression
`++` | Increments a value by 1
`--` | Decrements a value by 1
`(type)` | Casts a value to a specific type.

* The `!` operator flips the value of a boolean expression.

```java
boolean isAnimalAsleep = false;
System.out.println(isAnimalAsleep);  // false
System.out.println(!isAnimalAsleep); // true
```

* The negation operator `-` reverses the sign of a numeric expression

```java
double temp = 1.21;
temp = -temp;    // -1.21
temp = -(-temp); // -1.21 (Turned into positive and then negative)
```

**PS**: You cannot apply a negation operator (-) to a boolean expression, nor can you apply a logical complement operator (!) to a numeric expression.

```java
int pelican = !5;         // DOES NOT COMPILE
boolean penguin = -true;  // DOES NOT COMPILE
boolean peacock = !0;     // DOES NOT COMPILE
```

---
<a id="c3-increment-decrement"/></a>
#### Increment and Decrement Operators
* Pre-increment `++x` / pre-decrement `--x`: we **applied first** and the value returned is the new value of the expression.
* Post-increment operator `x++` / Post-decrement `x--`: the original value of the expression is returned, with operator **applied after** the value is returned.

```java
int value = 0;
System.out.println(++value);  // 1
System.out.println(value--);  // 1
System.out.println(value);    // 0
```

* We can apply multiple increment or decrement operators to a single variable on the same line. Keep in mind the <a href="#c3-operator-procedence">Order of operator precedence</a>

```java
int a = 3;
int b = ++a * 5 / a--;
System.out.println(a); //Output: 3
System.out.println(b); //Output: 5

//Processing order:
int b = ++a * 5 / 3; // a assigned value of 2
int b = 3 * 5 / 3;   // a assigned value of 3
```

---
<a id="c3-binary-operators"/></a>
### Working with Binary Arithmetic Operators

Operator | Description
------- | -------
`+` | Adds two numerics values
`-` | Subtracts two numeric values
`*` | Multiplies two numeric values
`/` | Divides one numeric value by another
`%` | Modulus operators returns the remainder after division of one numeric value by another

*Reminder*: The operators `*, /, %` have a higher order of precedence than the `+, -` ones.

---
<a id="c3-adding-parentheses"/></a>
#### Adding Parentheses
We can override the order of operator precedence using parentheses, by wrapping parentheses around the sections you want evaluated first.


```java
int mine = 2 * (32 - 8); //The code inside parentheses will be evaluated first
int mine = 2 * 24;

//PS: The parentheses should be balanced, it would NOT WORK:
int mine = 2 * (32 - 8;
int mine = 2 * (32 - 8));
```

---
<a id="c3-division-module-operators"/></a>
#### Division and Modulus Operators
* Modulus Operator `%`: Modulus operators returns the remainder after division of one numeric value by another

```java
System.out.println(9 / 3);   // 3
System.out.println(9 % 3);   // 0

System.out.println(10 / 3);  // 3
System.out.println(10 % 3);  // 1
```

:bangbang: **Exam Tip:**
> For the exam, you are not required to be able to take the modulus of a negative integer or a floating-point number.

 ---
 <a id="c3-numeric-promotion"/></a>
#### Numeric Promotion
*Numeric Promotion Rules*

- If two values have different data types, Java will automatically promote one of the values to the larger of the two data types.

- If one of the values is integral and the other is floating-point, Java will automatically promote the integral value to the floating-point value’s data type.
- Smaller data types, `byte, short, and char`, are first promoted to int any time they’re used with a Java binary arithmetic operator, even if neither of the operands is int. `Unary operators are excluded from this rule`. applying ++ to a short value results in a short value.
- After all promotion has occurred and the operands have the same data type, the resulting value will have the same data type as its promoted operands.

---
##### Complete example with all the rules being applied
```java
short w = 14;
float x = 13;
double y = 30;
var z = w * x / y;
```

**Processing order:**
- `w` will automatically be promoted to int solely because it is a short and it is being used in an arithmetic binary operation.
- The promoted `w` value will then be automatically promoted to a float so that it can be multiplied with x.
- The result of `w * x` will then be automatically promoted to a double so that it can be divided by y, resulting in a double value.

---

<a id="c3-assigning-values"/></a>
### Assigning Values
An assignment operator is a binary operator that modifies, or assigns, the variable on the left side of the operator, with the result of the value on the right side of the equation. `int a = 1;`

---
<a id="c3-casting-values"/></a>
#### Casting Values
* Casting is optional and unnecessary when converting to a larger or widening data type
* It is required when converting to a smaller or narrowing data type. Without casting, the compiler will generate an error when trying to put a larger data type inside a smaller one.


```java
//Cast is always on the left side
String type = (String)  "Bird"; 
long feathers = 10(long);  // DOES NOT COMPILE

//You should use parentheses if you want to apply to a expression result
short tail = (short)(4 + 10); 
```

---
<a id="c3-reviewing-primitive"/></a>
#### Reviewing Primitive Assignments
Similar examples we saw on Chapter 2

```java
int fish = 1.0;        // DOES NOT COMPILE -> Trying to assign a double 1.0 to an integer
short bird = 1921222;  // DOES NOT COMPILE -> Literal value is outside the range of short
int mammal = 9f;       // DOES NOT COMPILE -> "f" added to the end of the number that instructs the compiler to treat the number as a floating-point value
long reptile = 192301398193810323;  // DOES NOT COMPILE -> Java interprets the literal as an int and notices that the value is larger than int allows.
```

Now applying casting to this examples so they work

```java
int trainer = (int)1.0;
short ticketTaker = (short)1921222;  // Stored as 20678
int usher = (int)9f;
long manager = 192301398193810323L;
```

**By casting a larger value into a smaller data type, you are instructing the compiler to ignore its default behavior.**

* Another compile error and casting example

```java
short mouse = 10;
short hamster = 3;
short capybara = mouse * hamster;  // DOES NOT COMPILE
```

Trying to assign a short variable with an int value results in a compiler error, as Java thinks you are trying to implicitly convert from a larger data type to a smaller one. We can fix it by:


```java
short capybara = (short)(mouse * hamster);
```

**Review**: What's the difference and why one piece compiles and the other one not

```java
short mouse = 10;
short hamster = 3;
short capybara = mouse * hamster;  // DOES NOT COMPILE

short capybara2 = (short) 10 + (short) 3;  // COMPILES
```

---
<a id="c3-compound-assignment"/></a>
#### Compound Assignment Operators

Operator | Description | Ex
------- | ------- | -------
+= | Adds the value on the right to the variable on the left and assigns the sum to the variable | `a = a + b` </br> `a += b`
-= | Subtracts ... ^ ^ | `a = a - b` </br> `a -= b`
*= | Multiplies ... ^ ^ | `a = a * b` </br> `a *= b`
/= | Divides the variable on the left by the value on the right and assigns the quotient to the variable | `a = a / b` </br> `a /= b`

**Notes about Compound Assignment Operators**

* The left side of the compound operator can be applied only to a variable that is already defined and cannot be used to declare a new variable.

```java
//DOES NOT COMPILE
int b = 2;
a = a + b;

//COMPILES
int a = 3, b = 2;
a = a + b;
```

* They can also save us from having to explicitly cast a value.

```java
//Not using the Compound
long goat = 10;
int sheep = 5;
sheep = sheep * goat;   // DOES NOT COMPILE 
//We are trying to assign a long value to an int variable


//Using the Compound
long goat = 10;
int sheep = 5;
sheep *= goat; // COMPILES
//The compound operator will first cast sheep to a long, apply the multiplication of two long values, and then cast the result to an int.
```

---
<a id="c3-assignment-operator-return"/></a>
#### Assignment Operator Return Value
The result of an assignment is an expression in and of itself, equal to the value of the assignment.

```java
long a = 5;
long b = (a=3);
System.out.println(a); // 3
System.out.println(b); // 3

//Processing order
// Sets a value = 3
// Returns a value of the assignment, which is also 3.
```

Another tricky one

```java
boolean checked = false;
if(checked = true)
   System.out.print("Message!");

//It prints the Message, because we're assigning the value and only after this, comparing, which is "true".
```

---
<a id="c3-comparing-values"/></a>
### Comparing Values
They can be used to check if two values are the same, check if one numeric value is less than or greater than another, and perform boolean arithmetic.

---
<a id="c3-equality-operators"/></a>
#### Equality Operators
The equals operator `(==)` and not equals operator `(!=)` compare two operands and return a boolean value determining whether the expressions or values are equal or not equal, respectively.


Operators | Apply to primitive | Apply to objects
------- | ------- | -------
== | Returns true if the two values represent the same value | Returns true if the two values reference the same object
!= | Returns true if the two values represent different values | Returns true if the two values do not reference the same object

You can use them to:

* Comparing two numeric or character primitive types. </br>If the numeric values are of different data types, the values are automatically promoted. For example, `5 == 5.00` returns true since the left side is promoted to a double.
* Comparing two boolean values
* Comparing two objects, including null and String values

**PS**: You **CAN'T** mix and match types.

```java
// DOES NOT COMPILE (ALL)

boolean monkey = true == 3;
boolean ape = false != "Grape";
boolean gorilla = 10.2 == "Koko";
```

**PS:** When comparing objects, the equality operators check if they both point to the same memory reference, its not related to object values itself, <a href="#c2-reference-types">we saw that on Chapter 2</a>

---
<a id="c3-relational-operators"/></a>
#### Relational Operators

Operator | Description
------- | -------
`<` | Returns true if the value on the left is **strictly less** than the value on the right
`<=` | Returns true if the value on the left is less than **or equal** to the value on the right
`>` | Returns true if the value on the left is **strictly greater** than the value on the right
`>=` | Returns true if the value on the left is greater than **or equal** to the value on the right
`a instanceof b` | Returns true if the reference that a points to is an instance of a class, subclass, or class that implements a particular interface, as named in b

The first four relational operators, apply only to numeric values. If the two numeric operands are not of the same data type, the smaller one is promoted as previously discussed.

---
<a id="c3-instanceof-operator"/></a>
#### instaceof Operator
It is useful for determining whether an arbitrary object is a member of a particular class or interface at runtime.

**PS**: With polymorphism, using the `instaceof` will return true if the class is a subclass of that type

```java
Integer ex = Integer.valueOf(9);

System.out.print(ex instanceof Integer); //true
System.out.print(ex instanceof Number);  //true
System.out.print(ex instanceof Object);  //true
```

---
##### Invalid instaceof
The exam might try to trip you up on is using instanceof with incompatible types. </br>For example, Number cannot possibly hold a String value

```java
Integer ex = Integer.valueOf(9);
System.out.print(ex instanceof String);  // DOES NOT COMPILE
```

---
##### null and the instanceof operator
Calling instanceof on the null literal or a null reference (left side) **always returns false**.

```java
System.out.print(null instanceof Object); //false

Object noObjectHere = null;
System.out.print(noObjectHere instanceof String); //false

//You CAN'T use "null" on the right side of instaceof
System.out.print(null instanceof null);  // DOES NOT COMPILE
```

---
<a id="c3-logical-operator"/></a>
#### Logical Operators
The logical operators, `(&), (|), and (^)`, may be applied to both numeric and boolean data types. When they’re applied to boolean data types, they’re referred to as logical operators.

:bangbang: **Exam Tip:**
> For the exam, though, you don’t need to know anything about numeric bitwise comparisons (logical operators applied to numeric data type)


Operator | Description
------- | -------
& | Logical AND is true only if both values are true.
PIPE | Inclusive OR is true if at least one of the values is true.
^ | Exclusive XOR is true only if one value is true and the other is false.

**PS: PIPE means `|`,** MD format did not let me put in this way above because it's inside a table that uses `|` as column separator

---
<a id="c3-short-circuit-operators"/></a>
#### Short-Circuit Operators

Operator | Description
------- | -------
&& | Is true only if both values are true.</br> If the left side is false, then the right side **will not be evaluated.**
PIPE PIPE | Is true if at least one of the values is true.</br>If the left side is true, then the right side **will not be evaluated.**

**PS: PIPE PIOE means `||`,** MD format did not let me put in this way above because it's inside a table that uses `|` as column separator

* Logical Operator `& |`: evaluates **both sides** of the expression.
* Short-Circuit Operator `&& ||`: the *right side of the expression may never be evaluated* **if the final result** can be determined **by the left side** of the expression.

---
##### Avoiding NPE:
```java
if(duck!=null & duck.getAge()<5) { //Can throw a NullPointerException

if(duck!=null && duck.getAge()<5) { //Can't throw a NullPointerException
```

---
##### Checking for Unperformed Side Effects
Since the right side of the expression may never be reached, we must pay attention in tricky questions like this

```java
int rabbit = 6;
boolean bunny = (rabbit >= 6) || (++rabbit <= 7);
System.out.println(rabbit); //Output: 6
```

---
<a id="c3-ternary-operators"/></a>
#### Ternary Operator
The ternary operation is really a condensed form of a combined if and else statement that returns a value.

```java
int owl = 5;
int food = owl < 2 ? 3 : 4;
System.out.println(food); // 4
```

* There is no requirement that second and third expressions in ternary operations have the same data types, **BUT IF** you're assigning a value to a variable things can change

```java
int test = 7;
 
System.out.print((test > 5) ? 21 : "Zebra");
 
int animal = (test < 9) ? 3 : "Horse";  // DOES NOT COMPILE
//The "else" result tries to put the a String inside an Int
```

**PS:**: If the ternary doesn't reach a specific condition, the code inside that block will not be executed

```java
int a = 1, b = 1;
int sleep = a<10 ? a++ : b++;
System.out.print(a + "," + b);  // 2,1 
//b was not incremented because the code was not reached
```

---
---
<a id="chapter4"/></a>
## _Chapter 4:  Making Decisions_ 

<a id="c4-creation-decision"/></a>
### Creating Decision-Making Statements

<a id="c4-if-statement"/></a>
#### The if Statement
It allows our application to execute a particular block of code if and only if a boolean expression evaluates to true at runtime.

```java
if(booleanExpression){
	//code to be executed if true
}
```

<a id="c4-if-rules"/></a>
**IF Rules:**

* Parentheses required
* Curly braces required for block of multiple statements, optional for single statement. If you **NOT PUT braces**, java will execute **only the next line**, it doesn't matter if the rest of the code is indented
* Expression must be boolean expressions

```java
int hourOfDay = 1;
if(hourOfDay) {  // DOES NOT COMPILE
```

* Assignments operators are valid if they return a boolean expression

```java
int hourOfDay = 1;
if(hourOfDay = 5) {  // DOES NOT COMPILE

boolean valid = false;
if(valid = true) { // COMPILES (but doesn't make sense)
```

---
<a id="c4-else-statement"/></a>
#### The else Statement
We can use `else` to execute a specific piece of code if none of the `if` conditions were satisfied

```java
if(dayTime < 15) {
   System.out.println("Good Morning");
} else if(dayTime < 11) { // COMPILES BUT IS UNREACHABLE
   System.out.println("Good Afternoon");
} else {
   System.out.println("Good Evening");
}

// Second if is not reachable because the first condition covers this by having a larger number
```

PS: The <a href="#c4-if-rules">IF Rules</a> are the same for `else` statement 

---
<a id="c4-switch-statement"/></a>
#### The switch Statement
A switch statement is a complex decision-making structure in which a single value is evaluated and flow is redirected to the first matching branch, known as a case statement.

```java
int month = 5;
switch (month) {
   case 1: System.out.print("Jan"); break;
   case 2: System.out.print("Feb");
   default: System.out.print("None");
}
```

**Switch Rules:**

* **Required:** Parentheses
* **Required:**  Curly braces (beginning and ending) 
* **Required:**  Follow the `case X:` syntax, the `case / default` keyword and ":" are mandatory
* Optional: `break`
* Optional: `default` case. There's specific place required for it
* Optional: Spaces / Lines breaks inside the switch structure: `switch, case, default, :`
* **Possible** values to be evaluated: `int, byte, short, chat, String, ENUM, var (if the type resolves to one of the preceding types)` and the related Wrappers from these primitives `Integer, Byte, Short, Character`
* **Not possible** values: All the other ones that were not mentioned above: `boolean, long, float, double` and their related Wrappers
* You **CAN'T**: Use `&&` and `||` on switch `cases`

**PS:** You can use `&` and `|` (single ones) in switch but it's related to bitwise arithmetic but it **WILL NOT** be covered **on the exam**. Just remember that it compiles

---
##### Break statement
We use break when we want to terminate the switch statement and return flow control to the enclosing statement.

So if you **don't put** the break statement in a specific `case` condition, flow will continue to the **next proceeding cases or default** block **automatically**.

* Example Without break

```java
var value = 0;
switch(value) {
   case 0:
      System.out.println("0");
   default:
      System.out.println("1");
   case 2:
      System.out.println("2");
      
//Output: 0, 1, 2
// It matches the first case but it keeps "sliding" but it continues to slide through the cases below (including default) because it does not find a "break" in any of them
```

* Example With break

```java
var value = 0;
switch(value) {
   case 0:
      System.out.println("0");
      break;
   default:
      System.out.println("1");
   case 2:
      System.out.println("2");
      
//Output: 0
// It matches the first case and stop it there because of "break"
```

##### Default statement
The default is executed only in 2 cases

* None of the case conditions were met
* A `case` "above" the `default` was executed and does not have a "break" inside. (Code example above)

**PS:** The `default` doesn't NOT require a specific declaration order

---
##### Acceptable Case Values
* The values in each case statement must be **compile-time constant** values of the **same data type** as the switch value.
* This means you can use only `literals`, `enum constants`, or `final constant` variables of the same data type.

```java
final int getCookies() { return 4; }
void feedAnimals() {
   final int bananas = 1;
   int apples = 2;
   int numberOfAnimals = 3;
   final int cookies = getCookies();
   switch (numberOfAnimals) {
      case bananas:
      case apples:  // DOES NOT COMPILES
      case getCookies():  // DOES NOT COMPILE
		 case cookies :  // DOES NOT COMPILE
      case 3 * 5 :
   }
}
```

**PS:**

* Even if you're passing a parameter with `final` in a method, you can't use it on the `case` statement, it is not constant as it is passed to the function

---
##### Numeric Promotion and Casting
Switch statements support numeric promotion that does not require an explicit cast.

```java
short size = 4;
final int small = 15;
final int big = 1_000_000;
switch(size) {
   case small:
   case 1+2 :
   case big:  // DOES NOT COMPILE
}
```

* As we discussed in <a href="#c3-numeric-promotion">numeric promotion</a>, the compiler can easily cast `small` from `int` to `short` at compile-time because the value 15 is small enough to fit inside a short. The same for the `1+2` expression </br>But in the last case, the `big` is **too large** to fit inside of short **without an explicit cast**.

---
<a id="c4-writing-while-loops"/></a>
### Writing while Loops
A loop is a repetitive control structure that can execute a statement of code multiple times in succession.

---
<a id="c4-while-statement"/></a>
#### While statement
```java
while (booleanExpression){
}
```

**While Rules:**

* **Required:** Parentheses
* Curly braces required for block of multiple statements, optional for single statement. If you **NOT PUT braces**, java will execute **only the next line**, it doesn't matter if the rest of the code is indented
* You can use `&&`, `||`, `&`, `|` operators on the expression

---
<a id="c4-do-while-statement"/></a>
#### The do/while Statement
A `do/while` loop guarantees that the statement or block will be executed at least once. Whereas a while loop is executed zero or more times, a do/while loop is executed one or more times.


```java
do {

} while (booleanExpression); //semicolon required
```

**PS:** The <a href="#c4-if-rules">While Rules</a> are the same for `do/while` statement

---
##### Infinite loops
Make sure the loop condition, or the variables the condition is dependent on, are changing between executions, otherwise you could run out of memory.

---
<a id="c4-cont-for-loops"/></a>
### Constructing for Loops
Another kind of loop, when you want to iterate over a statement a specific number of times may be the best option

<a id="c4-for-loops"/></a>
#### The for Loop

```java
for (initialization; booleanExpression; updateStatement) {
	//Body
}
```

**For Rules:**

* **Required:** Parentheses
* **Required:** Semicolons
* Curly braces required for block of multiple statements, optional for single statement. If you **NOT PUT braces**, java will execute **only the next line**, it doesn't matter if the rest of the code is indented
* Variables initialized in the `for` statement are not visible to outside (just remember about <a href="#c2-managing-var-scope">Variable scopes</a>) 
* You can use `&&`, `||`, `&`, `|` operators on the `booleanExpression`

> The items `initialization`, `booleanExpression` and `updateStatement` are **not required**, it will not cause a compilation error if you omit them (may not make sense or cause an infinite loop but it is something to keep in mind during the exam)

**Execution Order**

*  1 - `initialization` statement executes
*  2 - If `booleanExpression` was **is true** continue; else exit loop
*  3 - `Body` executes
*  4 - Execute `updateStatement`
*  5 - Return to Step 2

---
##### Printing Elements in Reverse
We can use `--` instead of `++` on the `updateStatement` and do a "reverse loop", this is completely normal

```java
for(int i = 0; i < 5; i++) {
   System.out.print(i + " "); //0 1 2 3 4
}

for (var i = 4; i >= 0; i--) {
   System.out.print(i + " "); //4 3 2 1 0
}
```

---
<a id="c4-scenarios-using-loops"/></a>
#### Scenarios while using for loop
There are some scenarios that are not normal in real life but we must be aware during the exam

##### Creating an Infinite Loop

```java
for( ; ; ) //COMPILES but It's infinite
   System.out.println("Hello World");
```

##### Adding Multiple Terms to the for Statement

```java
int x = 0;
for(long y = 0, z = 4; x < 5 && y < 10; x++, y++) { //COMPILES
	System.out.print(y + " ");
}
System.out.print(x + " ");
// Output: 0 1 2 3 4 5
```

* Declaring a variable `x` before the loop and using it
* Including extra variables in the 3 sections (init; expression; update) that *may or may not* reference each other
* Modifying multiple variables in the update section

##### Redeclaring a Variable in the Initialization Block

```java
//Redeclaring a existing variable
int x = 0;
for(int x = 4; x < 5; x++) {   // DOES NOT COMPILE
   System.out.print(x + " ");
}

//Reusing a existing variable WITHOUT redeclaring
int x = 0;
for(x = 0; x < 5; x++) { // COMPILES
   System.out.print(x + " ");
}
```

##### Using Incompatible Data Types in the Initialization Block
The variables in the initialization block **must** all be of the **same type**.

```java
int x = 0;
for(long y = 0, int z = 4; x < 5; x++) {  // DOES NOT COMPILE
```

**PS**: When declaring multiple variables on the init block that have the same type, you **can't** repeat the type keyword

```java
for(int y = 0, int z = 4; x < 5; x++) {  // DOES NOT COMPILE

for(int y = 0, z = 4; x < 5; x++) {  // COMPILES
``` 

##### Using Loop Variables Outside the Loop

```java
for(long y = 0, x = 4; x < 5 && y < 10; x++, y++) {
   System.out.print(y + " ");
}
System.out.print(x);  // DOES NOT COMPILE
//Variable scope rules applies to "for" statement as well
```

##### Modifying Loop Variables
You **CAN** modify the loop variables inside the `for` scope, **BUT** you can mess things up like creating infinite loops

```java
for(int i=0; i<10; i++)
   i = 0; //COMPILES but it's infinite
 
for(int j=1; j<10; j++)
   j--; //COMPILES but it's infinite
   
for(int k=0; k<10; ) //COMPILES and NOT infinite (good example)
   k++;

```

---
<a id="c4-for-each-loop"/></a>
#### The for-each Loop
The for-each loop is a specialized structure designed to iterate over arrays and various Collection Framework classes


```java
for (dataType instance : Colletion){
	//Body
}
```

**For-each Rules:**

* **Required:** Parentheses
* **Required:** Colon
* **Required:** The right side **must** be an array or collection of items, such as a List or a Set (Any class that **implements Collection** interface)

Concrete example:

```java
public void showNames(String[] names) {
   for(String name : names)
      System.out.println(name);
}
```

---
##### More notes about for-each

* Like the regular for loop, the for-each loop also accepts var for the loop variable
* When you see a for-each loop on the exam, **make sure** the right side is an **array or Iterable object** and the left side has **a matching type**.

```java
String[] names = new String[3];
for(int name : names) {  // DOES NOT COMPILE
```

---
<a id="c4-flow-with-branching"/></a>
### Controlling Flow with Branching

<a id="c4-nested-loops"/></a>
#### Nested Loops
A nested loop is a loop that contains another loop including while, do/while, for, and for-each loops. You can create infinite "loop inside loop" structure mixing everything we've seen so far `for, foreach, while, do-while`

* Looping a two-dimensional array

```java
int[][] myComplexArray = {{5,2,1,3},{3,9,8,9},{5,7,12,7}};
 
for(int[] mySimpleArray : myComplexArray) {
   for(int i=0; i<mySimpleArray.length; i++) {
      System.out.print(mySimpleArray[i]+"\t");
   }
   System.out.println();
}

/*Output: 
5       2       1       3
3       9       8       9
5       7       12      7
*/
```

* Mixing while/do-while

```java
int hungryHippopotamus = 8;
while(hungryHippopotamus>0) {
   do {
      hungryHippopotamus -= 2;
   } while (hungryHippopotamus>5);
   hungryHippopotamus--;
   System.out.print(hungryHippopotamus+", ");
}
//Output: 3, 0,
//To follow this conclusion, remember do-while always execute once, even if the condition is not true
```

> When working with inner-loops, pay attention to the order of execution, the innermost loop "holds" the outermost one. Review the examples above to understand

---
<a id="c4-optional-labels"/></a>
#### Adding Optional Labels
A label is an optional pointer to the head of a statement that allows the application flow to jump to it or break from it.</br> It is a *single identifier* that is proceeded by a colon (`:`).

##### Statements that can have optional labels

* `if / else`, `switch`, `loops` (in general), `block-statements` (`{ }`)

```java
//COMPILES
OUTER_LOOP:  for(int[] mySimpleArray : myComplexArray) {
   INNER_LOOP:  for(int i=0; i<mySimpleArray.length; i++) {
	IF_LABEL: if(frog>10)
					CODE_BLOCK_LABEL: {
					   ANOTHER_LABEL: frog++;
					}
```
 
```java
//DOES NOT COMPILE
     VAR_LABEL: int frog = 15; //COMPILATION ERROR: Not a statement
     if(frog>10)
         {
             frog++;
ANOTHER: } //COMPILATION ERROR: Label without a statement

```

> Label are useful for `loop` statements, because you can reference an **external loop** inside an **internal loop** for example, and ask to stop it (`break;`)

---
<a id="c4-break-statement"/></a>
#### The break Statement
A break statement transfers the flow of control out to the enclosing statement. When used with `loops` it will end the loop early.

```java
optionalLabel: while(booleanExpression){
	// Body
	
	//Somewhere in loop
	break optionalLabel;
}
```

**Break Rules:**

* **Required:** Semicolon `;`

* **Optional:** Label </br>If you not refer a Label, the break statement will terminate the nearest inner loop it is currently in the process of executing.


---
**Label Rules**

* **Required:** Semicolon `;`

* **Optional**: Using uppercase letters, with underscores between words. Not required, it's just a convention 

---

The optional label parameter allows us to break out of a higher-level outer loop.

```java
PARENT_LOOP: for(...) {
         for(...) {
            if(conditionMet) {
               break PARENT_LOOP;
            }
         }
      }
```

In the example above, if we used the `break` **without a label**, it would stop just the inner loop and move on to the next iteration of the outer loop, this can **generate unnecessary loops** and can also **affect the output result**

> Using a label on a break statement in a nested loop, or not using the break statement at all, can cause the loop structure to behave quite differently.

---
<a id="c4-continue-statement"/></a>
#### The continue Statement
A statement that causes flow to finish the execution of the current loop

```java
optionalLabel: while(booleanExpression){
	// Body
	
	//Somewhere in loop
	continue optionalLabel;
}
```

**Continue Rules:**

* **Required:** Semicolon `;`

* **Optional:** Label </br>If you not refer a Label, the continue statement will terminate the nearest inner loop it is currently in the process of executing.

While the **break statement transfers control to the enclosing statement**, </br>the **continue statement transfers control to the boolean expression that determines if the loop should continue**. In other words, **it ends the current iteration of the loop**.

```java
//TODO: Elaborate continue Example in code
```

---
<a id="c4-return-statement"/></a>
#### The return Statement
Assuming your loop is inside a method, you can use the `return` statement to exit a chain of loops instead of using `break / continue` statements

```java
public int findValue(...)
for(...){
   for (...) {
   	for (...) {
   		if(conditionMet) {
   			return value; //If code reaches to this point, it will return the value to the method and all the chain of loops will be skipped.
```

**PS**: We'll take more about `return` in the next Chapers

---
<a id="c4-unreachable-code"/></a>
#### Unreachable Code
When using `break`, `continue`, and `return` any code **placed immediately after** them in the same block is **considered unreachable** and will **not compile**.

```java
//Ex 1:
for (...){
	if(conditionMet) {
      break;
      checkDate++;  // DOES NOT COMPILE
   }
   
//Ex 2:
int myVar = 1;
HEY: while(...) {
   if(conditionMet) {
      continue HEY; myVar++; // DOES NOT COMPILE
      System.out.print("Hello!");  // DOES NOT COMPILE
```

---
<a id="c4-reviewing-branching"/></a>
#### Reviewing Branching

Loop | Allows labels | Allows break | Allows continue
------- | ------- | ------- | -------
while | Yes | Yes | Yes
do while | Yes | Yes | Yes
for | Yes | Yes | Yes
switch | Yes | Yes | No

**PS:** You can use `return` in all of them</br> Just keep in mind you're covering all the possible "return cases" in your code, otherwise you will face a `Missing return statement` (we'll talk more about it latter)

**PS II**: `if` statement only supports `return` and `labels`, but **NOT** `break` and `continue`


---

<a id="chapter5"/></a>
## _Chapter 5:  Core Java APIs_ 
<a id="c3-operators"/></a>
### Creating and Manipulating Strings
A string is basically a sequence of characters. In Java, these two snippets both create a String

```java
String name = "Fluffy";
String name = new String("Fluffy");
```

This difference is related to `StringPool`, we'll cover it latter. Just remember we can create Strings *with/without* `new` keyword.

---
#### Concatenation
Placing one String before the other String and combining them (`+`) is called string concatenation. The `+` operator can be used in two ways within the same line of code.

* If both operands are **numeric**, `+` means **numeric addition**
* If either operand is a **String**, `+` means **concatenation**
* The expression is evaluated left to right

```java
System.out.println(1 + 2);           // 3
System.out.println("a" + "b");       // ab
System.out.println("a" + "b" + 3);   // ab3
System.out.println(1 + 2 + "c");     // 3c
System.out.println("c" + 1 + 2);     // c12
```

The **same rules** are applied to <a href="#c3-compound-assignment">compound assignment operators</a>

```java
4: String s = "1";             // s currently holds "1"
5: s += "2";                   // s currently holds "12"
6: s += 3;                     // s currently holds "123"
7: System.out.println(s);      // 123
```

---
#### Immutability
**String is immutable**. Once a String object is created, it is not allowed to change. It cannot be made larger or smaller, and you cannot change one of the characters inside it.

A Immutable class means that the class can't change. You can make a Immutable class by not exposing its attributes and not creating `set methods`, only `get` ones.

**PS:** Immutable classes in java are `final`, which *prevents* subclasses creation.

---
##### Concat method
We saw that we can use `+` to concatenate strings, but there's also the `concat` method.

`Method Overloads: 0`

```java
String s1 = "1";
String s2 = s1.concat("2");
s2.concat("3");
System.out.println(s2); //12
```

> The output is 12 because Strings are Immutable, so the original String object did not change! The concat method only returns a new String instance

---
<a id="c5-important-string-methods"/></a>
#### Important String Methods
Remember that a **string** is a **sequence of characters** and Java **counts from 0**

##### length()
The method length() returns the number of characters in the String

`Method Overloads: 0`

```java
String string = "animals";
System.out.println(string.length());  // 7
//The index counts from 0 but the length counts from 1, that's why the output is 7 and not 6
```

---
##### charAt()
The method charAt() lets you query the string to find out what character is at a `specific index`.

`Method Overloads: 0`

```java
String string = "animals";
System.out.println(string.charAt(0));  // a
System.out.println(string.charAt(6));  // s
System.out.println(string.charAt(7));  // throws exception
//Like we said, indexes count from 0, so the last letter is on the 6 index, not 7
```

---
##### indexOf()
The method indexOf() looks at the characters in the string and finds the first index that matches the desired value.

* `indexOf` can work with an individual character or a whole String as input
* It can also start from a requested position (index), it's the second parameter when exists
* The method signature when receives a `char` is `indexOf(int ch)` because char can be passed as a int
* If it can't find a match, it will return `-1`
* Doesn't throw exception if can't find the value (different from `charAt`)
* It's **case sensitive**

`Method Overloads: 4`

```java
//All possible method signatures
String string = "animals";
System.out.println(string.indexOf('a'));         // 0
System.out.println(string.indexOf("al"));        // 4
System.out.println(string.indexOf('a', 4));      // 4
System.out.println(string.indexOf("al", 5));     // -1 (Not Match)
```

---
##### substring()
The method substring() also looks for characters in a string. It returns parts of the string

* The first parameter is the index to start with for the returned string.
* There is an optional second parameter, which is the end index you want to stop at

With this method we have to think in index in a different way. Pretend the indexes are right before the character they would point to.

<a id="c5-sub-string-logic"/></a>
![subStringEx](https://github.com/rickhpdev/java-11-certification/blob/main/images/subStringEx.png?raw=true)

`Method Overloads: 2`

```java
String string = "animals";
System.out.println(string.substring(3));                   // mals
System.out.println(string.substring(string.indexOf('m'))); // mals
System.out.println(string.substring(3, 4));                // m
System.out.println(string.substring(3, 7));                // mals
```

* There are also less obvious / edge-cases

```java
//Case 1: we start and end with the same index, there are no characters in between
System.out.println(string.substring(3, 3)); // empty string

//Case 2: the indexes can’t be backward
System.out.println(string.substring(3, 2));  // throws exception 

//Case 3: There is no eighth position
System.out.println(string.substring(3, 8)); // throws exception

//PS: There is no seventh character either, but at least there is the “end of string” invisible position
```

* Substring review: Returns the string starting from the requested index. If an end index is requested, it stops right before that index. Otherwise, it goes to the end of the string

:bangbang: **Exam Tip:**
> The substring() method is the trickiest String method on the exam. Make sure you understand how it works reviewing the examples and the edge-cases

---
##### toLowerCase() and toUpperCase()
These methods converts any lowercase characters to uppercase and vice-versa in the returned string

`Method Overloads: 0`

```java
String string = "dAaDy";
System.out.println(string.toUpperCase());  // DADDY
System.out.println("Abc123".toLowerCase());  // daddy
```

---
##### equals() and equalsIgnoreCase()
* The **equals()**: checks whether two String objects contain exactly the same characters in the same order.
* The **equalsIgnoreCase()**: the same but it will "ignore" the case (convert the characters’ case if needed)

`Method Overloads: 0`

```java
System.out.println("abc".equals("ABC"));  // false
System.out.println("ABC".equals("ABC"));  // true
System.out.println("abc".equalsIgnoreCase("ABC"));  // true
```

**PS**: The `equals()` **receives an object** because it's the same for all Objects (comes from Object Class), the `equalsIgnoreCase()` **only receives** `String`

---
##### startsWith() and endsWith()
The startsWith() and endsWith() methods look at whether the provided value matches part of the String (start or end) 

`Method Overloads: 0`

```java
System.out.println("baby".startsWith("b")); // true
System.out.println("baby".startsWith("B")); // false
System.out.println("baby".endsWith("y")); // true
System.out.println("baby".endsWith("b")); // false
```

**PS**: Like all other methods, it's **case-sensitive**

---
##### replace()
The replace() method does a simple search and replace on the string

`Method Overloads: 2`

```java
//Receiving char
System.out.println("abcabc".replace('a', 'A')); // AbcAbc

//Receiving char-sequence (String)
System.out.println("abcabc".replace("ab", "AB")); // ABcABc
```

---
##### contains()
Looks for matches in the String, the match can be anywhere in the String

`Method Overloads: 0`

```java
System.out.println("abc".contains("b")); // true
System.out.println("abc".contains("B")); // false
```

---
##### trim(), strip(), stripLeading(), and stripTrailing()
They're all related to remove space from String with some differences


Method | Descrption
------- | -------
`trim()`  | Remove whitespace from the beginning and end of a String
`strip()` | Same of `trim()` but supports Unicode
`stripLeading()` | **Removes** whitespace from **the beginning** of the String and **leaves** at **the end**
`stripTrailing()` | **Removes** whitespace from **the end** of the String and **leaves** at **the beginning**

**PS:** None of them remove spaces between the string, only before/after

`Method Overloads: 0`

```java
String t = " abc\t ";
System.out.println(t.trim().length());         // 3
System.out.println(t.strip().length());        // 3
System.out.println(t.stripLeading().length()); // 5
System.out.println(t.stripTrailing().length());// 4
```

**Whitespace consists of** (what is trimmed)

* Spaces along with the `\t` (tab) and `\n` (newline) characters 
* Other characters, such as `\r` (carriage return)

**PS:** Do not confuse `\` with `/`. The `/` are is a normal character, the `\` is a backslash escape

##### Notes that this special characters (and spaces)

```java
//1 - They count as ONE character
System.out.println("b\na".length()); //3 (not 4)

//2 - If there's no content on their left side, they don't count
System.out.println("\n\t\r".length()); //0 (not 3)

//3 - Only spaces don't count
System.out.println("     ".length()); //0

4 - Only spaces between "valid" content counts
System.out.println("      2  a  c";.length()); //7 (spaces before "2" are not being counted)
```

:bangbang: **Exam Tip:**
> You don’t need to know about Unicode for the exam

---
##### intern()
The `intern()` method returns the value from the string pool if it is there. Otherwise, it adds the value to the string pool. It will be covered latter

`Method Overloads: 0`

```java
String intern()
```

---
#### Method Chaining
We can mix all this String methods we've seen so far, be aware of that and practice it.</br> Since all the methods returns a **new String**, we can keep **chaining the methods** calling if from the **new String returned**.

```java
String result = "1TeXt   ".trim().toLowerCase().replace('1', '2'); // 2text
```

* Remember that String is immutable. Every string Method will return a NEW STRING and NOT modify the existing one

```java
5: String a = "abc";
6: String b = a.toUpperCase();
7: b = b.replace("B", "2").replace('C', '3');
8: System.out.println("a=" + a); //abc
9: System.out.println("b=" + b); //AC3

//PS: 4 Strings were created here
```

---
### Using the StringBuilder Class
Concat Strings using `+` creates a bunch of objects since String is immutable, that's why we have the StringBuilder class!

**PS:** Look at the book for a full explanation about it with examples

```java
StringBuilder builder = new StringBuilder();
builder.append("text").append("text2")...;
```

:bangbang: **Exam Tip:**
> In addition to StringBuilder, there's also StringBuffer BUT is no longer on either exam

---
#### Mutability and Chaining
Different from `String`, the `StringBuilder` is **Mutable**. When chaining StringBuilder, it **does not create a new object**, it changes its own state and **returns a reference to itself**

```java
StringBuilder sb = new StringBuilder("start");
sb.append("+middle");                      // sb = "start+middle"
StringBuilder same = sb.append("+end");    // "start+middle+end"

System.out.println(same == sb); //true (same object in memory)
```

---
#### Creating a StringBuilder
There are three ways to construct a StringBuilder

```java
// 1 - Creates containing empty characters
StringBuilder sb1 = new StringBuilder();

// 2 - Creates containing some characters
StringBuilder sb2 = new StringBuilder("animal");

// 3 - Creates containing empty characters 
// But Tells Java that we have some idea of how big the eventual value will be
StringBuilder sb3 = new StringBuilder(10);
```

---
#### Important StringBuilder Methods
##### charAt(), indexOf(), length(), and substring()
Work exactly the same as in the <a href="#c5-important-string-methods">String class</a>

**PS**: When using **these specific methods** on StringBuilder, remember they don't modify the StringBuilder instance, they return new values to be used / assigned

```java
StringBuilder sb = new StringBuilder("animals");
String sub = sb.substring(...); //Returns a new String
```

---
##### append()
It adds the parameter to the StringBuilder and returns a reference to the current StringBuilder

`Method Overloads: 10+` (Because it accepts different variable types)

```java
StringBuilder sb = new StringBuilder().append(2).append('D');
sb.append("-").append(true); // // 2D-true
```

---
##### insert()
Adds characters to the StringBuilder at the **requested index** and returns a reference to the current StringBuilder

```java
StringBuilder sb = new StringBuilder("hello");
sb.insert(5, "-");                   // sb = hello-
sb.insert(2, "-");                   // sb = he-llo-
```

`Method Overloads: 0`
`Methods throw exception if invalid Index?` **YES** 

**Notes:**

* Every time you put a new character, the indexes changes
* The index says where the character will be put, so the existing character at that index will be moved to right

---
##### delete() and deleteCharAt()
`delete()` removes **characters from a index sequence** and returns a reference to the current StringBuilder
`deleteCharAt()` removes **one character from a specific index** and returns a reference to the current StringBuilder

```java
StringBuilder sb = new StringBuilder("abcdef");
sb.delete(1, 3);                  // sb = adef (same "substring logic")
sb.deleteCharAt(5);               // throws an exception
```

`Method Overloads: 0`
`Methods throw exception if invalid Index?` **YES** 

* As we can see, in the first example, the method removed from `index 1` (d) to **right before** `index 3` (c)

**PS**: The `delete()` method uses the same <a href="#c5-sub-string-logic">"right before index" substring logic</a>

---
##### replace()
Works different from String one and returns a reference to the current StringBuilder 

```java
StringBuilder builder = new StringBuilder("pigeon dirty");
builder.replace(3, 6, "sty"); // pigsty dirty  

//Also possible: Replacing the text with nothing
builder.replace(3, 100, ""); //pig

// Invalid starting index
builder.replace(233, 100, ""); //throws an exception
```

`Method Overloads: 0`
`Methods throw exception if invalid Index?` **YES** (Only when invalid `startIndex`)

**PS**: Also uses the same <a href="#c5-sub-string-logic">"right before index" substring logic</a>

---
##### reverse()
Reverses the characters in the sequences and returns a reference to the current StringBuilder

```java
StringBuilder sb = new StringBuilder("ABC");
sb.reverse(); //CBA
```

---
##### toString()
Converts a StringBuilder into a String

```java
StringBuilder sb = new StringBuilder("ABC");
String s = sb.toString();
```

---
### Understanding Equality
#### Comparing equals() and ==

* `equals()`: Depends on object equals implementation, **the String equals() compares the content**
* `==`: Compares memory reference

**PS:** **The String equals() compares the content**. The authors did not implement equals for StringBuilder.
**PS II:** If a object does not implement the `equals()` method, the default behavior is compare the memory reference `==`

```java
String x = new String("Hello World");
String z = new String("Hello World");
System.out.println(x.equals(z)); // true
System.out.println(x == z); // false
```

* You can't compare objects references of different types 

```java
String string = "a";
StringBuilder builder = new StringBuilder("a");
System.out.println(string == builder); //DOES NOT COMPILE
```

-> **New People:** _Important topic_, look at the book for more in-depth explanation and more examples.

---
#### The String Pool
Was created for memory optimisation when talking about String. The string pool contains literal values and constants that appear in your program

* When we create literals/constants they're stored as one in the String Pool, both point to the same memory reference

```java
String x = "Henry";
String y = "Henry";
System.out.println(x == y);    // true
```

* If you perform a action that **creates a new String object**, it **will not** be stored on the String Pool, since it's not a literal/constant. </br>Basically when you use `new` (or use a methods that does this) you're telling Java: "Don't use String Pool!"

```java
String x = "Henry";
String z = " Henry".trim();
System.out.println(x == z); // false
```

* You can "force" Java to use the String Pool by using the `intern()` method

```java
String name = "Hello World";
String name2 = new String("Hello World").intern();
System.out.println(name == name2);     // true
```

The intern() method will use an object in the string pool if one is present. If the literal is not yet in the string pool, Java will add it at this time

**PS**: Remember that **compile-time constant** (without `new()`) automatically **gets placed in the string pool**

```java
// Two compile-time constant WITHOUT new
String first = "rat" + 1;
String second = "r" + "a" + "t" + "1";
System.out.println(first == second); //true

// compile-time constant WITH new
String third = "r" + "a" + "t" + new String("1");
System.out.println(first == second); //false

// Works when we force String Pool
System.out.println(first == third.intern());
```

-> **New People:** _Important topic_, look at the book for more in-depth explanation and more examples.

---
### Understanding Java Arrays
array is an area of memory on the heap with space for a designated number of elements, is an ordered list

**PS:** We can create arrays of primitive types but the **array itself is a reference type**

---
#### Creating an Array of Primitives

```java
int[] myAar = new int[3];

//element [0, 0, 0]
//index   [0, 1, 2]
```

Here we have (left to right):

* `int`: Type of array
* `[]`: Array Symbol (Required)
* `[3]`: Size of array

**Things to keep in Mind**

* When we create an array, all elements are set to the <a href="#c2-default-initialization">default value</a>, in case of int it's `0`
* The indexes also starts from 0

##### Creating array specifying all the elements it should start out with

```java
int[] numbers2 = {42, 55, 99}; //Possible (called anonymous array)
int[] numbers2 = new int[] {42, 55, 99}; //Also Possible (but redundant)

//element [42, 55, 99]
//index   [0,  1,  2]
```

The second example is redundant because java already knows the type and array size when you specify the values, so you can ommit it (first example)

---
##### Another syntaxes to create arrays

```java
int[] numAnimals;
int numAnimals4[];
int      [] 
		numAnimals2; //In Java spaces and line breaks doesn't matter
```

* You can use <a href="#c2-multiple-variables">multiple declaration</a> with arrays also

```java
int[] ids, types; //Creates 2 arrays

int ids[], types; //Creates 1 int array and 1 int primitive
```

---
#### Creating an Array with Reference Variables
You can choose any Java type to be the type of the array

```java
String [] bugs = { "cricket", "beetle", "ladybug" };
String [] alias = bugs;
System.out.println(bugs.equals(alias));     // true

//Arrays doesn't implement equals, so it compares memory reference
``` 

The equals() method on arrays **does not look at the elements** of the array, arrays don't implement equals, so **it compares array memory reference**

* Since array can hold reference types, we can point them to another places but we should keep in mind the casting rules

```java
3: String[] strings = { "stringValue" };
4: Object[] objects = strings;
5: String[] againStrings = (String[]) objects; // Casting
6: againStrings[0] = new StringBuilder();   // DOES NOT COMPILE (Builder is not a String type)
7: objects[0] = new StringBuilder();        // COMPILES (Builder inherit from Object, like ALL OTHER objects in Java)

//PS: last case compiles but throws exception since we have an array of objects that are Strings and no StringBuilders
```

---
#### Using an Array

```java
4: int mine = {99};
5: System.out.println(mine.length);          // 1
6: System.out.println(mine0]);               // 99
6: System.out.println(mine[1]);              // OutOfBounds exception
6: System.out.println(mine[mine.length]);    // OutOfBounds exception
```

* Remember that **indexes are different from length**. Index starts from 0 so the last index position is always `length - 1`

---
#### Sorting
We can sort an array by providing a bunch of sort methods

* Remember we should import array before using it

```java
import java.util.*;          // import whole package including Arrays
import java.util.Arrays;     // import just Arrays
```

* Sorting using `int` type: sorts in Asc Order

```java
int[] numbers = { 6, 9, 1 };
Arrays.sort(numbers); // 1, 6, 9
```

* Sorting using `String` type: sorts in alphabetic order

```java
String[] strings = { "10", "9", "100" };
Arrays.sort(strings); // 10 100 9 (1 sorts before 9)
```

Alphabetic Order: Numbers sort before letters, and uppercase sorts before lowercase, in case you were wondering

:bangbang: **Exam Tip:**
> We can create custom sort orders by using `Comparator`, it should be covered latter

---
#### Searching
Java also provides a convenient way to search—but **only if the array is already sorted** (ASC Order)

Scenario | Result
------- | -------
Target element found in sorted array | Index of match
Target element not found in sorted array | Negative value showing one smaller than the negative of the index, where a match needs to be inserted to preserve sorted order
Unsorted array | A surprise—this result isn’t predictable

```java
3: int[] n = {2,4,6,8};
4: System.out.println(Arrays.binarySearch(n, 2)); // 0
5: System.out.println(Arrays.binarySearch(n, 4)); // 1
6: System.out.println(Arrays.binarySearch(n, 1)); // -1
7: System.out.println(Arrays.binarySearch(n, 3)); // -2
```

* If the value is not in the vector, it shows **where it would be in the index and adds +1** to this index, and then **prints as negative value** `-`

:bangbang: **Exam Tip:**
> During the exam, you don't need to know the output when the array is not ordered, in this case look for the unpredictable output answer.

---
#### Comparing
Java also provides methods to compare two arrays to determine which is “smaller.”

##### compare()
When using `compare()`, what the return value means:

* A **negative number** means the first array is smaller than the second.
* A **zero** means the arrays are equal.
* A **positive number** means the first array is larger than the second.

---
##### And some rules when comparing arrays of different lengths:

* If both arrays are the **same length** and have the **same values** in each spot in the **same order**, **return zero**
* If all the elements **are the same** but the **second array has extra elements** at the end, **return a negative** number
* If all the elements **are the same** but the **first array has extra elements** at the end, **return a positive** number
* If the **first element that differs is smaller** in the **first array**, **return a negative** number
* If the **first element that differs is larger** in the **first array**, **return a positive number**


---
##### What does smaller mean

* **null** is smaller than any other value
* For **numbers**, normal numeric order applies
* For **strings**, one is smaller if it is a prefix of another
* For **strings/characters**, numbers are smaller than letters
* For **strings/characters**, uppercase is smaller than lowercase

---
##### Compare examples with some rules applied

First array | Second array | Result | Reason
------- | ------- | ------- | ------- 
`{1, 2}` | `{1}` | Positive number | The first element is the same, but the first array is longer
`{1, 2}` | `{1, 2}` | Zero | Exact match
`{"a"}`  | `{"aa"}` | Negative number | The first element is a substring of the second
`{"a"}`  | `{"A"}`  | Positive number | Uppercase is smaller than lowercase
`{"a"}`  | `{null}` | Negative number | null is smaller than a letter

* We can't compare arrays of different types

```java
System.out.println(Arrays.compare(
   new int[] {1}, new String[] {"a"})); // DOES NOT COMPILE
```

---
#### missmatch
If the arrays are equal, mismatch() returns -1. Otherwise, it returns the first index where they differ

```java
System.out.println(Arrays.mismatch(new int[] {1}, new int[] {1})); //-1
System.out.println(Arrays.mismatch(new String[] {"a"}, new String[] {"A"})); //0
System.out.println(Arrays.mismatch(new int[] {1, 2}, new int[] {1})); //1
```

<!-- Colocar no menu -->
##### equals() vs compare() vs mismatch()

Method | When arrays are the same | When arrays are different
------- | ------- | -------
`equals()`   | true | false
`compare()`  | 0    | Positive or negative number
`mismatch()` | -1   | Zero or positive index

---
#### Varargs
We can pass arrays as a different way for methods

```java
public static void main(String[] args)
public static void main(String args[])
public static void main(String... args) // varargs
```

---
#### Creating a Multidimensional Array
There are some ways to declare multiple arrays

```java
int[][] vars1;          // 2D array
int vars2 [][];         // 2D array
int[] vars3[];          // 2D array
int[] vars4 [], space [][];  // a 2D AND a 3D array

String [][] rectangle = new String[3][2]; // 2D array initializing values
rectangle[0][1] = "set"; // Accessing a 2D array position
```

* We can create different multi-dimensional arrays

```java
// Creating a "sparsely" multi-dimensional array
int[][] differentSizes = {{1, 4}, {3}, {9,8,7}};

// Initializing just an array’s first dimension and define the size of each array component in a separate statement
int [][] args = new int[4][];
args[0] = new int[5];
args[1] = new int[3];
```

#### Using a Multidimensional Array
```java
//For
int[][] twoD = new int[3][2];

for (int i = 0; i < twoD.length; i++) {
   for (int j = 0; j < twoD[i].length; j++)
      System.out.print(twoD[i][j] + " "); // print element
      
   System.out.println(); // new row
}

//For-each
for (int[] inner : twoD) {
   for (int num : inner)
      System.out.print(num + " ");
      
   System.out.println(); // new row
}
```

---



