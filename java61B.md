# Phrase One: Java
## static vs non static
1. non-static: AKA instance method. every instance can have their own way. So if want to call the method on a instance, the method must be non-static
2. Static methods can't access "my" instance variables, because there is no "me".

"new" can initiate a instance or creates an array
```java
Dog[] dogs = new Dog[2];  //create an array of dogs of size 2.
dogs[0] = new Dog(8); //create a dog instance into a array.
```
## Philosophy: helper function and decoupling
use helper method/ function to decouple complicated part of program

## Reference Type and Primitive Types
There are 8 primitive types in Java:
- byte, short, int, long, float, double, boolean, char 
Everything else, including arrays, is a reference type.

When you declare a variable of a certain type in Java:
- Your computer sets aside exactly enough bits to hold a thing of that type. 
  - Example: Declaring an int sets aside a "box" of 32 bits.
- Java does NOT write anything into the reserved boxes.
  - For safety, Java will not let access a variable that is uninitialized.

For reference type:
Java allocates exactly a box of size 64 bits, no matter what type of object.
These bits can be either set to:
- Null (all zeros).
- The 64 bit "address" of a specific instance of that class (returned by new).

The golden rule:
- b = a **copies the bits** from a into b. 
- Passing parameters copies the bits.