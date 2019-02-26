# Java Cheat Sheet

<!-- <details><summary>Data Structures</summary> -->

## ArrayLists
### __Initialize using Interfaces__
```java
List<Element> list = new ArrayList();
```
### __Methods__

* <details><summary> add(E e) </summary>
  <pre><code>// Add Element e to list
  add(E e);             @return {boolean}
  </code></pre>
  </details>

* <details><summary> add(int i, E e) </summary>
  <pre><code>// Add Element e into list at position i
  add(int i, E e);      @return {void}
  </code></pre>
  </details>

* <details><summary> clear() </summary>
  <pre><code>// Clear list
  clear();              @return {void}
  </code></pre>
  </details>

* <details><summary> clone() </summary>
  <pre><code>// Creates a clone of current list
  clone();              @return {Object} 
  </code></pre>
  </details>

* <details><summary> contains(Object o) </summary>
  <pre><code>// Return true if Object o exists in list
  contains(Object o);   @return {boolean} 
  </code></pre>
  </details>

* <details><summary> get(int index) </summary>
  <pre><code>// Returns element at index index
  get(int index);       @return {E}
  </code></pre>
  </details>

* <details><summary> indexOf(Object o) </summary>
  <pre><code>// Return index of Object o
  indexOf(Object o)     @return {int}
  </code></pre>
  </details>

* <details><summary> remove(int index) </summary>
  <pre><code>// Removes element at index index
  remove(int index);    @return {E}
  </code></pre>
  </details>

* <details><summary> remove(Object o) </summary>
  <pre><code>// Removes Object o. Returns true if successful
  remove(Object o);     @return {boolean}
  </code></pre>
  </details>

* <details><summary> size() </summary>
  <pre><code>// Returns size of list
  size();               @return {int}
  </code></pre>
  </details>

* <details><summary> toArray() </summary>
  <pre><code>// Maps list to array of list Objects
  toArray();            @return {Object[]}
  </code></pre>
  </details>

</details>
