## Type of Variables
There are mutliple ways to categorise variables in java. 

### Categorisation on the basis of type of value

**Primitive Variable** 

Used to store the value of primitive data type i.e int, byte, short etc.

```java
int x = 10
```

Where are the primitive variable stored?

Primitive data types go to either the stack or the heap — depending on where they’re declared.

| Declared As...              | Goes To...                  |
| --------------------------- | --------------------------- |
| Local variable in a method  | **Stack**                   |
| Instance field in an object | **Heap**                    |
| Part of a static field      | **Method Area** (Heap-like) |



**Reference Variable**

Used to store a reference to an object.

```java
class Dog {
    String name;
}

public class Main {
    public static void main(String[] args) {
        Dog d = new Dog();   // 'd' is the reference variable
        d.name = "Buddy";    // accessing object via reference
    }
}
```

Where are the reference variable stored?

The reference variable is stored in stack while the object is stored in the heap.

```lua
[Stack]                    [Heap]
--------                  ------------------
|   d   | --------------> |  Dog Object     |
--------                  |----------------|
                          | name = "Buddy" |
                          ------------------

```

### Categorisation on the basis of variable behaviour

**Instance Variables**

**Static Variables**

**Local Variables**

A local variable is a temporary placeholder for data that can only be accessed within the method or block in which it is declared.


Local variables will be created while executing the block in which it was declared, once the block execution completes automatically the local variable will be destroyed and hence the scope of local variable is the block in which it was declared. 

JVM doesn't provide the default values for local variables and must be initialised before the usage.

Where are the local variables stored?

Stored inside the stack memory.

**Thread Safety of local variables**

Since the local variable lives in stack, each thread has its own copy and no other thread can directly touch it, the local variables are considered thread safe.

```lua
Thread A (Stack)                Thread B (Stack)
+----------------+              +----------------+
| localVar = 10  |              | localVar = 10  |
+----------------+              +----------------+
         |                              |
         V                              V
   (Primitive value)              (Primitive value)
     [No sharing]                   [No sharing]
```