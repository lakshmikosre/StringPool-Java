# What is the Java String Pool? 

The Java string pool is a mechanism that is used to optimize memory usage in Java. When a string object is created in Java, it is stored in the string pool if a string with the same value already exists in the pool. If a string with the same value does not exist in the pool, a new string object is created and stored in the pool. 
String pool is a storage space in the Java heap memory where string literals are stored. It is also known as String Constant Pool or String Intern Pool. It is privately maintained by the Java String class. By default, the String pool is empty. A pool of strings decreases the number of String objects created in the JVM, thereby reducing memory load and improving performance.

# How Does the Java String Pool Work? 
When a string is created using a string literal, such as "Hello, World!", the Java runtime checks to see if an instance of the string with the same value already exists in the string pool. If a matching string is found, a reference to that string is returned. If a matching string is not found, a new string object is created and added to the pool. 
Here's an example: 

String str1 = "Hello, World!"; 
String str2 = "Hello, World!"; 
System.out.println(str1 == str2); // true 
In this example, str1 and str2 both reference the same object in the string pool because they have the same value. 
