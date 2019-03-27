# Java Cheat Sheet

## ArrayLists
<details><summary>ArrayLists</summary>

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

## HashMaps
<details><summary>HashMaps</summary>

### __Initialize using Interfaces__
```java
Map<Element,Element> map = new HashMap();
```

### __Methods__

* <details><summary> put(K key, V value) </summary>
  <pre><code>// Adds Key key Value value mapping to map
  put(K key, V value);  @return {V}
  </code></pre>
  </details>

* <details><summary> get(Object key) </summary>
  <pre><code>// Returns Value V associated with key
  get(Object key);  @return {V}
  </code></pre>
  </details>

* <details><summary> getOrDefault(Object key, V defaultValue) </summary>
  <pre><code>// Returns Value V associated with key or defaultValue if map contains no mapping for key
  getOrDefault(Object key, V defaultValue);  @return {V}
  </code></pre>
  </details>

* <details><summary> isEmpty() </summary>
  <pre><code>// Returns true if map is empty
  isEmpty();  @return {boolean}
  </code></pre>
  </details>

</details> 
<!-- End of HashMaps -->

## MergeSort
```java
class mergesort {

    public static void merge(int[] arr, int[] l, int[] r, int left, int right) {
        int l_index = 0;
        int r_index = 0;
        int arr_index = 0;

        while(l_index < left && r_index < right) {
            if(l[l_index] < r[r_index]) {
                arr[arr_index++] = l[l_index++];
            } else {
                arr[arr_index++] = r[r_index++];
                count++;
            }
        }

        while(l_index < left) {
            arr[arr_index++] = l[l_index++];
        }

        while(r_index < right) {
            arr[arr_index++] = r[r_index++];
        }
    }

    public static void mergeSort(int[] arr, int n) {
        if(n <= 1) return;
        int mid = n/2;
        int[] l = new int[mid];
        int[] r = new int[n-mid];

        for(int i = 0; i < mid; i++) {
            l[i] = arr[i];
        }

        for(int i = mid; i < n; i++) {
            r[i-mid] = arr[i];
        }

        mergeSort(l, mid);
        mergeSort(r, n-mid);

        merge(arr, l, r, mid, n-mid);
    }

    public static void print(int[] arr) {
        for(int num : arr) {
            System.out.print(num + " ");
        }
        System.out.println();
    }
    public static void main(String[] args) {
        int[] test = new int[] {5, 4, 3, 2, 7};
        print(test);
        mergeSort(test, test.length);
        print(test);
    }
}
```
<!-- End of MergeSort -->