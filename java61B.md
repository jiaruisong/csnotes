# Phrase One: Java
## static vs non static
1. non-static: AKA instance method. every instance can have their own way. So if want to call the method on a instance, the method must be non-static
2. Static methods can't access "my" instance variables, because there is no "me".

"new" can initiate a instance or creates an array
```java
Dog[] dogs = new Dog[2];  //create an array of dogs of size 2.
dogs[0] = new Dog(8); //create a dog instance into a array.
```
## Phlisophy: helper function and decoupling
use helper method/ function to decouple complicated part of program