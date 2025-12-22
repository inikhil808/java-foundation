Child interface of Collection

### Characteristics
- Duplicates are not allowed.
- Insertion order not required.



### Implementation Classes of List Interface

#### **Hash Set**
Implements Set interface

- Underlying datastructure is **HashTable**
- Implements `Serializable` and `Clonable` interfaces.
- Allows Hetrogenous Objects
- Allows null insertion.
- Insertion order is not preserved.

**Fill Ratio:** The ratio of `occupied buckets/total buckets`

**Load Factor:** The ratio of `number of elements stored/ number of buckets`, this is also used to create a threshold to create a new hashset when the load factor is reached. Default value: 0.75

#### **Linked HashSet**
Child class of HashSet 

- Underlying datastructure is Linked List and HashTable
- Insertion order is preserved: *this is the only difference between HashSet and LinkedHashSet*.


#### **Sorted Set Interface**
Child Interface of Set

- Uses Red Black Tree of type self balancing binary search tree which is used to store elements in a sorted order.
- Duplicates are not allowed.
- Objects should be inserted according to a some sorting order.

Special methods that are offered by Sorted Set
- first(): returns the smallest element
- last(): returns the last element
- headSet(Object o): returns all the elements less than object o
- tailSet(Object o): returns all the elements greator than object o
- subSet(Object o1, Object o2): returns all the element between o1 and o2
- comparator(): returns Comparator object which defines the sorting algorithm used to store the values in set

#### **Navigable Set Interface**
- Child Interface of Sorted Set

- It contains several methods for navigation purposes.
- 


#### **Tree Set Implementation Class**
