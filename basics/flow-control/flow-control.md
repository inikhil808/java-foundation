Flow control is how Java decide what will be executed next in the program at runtime based on the conditions, iteratives and transfer statements.

### Type of statements

#### Selection statements
#### 1. If else
```java
if(b) {
   //executed if b is true 
}
else {
    // execute if b is false
}
```
> The argument to if statement should be boolean type and if anything else is provided it will results in Compilation Error.

Question?
What will be the output
```java
    int a = 10;
    if(a) {
        return a + 1;
    }
    else {
        return a - 1;
    }
```

Answer
> This will return CE: incompatible types required boolean provided boolean. 

Question?
What will be the output
```java
    int a = 10;
    if(a = 20) {
        return a + 1;
    }
    else {
        return a - 1;
    }
```

Answer
> This will return CE: incompatible types required boolean provided boolean. 

Question?
What will be the output
```java
    boolean a = false;
    if(a = true) {
        return "Hello";
    }
    else {
        return "No Hello";
    }
```

Answer
> This will print Hello since the assignment before the if condition was checked.
- switch()

---
#### Iterative statements
- for
- while
- do-while
- for each

#### Transfer statements
- break
- continue
- return
- try-catch block
- assert

