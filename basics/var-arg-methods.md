### Var Arg Methods (Variable Arguments Methods)

Until 1.4 version we couldn't declare method with variable number of arguments.

We can declare var-arg method using the syntax below.

```java
 // We can call this method by passing any number of int value including zero number.

 m1(int... x) 
```

Calling Syntax 

```java
m1(10, 20, 30);
```

Internally var arg parameter will be converted into one dimensional array. Hence within the var arg method we can differentiate values by using index.

Example
```java
// declaration
public static int sum(int... x) {
    int total = 0;
    for(int val: x) {
        total = total + x;
    }
    return total;
}

// Usage example 1
    int[] arr = {1, 2, 3, 4};
    sum(arr);

// Usage example 2
    sum(1, 2, 3, 4);
```

Varargs must be the last parameter in the method; you can have other fixed parameters before it.

**Real Life Use Case**

``` java
// Example declaration
public static String format(String format, Object... args)

//Example Usage
String text = String.format("ID: %d, Name: %s", 101, "Alice");

```


### Performance Consideration
**Array Creation Overhead:** Every time a varargs method is called, Java internally creates a new array to hold the arguments. If the method is called frequently (such as in a tight loop or performance-critical code), this repeated array allocation can increase pressure on the garbage collector and slow down execution.