## Type of Variables
There are mutliple ways to categorise variables in java. 

### Categorisation on the basis of type

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
