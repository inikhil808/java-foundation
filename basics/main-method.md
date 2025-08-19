Whether class contains main method or not and whether main method is declared according to requirement or not, these things won't be checked by compiler.

At runtime JVM is responsible to check these things, if JVM unable to find main method than we will get runtime exception saying `NoSuchMethod: main`.

At runtime JVM always search for the `main()` method with the following prototype.

```java
 public static void main(String[] args)
```

Why public?

To allow calling the JVM from anywhere.

Why static?

Without the existence of the object JVM will need to call this method.

Why void?

`main()` method will not return anything to JVM.

Why is the name main?

This is the name configured inside JVM.

What is String array as the method input?

These are command line argument.

> Any changes in the declaration of the main method will results in RuntimeException saying `NoSuchMethodError: main`


#### Acceptable changes

Eventhough the above syntax very strict following changes are acceptable.

1. Instead of public static we can take static public i.e the order of modifiers is not important.
2. We can take any valid Java identifier for the args. Example `main(String[] var)`
3. We can replace String array with var arg parameter. `main(String... args)`

#### Allowed modifiers

We can declare main method with the following modifiers
- final
- synchronized
- strictfp


```java

//Valid main method

    class Test {
        public static final synchronized strictfp void main(String... nikhil){

        }
    }
```