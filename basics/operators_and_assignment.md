### Increment and Decrement Operators

**PreIncrement/PreDecrement**

First Assign and than Increment/Decrement
```java
// preIncrement
y = ++x;
// preDecrement
y = --x;
```

**PostIncrement**

First Increment/Decrement and than Assign

```java
//postIncrement
y = x++;

//postDecrement
y = x--;
```

We can apply increment and decrement operators only for variables but not constant values.

```java
y = ++10;
// Results in Compiler Error

y = ++(++x);
// Results in Compiler Error
```

We can apply increment and decrement operators for every primitive type except boolean.



### Arthimetic Operators

If we apply any arthimetic operator between two varibales a and b the result type is always `max(int, type of a, type of b)`

Example 
```java
byte a = 10;
byte b = 20;
byte c = a + b; // Results in Compilation Error, since assigning int value to byte variable.
```


### Assignment Operators
There are 3 types of assignment operator

**Simple Assignment Operator**
```java
int x = 10;
```

**Chained Assignment Operator**
```java
a = b = c = d = 10;
```

**Compound Assignment Operator**
```java
a += 10;
```

> Question: What will be the output of
> ```java
> int a = b = c = 10;
> ```
> This will result in CE: cannot find symbol b.