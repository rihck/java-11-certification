## Summary
Intro
---


- We'll be using [this Book](https://www.amazon.com/gp/product/B08DF4R2V9/ref=ppx_yo_dt_b_d_asin_title_o00?ie=UTF8&psc=1) to study to the certification.


Chapters
---

- <a href="#chapter1">1 - Welcome to Java</a>
	+ <a href="#questions-chapter1">Review Questions</a>

Extra
---

- <a href="#otherQuestions">Other questions to practice</a>

---
<a id="chapter1"/></a>
### _Chapter 1:  Welcome to Java_ 
#### Comments: 
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
####  Class structure
* You can put two classes in the same file. When you do so, at most one of the classes in the file is allowed to be public. If you do have a public class, it needs to match the filename.
* If one class is referring another that IS NOT at the same package, you should `import` specifying the package the class is
* If the class is referring another that IS in the same package, you don't need to `import` it

##### Ordering elements in a class:

Element | Example | Required? | Where does it go? |
--- | --- | --- | ---
Package declaration | package abc; | No | First line in the file
Import statements | import java.util.* | No | Immediately after the package (if present)
Class declaration | public Class A | Yes | Immediately after the import (if any)
Field declarations | int value; | No | Any top-level element in a class
Method declarations | void method(); | No | Any top-level element in a class
 

-------
####  Main method
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
#### JAVAC CLI 
* You use to compile a `.java` file into `.class` file, so it run anywhere using JVM
	
```java
//Compiling one class
javac Zoo.java

//Compiling 2 classes in different packages (folders)
javac packagea/ClassA.java packageb/ClassB.java

//Compiling with Wildcards (It will compite all .java files in both packages)
javac packagea/*.java packageb/*.java
```

* `javac` Options you need to know for the exam:

Option | Description | 
--- | --- 
| -cp <classpath> <br/>  -classpath <classpath> <br/> --class-path <classpath> | Location of classes needed to compile the program

-------
####  JAVA CLI
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
	
* In Java 11 We can run our java classes without actually having to compile it (no `.class` files will be generated).
```java
//You must write the `.java` extension
java Zoo.java
```

* This feature is called launching **single-file source-code programs**
But there are some conditions do to this:

Full Command | Single-file-source-code command | 
--- | --- 
javac HelloWorld.java <br/> java HelloWorld| java HelloWorld.java | 
Produces a class file | Fully in memory
For any program | For programs with one file
Can import code in any available Java library | Can only import code that came with the JDK

* `java` Options you need to know for the exam:

Option | Description | 
--- | --- 
| -cp <classpath> <br/>  -classpath <classpath> <br/> --class-path <classpath> | Location of classes needed to compile the program
| -d <dir> | Directory to place generated class files


-------
#### Wildcards
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
#### Redundant Imports
* There’s one special package `java.lang`, this package is automatically imported **(we don't need to explicit import it)**. Inside this package we can find the `System` class for example

-------
#### Conflict Imports
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

#### Code Formatting on the Exam
Not all questions will include package declarations and imports. Don’t worry about missing package statements or imports unless you are asked about them.

* The following are common cases where you don’t need to check the imports: 
	+ Code that begins with a class name 
	+ Code that begins with a method declaration 
	+ Code that begins with a code snippet that would normally be inside a class or method 
	+ Code that has line numbers that **don’t begin with 1**


