# Java basics

Class is a a either a library of static methods or a data type definition

# Primitive data types
1. integer (arithmetic operations) 
    - short 16-bit
    - int 32-bit
    - long 64-bit
    - byte 8-bit
3. real number (arithmetic operations)
    - float 32-bit (single-precision)
    - double 64-bit
5. boolean (logical operations)
    - boolean 
7. Characters 
    - char 16-bit


Type conversion
- a cast



Operations can be combined into expressions
- Precedence
- Comparison (mixed-type operation)
    - equal
    - not equal
    - greater/less than (or equal)

- Shortcut notations

Variables are 
- named with identifiers
- assosiated with a data type and store one of the permissible data-type values


Statements allow for 
1. creation and assigment of variables, 
2. controlling execution flow 
3. or causing side affects

Types of statemts include
1. Declaration 
    - (java is strongly-typed)
    - scope within a block
3. Assignments
4. conditionals
5. loops
6. calls
7. returns

Compiled to java bytecode using javac command 
Run using java command 

Overloaded operations specify different operations on a new data-type

Property of primitive operations
- an operation involving values of a given type has a value of that type

Expression
- typicaly infix, prefix, postfix

# Arrays
- Values of the same type
- **Operations** : Declare, initialize & index
- T\[\] = new T\[n\]
- T\[\] = {1,2,3,4,5}
- Aliasing
- An array of objects is a an array of references to the objects.
    - If ojects are lagre: efficiency improves when objects are not moved aroung
    - If objects are small: efficiency is deminished by the requirement to follow a reference each time.


# Properties of methods
- arguments are **passed by value** (arrays are **aliased** -> values of the calling codes array is changed, but not the array itself). meaning, the method works with the value of the argument, not the argument itself. change the value of the argument in a static method has not effect on the calling code.
- method named can be **overloaded**
- can have **side effects**
    - consume input
    - produce output
    - change enteries in an array
    - change the state of the system
- has **single return value**, but can have multiple return statemenets
- *Instance* vs *Static*

A basic model for java programming is to develop a program that addresses a specific computational task by creating a library of static methods, one of which is named `main()`

# Modular programming
- libraries of static methods i.e. **modules** where a static method in on library can call a static method in another library.
- Advantage
    - With with modules of resonable size, even in program involving a large amout of code
    - Share and reuse code without reimplementation
    - Easily substitute improved implementations
    - Develop appropriate abstract models for addressing probramming problems
    - Localize debugging

Unit testing
Java libraries
External libraries
APIs
Documentation



# Strings
- Sequence of characters
- not primitive data type
- def `"string here"`
- Concatenation `"Ac" + "Bc"` becomes`"AcBc"`
- Conversion from string to number
    - `static int parseInt(String s)`
    - `static int parseDouble(String s)`
- Conversion from number to string
    - `static String toString(int i)`
    - `static String toString(double d)`
- Automatic conversion
    - omit use of `toSting(...)` in concatenation of a String with none-string data type
- Formatting


# Input and Output
- Standard input stream
- Standard output stream

# Objects
- an entity that can take on a data-type value
- characterized by
    - *state*
    - *identity*
    - *behaviour*
- An *assignment statement* with a reference type creates a *copy of the refererence*. i.e. **Aliasing**-

# Class
- All classes are subclasses of the `Object` class
- All class have inherited methods from `Object` class
    - `toString()` : string representation of this object
    - `hashCode()` : hashcode for this object
    - `equals()` : is this object equal to that
    - `getClass()` : what class is this object

- A class *A* can be used by another class *B*, provided one of the following:
    - the source code is in a `.java` file, in the same directory
    - the class *A* is in the standard library
    - the class *A* is imported into class *B*

## Constructur
- Each time a client uses `new()`, the system
    1. Allocates memory space for the object
    2. Invokes the constructor to initilize its value
    3. Returns a reference to the object._
# Enum
# Interface

## Inharitence
- subtyping using *interface inheritence*
- subclassing using *implmenetation inheritence* (works against encapsulation)
- 


We can use == operators for reference comparison (address comparison) and .equals() method for content comparison.