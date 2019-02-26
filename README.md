# Java Cheat Sheet

<!-- <details><summary>Data Structures</summary> -->

### ArrayLists
Initialize using Interfaces
```java
List<Element> list = new ArrayList();

// Add Element e to list
add(E e);             @return {boolean} 

// Add Element e into list at position i
add(int i, E e);      @return {void}

// Clear list
clear();              @return {void}

// Creates a clone of current list
clone();              @return {Object} 

// Return true if Object o exists in list
contains(Object o);   @return {boolean} 

// Returns element at index index
get(int index);       @return {E}

// Return index of Object o
indexOf(Object o)     @return {int}

// Returns true is list is empty
isEmpty();            @return {boolean}

// Removes element at index index
remove(int index);    @return {E}

// Removes Object o. Returns true if successful
remove(Object o);     @return {boolean}

// Returns size of list
size();               @return {int}

// Maps list to array of list Objects
toArray();            @return {Object[]}
```

</details>
