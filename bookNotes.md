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

