Used to retrieve elements in sequence from Collections.

Three types of cursors available in java:
### Enumeration
We can create enumeration object using the `elements()` method from the vector class. 
```java
    Enumeration e = v.element();
```

Available Methods:
1. hasMoreElements():
2. nextElement():
3. Iterator
4. ListIterator

### Limitations of Enumeration
1. Non Universal Nature: Only applicable for legacy classes, doesn't work for ArrayList, LinkedList etc but works for Vector and Stacks.
2. Doesn't allow for performing `remove` operations.

To overcome above limitation `Iterator` was developed.

### Iterators
- Universal Corsur
- Allows for read and remove operations. 

```java
    // Creation in Java
    List<Integer> list = new ArrayList();
    Iterator it = list.iterator();
```

Available Methods
- public boolean heasNext();
- public Object next();
- public void remove();

### Limitation of Iterators
1. Unidimentional Movement: We can only move towards the forward direction
2. Cannot perform addition, replace objects.


### List Iterator

```java
    // Java Declaration
    ListIterator iterator = l.listIterator();
    // where l is any list object
```

Available Methods 
- Child interface of Iterator so inherits all the Iterators methods
- public boolean hasPrevious();
- public Object previous();
- public int previousIndex();
- public void add(Object o);
- public void set(Object o); 

