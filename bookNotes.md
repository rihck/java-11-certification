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

####  Class structure
* You can put two classes in the same file. When you do so, at most one of the classes in the file is allowed to be public. If you do have a public class, it needs to match the filename.
* If one class is referring another that IS NOT at the same package, you should `import` specifying the package the class is
* If the class is referring another that IS in the same package, you don't need to `import` it

####  Main method
* The main() method lets the JVM call our code. If it doesn't have, the `java` CLI command will throw an error
* The base signature of main method is:
	
	```java
	// The "public static void main" part is mandatory and should be like this to be considered a main method
	public static void main(String[] args){}
	```	
But there are 3 possible ways to change the array parameter
	```java
	String[] args
	String args[]
	String... args;
	```
You can also change the parameter name
```java
String[] options
String options []
String... options;
```
	* The args you receive on main starts with 0, if you want to access the first param you should do `args[0]`
	
#### JAVAC CLI 
* You use to compile a `.java` file into `.class` file, so it run anywhere using JVM
	
```java
javac Zoo.java
```

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

	- Your class should NOT reference external classes
	- Your program should have only 1 file
	- Your classes can just refer classes from `java.util` (code that came with JDK)

#### Wildcards
* Classes in the same package are often imported together. You can use a shortcut to import all the classes in a package.

```java
 // imports java.util.Random among other things
import java.util.*;
//Every class in the java.util package is available to this program when Java compiles it.
```
* **==It doesn’t import child packages (is not recursive), fields, or methods;==** it imports only classes. (There is a special type of import called the static import that imports other types, which we’ll learn more about in Chapter 7.)

 




