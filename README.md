# Java Essentials

## Quick Access Links 
1. [Core Syntax](#core-syntax)
    1. [Variables and Data Types](#variables)
    2. [Control Flow](#control-flow)
    3. [Loops](#loops)
2. [Object-Oriented Programming](#oop)
    1. [Classes and Objects](#classes)
    2. [Inheritance](#inheritance)
    3. [Interfaces and Abstract Classes](#interface)
3. [Collections Framework](#collections)
    1. [Lists](#lists)
    2. [Sets](#sets)
    3. [Maps](#maps)
4. [Functional Programming (Java 8+)](#java8)
    1. [Lambda Expressions](#lambda)
    2. [Streams](#streams)
5. [Exception Handling](#expection-handling)
6. [Concurrency](#concurrency)
7. [Modern Java Features (Java 9-17)](#java9-17)
    1. [Records (Java 16+)](#java16)
    2. [Sealed Classes (java 17)](#sealed-classes)
    3. [Text Blocks(Java 15+)](#java15)
    4. [Pattern Matching (java 16+)](#pattern-matching)
8. [Testing with JUnit 5](#testing)
9. [Build Tools](#build)
    1. [Maven (pom.xml)](#maven)
    2. [Gradle (build.gradle)](#gradle)
 

<a name="core-syntax"></a>
## Core Syntax
<a name="variables"></a>
Variables and Data Types

```Java
// Primitive data types
byte b = 127;                     // 8-bit -128 to 127
short s = 32767;                  // 16-bit, -32,768 to 32,767
int i = 2147483647;               // 32-bit -2^31 to 2^31-1
long l = 9223372036854775808L;    // 64-bit, -2^63 to 2^63-1
float f = 3.14f;                  // 32-bit floating point
double d = 3.141592265359         //64-bit floating point
boolean bool = true;              // true or false
char c = 'A';                     // 16-bit Unicode character

//Reference types
String str = "Hello World";       // String literal
Internal num = 42;                // Wrapper class

```
<a name="control-flow"></a>
Control Flow

```java
// if-else statement
if(condition){
    // code block
} else if ( anotherCondition ){
    // code block
} else {
    // code block
}

// Switch statement
switch (variable) {
    case value1:
        // code block
        break;
    case value3:
        // code block
        break;
    default:
        // code block
}

 // Enhanced switch ( Java 14+)
 switch (variable) {
    case value1 -> ;// code or expression;
    case value2 -> ;// code or expression;
    default -> ;// code or expression;
}
```
<a name="loops"></a>
Loops

```Java
// For Loop
for(int i = 0; i < 10; i++){
    // code block
}

// Enhanced for loop (for-each)
for( String item : collection){
    //code block
}

//While loop
while ( condition ){
    //code block
}

// do - while loop
do {
    // code block
} while(condition)
```
<a name="oop"></a>
## Object-Oriented Programming
<a name="classes"></a>
### Classes and Objects
```java
// Classs definition
public class MyClass{
    //Fields
    private int field;

    // Constructor
    public MyClass(int field){
        this.field = field;
    }

    // Methods
    public void setField(int field) {
        this.field = field;
    }
}

// Creating objects
MyClass obj = new MyClss(42);
```
<a name="inheritance"></a>
### Inheritance
```java
// Parent class
public class Parent {
    protected int data;

    public void method() {
        // implementation
    }
}

// Child class
public class Child extenda Parent {
    @Override
    public void method(){
        super.method(); // Call parent's implementation
        // Additional implementation
    }
}
```
<a name="interface"></a>
## Interfaces and Abstract Classes
```java
// Interface
public interface MyInterface {
    void abstractMethod(); // Abstract by default

    default void defaultMethod() {
        // Default implementation
    }
}

// Abstract class
public abstract class AbstractClass {
    public abstract void abstractMethod(); // Must be implemented by subclasses

    public void concreteMethod() {
        // Implementation
    }
}
```

<a name="collections"></a>
## Collections Framework
<a name="lists"></a>
### Lists
```java
// ArrayList
List<String> arrayList = new ArrayList<>();
arrayList.add("item");
String item = arrayList.get(0);

// LinkedList
List<String> linkedList = new LinkedList<>();
linkedlist.add("item");
linkedList.addFirst("first");
linkedList.addLast("last");

```
<a name="sets"></a>
### Sets
```java
// Hashset (unordered)
Set<String> hashSet = new HashSet<>();
hashset.add("item");
boolean contains = hashSet.contains("items")

// TreeSet (sorted)
Set<String> treeSet = new TreeSet<>();
treeSet.add("b");
treeSet.add("a");
// treeSet will be ["a", "b"]

```
<a name="maps"></a>
### Maps
```java
// HashMap
Map<String, Integer> hashMap = new HashMap<>();
hashMap.put("key", 42);
int value = hashMap.get("key");

// TreeMap (sorted by keys)
Map<String, Integer> treeMap = new TreeMap<>();
treeMap.put("b", 2);
treeMap.put("a", 1);
// Keys will be ordered as "a", "b"
```
<a name="java8"></a>
## Functional Programming (Java 8+)
<a name="lambda"></a>
### Lambda Expressions
```java
// Basic lambda
Runnable r = () -> System.out.println("Hello")

// With Parameter
Consumer<String> c = (s) => System.out.println(s);

//With multiple statement
Comparator<String> comp = (s1, s2) -> {
    int result  = s1.length() - s2.length();
    return result  != 0  ? result : s1.compareTo(s2);
};
```
<a name="streams"></a>
### Streams
```java

```
<a name="expection-handling"></a>
## Exception Handling
```java

```
<a name="concurrency"></a>
## Concurrency
```java

```
<a name="java9-17"></a>
## Modern Java Features (Java 9-17)
```java

```
<a name="java16"></a>
### Records (Java 16+)
```java

```
<a name="sealed-classes"></a>
### Sealed Classes (Java 17)
```java

```
<a name="java15"></a>
### Text Blocks (Java 15+)
```java

```
<a name="pattern-matching"></a>
### Pattern Matching (Java 16+)
```java

```
<a name="testing"></a>
## Testing with JUnit 5
```java

```
<a name="build"></a>
## Build Tools
```java

```
<a name="maven"></a>
### Maven (pom.xml)
```java

```
<a name="gradle"></a>
### Gradle (build.gradle)
```java

```
