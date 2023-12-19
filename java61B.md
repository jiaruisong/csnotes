# Phrase One: Java
## static vs non static
non-static: AKA instance method. every instance can have their own way. So if want to call the method on a instance, the method must be non-static

```java
public static void printIndexed(String word){
    for (int i = word.length() - 1; i >= 0; i--){
        System.out.println(word.charAt(i) + i);
    }
}

```