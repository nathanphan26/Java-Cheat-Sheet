# Java Cheat Sheet

<!-- <details><summary>Data Structures</summary> -->

## ArrayLists
### __Initialize using Interfaces__
```java
List<Element> list = new ArrayList();
```

__Add Element e to list__
```java
add(E e);             @return {boolean} 
```

__Add Element e into list at position i__
```
add(int i, E e);      @return {void}
```

__Clear list__
```
clear();              @return {void}
```

__Creates a clone of current list__
```
clone();              @return {Object} 
```

__Return true if Object o exists in list__
```
contains(Object o);   @return {boolean} 
```

__Returns element at index index__
```
get(int index);       @return {E}
```

__Return index of Object o__
```
indexOf(Object o)     @return {int}
```

__Returns true is list is empty__
```
isEmpty();            @return {boolean}
```

__Removes element at index index__
```
remove(int index);    @return {E}
```

__Removes Object o. Returns true if successful__
```
remove(Object o);     @return {boolean}
```

__Returns size of list__
```
size();               @return {int}
```

__Maps list to array of list Objects__
```
toArray();            @return {Object[]}
```

</details>
