# Cpp most useful Functions

## `Array`

```cpp
std::array<int, 5> arr = {1, 2, 3, 4, 5};
// size of the array
arr.size();
// Iterating over the array
for (int i : arr) { code }
// Sorting the array
sort(arr.begin(), arr.end());
// Finding an element
auto it = std::find(arr.begin(), arr.end(), 3);
if (it != arr.end()) {
// index of the element
std::distance(arr.begin(), it) ;
} else {code }
// reverse
std::reverse(arr.begin(), arr.end());
// get min
auto minElement = std::min_element(arr.begin(), arr.end());
// get max
auto maxElement = std::max_element(arr.begin(), arr.end());
```

## `Vectors`

```cpp
std::vector<int> vec = {1, 2, 3, 4, 5};
// size of the vector
vec.size();
// Iterating over the vector
for (int i : vec) { code }
// Sorting the vector
std::sort(vec.begin(), vec.end());
// Finding an element
auto it = std::find(vec.begin(), vec.end(), 3);
if (it != vec.end()) {
    // index of the element
    std::distance(vec.begin(), it);
} else { code }
// Adding elements to the vector
vec.push_back(6);
vec.insert(vec.begin() + 2, 7);
// Removing elements from the vector
vec.pop_back();
vec.erase(vec.begin() + 3);
// reverse
std::reverse(vec.begin(), vec.end());
// max element from vectro
int max_element = *max_element(vect.begin(), vect.end());
// min element from vector
int min_element = *min_element(vect.begin(), vect.end());
```

---

<table>
<thead>
<tr>
<th>
<p dir="ltr" style="text-align: center"><span>Vector Function</span></p>
</th>
<th>
<p dir="ltr" style="text-align: center"><span>Description</span></p>
</th>
</tr>
</thead>
<tbody>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorpush_back-vectorpop_back-c-stl/"><span>push_back()</span></a></p>
</th>
<td><span>Adds an element to the end of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorpush_back-vectorpop_back-c-stl/"><span>pop_back()</span></a></p>
</th>
<td><span>Removes the last element of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorempty-vectorsize-c-stl/"><span>size()</span></a></p>
</th>
<td><span>Returns the number of elements in the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-max_size-function-in-c-stl/"><span>max_size()</span></a></p>
</th>
<td><span>Returns the maximum number of elements that the vector can hold.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-resize-c-stl/"><span>resize()</span></a></p>
</th>
<td><span>Changes the size of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorempty-vectorsize-c-stl/"><span>empty()</span></a></p>
</th>
<td><span>Checks if the vector is empty.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectoroperator-vectoroperator-c-stl/"><span>operator[]</span></a></p>
</th>
<td><span>Accesses the element at a specific position.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorat-vectorswap-c-stl/"><span>at()</span></a></p>
</th>
<td><span>Accesses the element at a specific position, with bounds checking.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorfront-vectorback-c-stl/"><span>front()</span></a></p>
</th>
<td><span>Accesses the first element of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorfront-vectorback-c-stl/"><span>back()</span></a></p>
</th>
<td><span>Accesses the last element of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorbegin-vectorend-c-stl/"><span>begin()</span></a></p>
</th>
<td><span>Returns an iterator pointing to the first element of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorbegin-vectorend-c-stl/"><span>end()</span></a></p>
</th>
<td><span>Returns an iterator pointing to the past-the-end element of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-rbegin-and-rend-function-in-c-stl/"><span>rbegin()</span></a></p>
</th>
<td><span>Returns a reverse iterator pointing to the last element of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-rbegin-and-rend-function-in-c-stl/"><span>rend()</span></a></p>
</th>
<td><span>Returns a reverse iterator pointing to the element preceding the first element of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-cbegin-vector-cend-c-stl/"><span>cbegin</span></a></p>
</th>
<td><span>Returns const_iterator to beginning&nbsp;</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-cbegin-vector-cend-c-stl/"><span>cend</span></a></p>
</th>
<td><span>Returns const_iterator to end</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorcrend-vectorcrbegin-examples/"><span>crbegin</span></a></p>
</th>
<td><span>Returns const_reverse_iterator to reverse beginning</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorcrend-vectorcrbegin-examples/"><span>crend</span></a></p>
</th>
<td><span>Returns const_reverse_iterator to reverse end</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-insert-function-in-cpp-stl/"><span>insert()</span></a></p>
</th>
<td><span>Inserts elements at a specific position in the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-erase-and-clear-in-cpp/"><span>erase()</span></a></p>
</th>
<td><span>Removes elements from a specific position or range in the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectorat-vectorswap-c-stl/"><span>swap()</span></a></p>
</th>
<td><span>Swaps the contents of the vector with those of another vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-erase-and-clear-in-cpp/"><span>clear()</span></a></p>
</th>
<td><span>Removes all elements from the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-emplace-function-in-c-stl/"><span>emplace()</span></a></p>
</th>
<td><span>Constructs and inserts an element in the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vectoremplace_back-c-stl/"><span>emplace_back()</span></a></p>
</th>
<td><span>Constructs and inserts an element at the end of the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-assign-in-c-stl/"><span>assign()</span></a></p>
</th>
<td><span>Assigns new values to the vector elements by replacing old ones.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-capacity-function-in-c-stl/"><span>capacity()</span></a></p>
</th>
<td><span>Returns the size of the storage space currently allocated to the vector.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/using-stdvectorreserve-whenever-possible/"><span>reserve()</span></a></p>
</th>
<td><span>Requests that the vector capacity be at least enough to contain a specified number of elements.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-shrink_to_fit-function-in-c-stl/"><span>shrink_to_fit()</span></a></p>
</th>
<td><span>Reduces memory usage by freeing unused space.</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/vector-data-function-in-c-stl/"><span>data()</span></a></p>
</th>
<td><span>Returns a direct pointer to the memory array used internally by the vector to store its owned elements.&nbsp;</span></td>
</tr>
<tr>
<th>
<p dir="ltr" style="text-align: center"><a href="https://www.geeksforgeeks.org/get_allocator-in-cpp/"><span>get_allocator</span></a></p>
</th>
<td><span>Returns a copy of the allocator object associated with the&nbsp;vector.</span></td>
</tr>
</tbody>
</table>

---

## `deque`

```cpp
std::deque<int> dq = {1, 2, 3, 4, 5};
// size of the deque
dq.size();
// Iterating over the deque
for (int i : dq) { code }
// Sorting the deque
std::sort(dq.begin(), dq.end());
// Finding an element
auto it = std::find(dq.begin(), dq.end(), 3);
if (it != dq.end()) {
    // index of the element
    std::distance(dq.begin(), it);
} else { code }
// Adding elements to the deque
dq.push_back(6);
dq.push_front(0);
dq.insert(dq.begin() + 2, 7);
// Removing elements from the deque
dq.pop_back();
dq.pop_front();
dq.erase(dq.begin() + 3);
// reverse
std::reverse(dq.begin(), dq.end());
```

---

<table class="GFGEditorTheme__table">
<colgroup>
<col>
<col></colgroup>
<thead>
<tr>
<th class="GFGEditorTheme__tableCell GFGEditorTheme__tableCellHeader"><span>Function</span></th>
<th class="GFGEditorTheme__tableCell GFGEditorTheme__tableCellHeader"><span>Description</span></th>
</tr>
</thead>
<tbody>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setbegin-setend-c-stl/"><span>begin()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns an iterator to the first element in the set.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setbegin-setend-c-stl/"><span>end()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns an iterator to the theoretical element that follows the last element in the set.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setrbegin-and-setrend-in-c-stl/"><span>rbegin()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns a reverse iterator pointing to the last element in the container.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setrbegin-and-setrend-in-c-stl/"><span>rend()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns a reverse iterator pointing to the theoretical element right before the first element in the set container.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-crbegin-and-crend-function-in-c-stl/"><span>crbegin()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns a constant iterator pointing to the last element in the container.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-crbegin-and-crend-function-in-c-stl/"><span>crend()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns a constant iterator pointing to the position just before the first element in the container.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-cbegin-and-cend-function-in-c-stl/"><span>cbegin()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns a constant iterator pointing to the first element in the container.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-cbegin-and-cend-function-in-c-stl/"><span>cend()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns a constant iterator pointing to the position past the last element in the container.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setsize-c-stl/"><span>size()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns the number of elements in the set.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-max_size-function-in-c-stl/"><span>max_size()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns the maximum number of elements that the set can hold.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setempty-c-stl/"><span>empty()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns whether the set is empty.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-insert-function-in-c-stl/"><span>insert(const g)&nbsp;</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Adds a new element ‘g’ to the set.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-insert-function-in-c-stl/"><span>iterator insert (iterator position, const g)</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Adds a new element ‘g’ at the position pointed by the iterator.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/seterase-c-stl/"><span>erase(iterator position)&nbsp;</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Removes the element at the position pointed by the iterator.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/seterase-c-stl/"><span>erase(const g)</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Removes the value ‘g’ from the set.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setclear-c-stl/"><span>clear()&nbsp;</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Removes all the elements from the set.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setkey_comp-in-c-stl/"><span>key_comp()</span></a><span> /</span><a href="https://www.geeksforgeeks.org/set-value_comp-function-in-c-stl/"><span> value_comp()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns the object that determines how the elements in the set are ordered (‘&lt;‘ by default).</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-find-function-in-c-stl/"><span>find(const g)</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns an iterator to the element ‘g’ in the set if found, else returns the iterator to the end.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-count-function-in-c-stl/"><span>count(const g)</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns 1 or 0 based on whether the element ‘g’ is present in the set or not.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-lower_bound-function-in-c-stl/"><span>lower_bound(const g)</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns an iterator to the first element that is equivalent to ‘g’ or definitely will not go before the element ‘g’ in the set.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-upper_bound-function-in-c-stl/"><span>upper_bound(const g)</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns an iterator to the first element that will go after the element ‘g’ in the set.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-equal_range-function-in-c-stl/"><span>equal_range()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>The function returns an iterator of pairs. (key_comp). The pair refers to the range that includes all the elements in the container which have a key equivalent to k.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setemplace-c-stl/"><span>emplace()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>This function is used to insert a new element into the set container, only if the element to be inserted is unique and does not already exist in the set.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-emplace_hint-function-in-c-stl/"><span>emplace_hint()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns an iterator pointing to the position where the insertion is done. If the element passed in the parameter already exists, then it returns an iterator pointing to the position where the existing element is.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/setswap-c-stl/"><span>swap()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>This function is used to exchange the contents of two sets but the sets must be of the same type, although sizes may differ.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-operator-in-c-stl/"><span>operator=</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>The ‘=’ is an operator in C++ STL that copies (or moves) a set to another set and set::operator= is the corresponding operator function.</span></td>
</tr>
<tr>
<td class="GFGEditorTheme__tableCell"><a href="https://www.geeksforgeeks.org/set-get_allocator-in-c-stl/"><span>get_allocator()</span></a></td>
<td class="GFGEditorTheme__tableCell"><span>Returns the copy of the allocator object associated with the set.</span></td>
</tr>
</tbody>
</table>

---

## `list`

```cpp
std::list<int> myList;

// Insertion functions
myList.push_back(5); // Adds an element to the end of the list
myList.push_front(2); // Adds an element to the beginning of the list
myList.insert(myList.begin(), 8); // Inserts an element at a specific position

// Access functions
int firstElement = myList.front(); // Returns the first element of the list
int lastElement = myList.back(); // Returns the last element of the list

// Modification functions
mylist.sort();
myList.pop_back(); // Removes the last element of the list
myList.pop_front(); // Removes the first element of the list
myList.erase(myList.begin()); // Removes an element at a specific position
myList.clear(); // Removes all elements from the list

// Size functions
int listSize = myList.size(); // Returns the number of elements in the list
bool isEmpty = myList.empty(); // Checks if the list is empty

// Iteration functions
for (auto it = myList.begin(); it != myList.end(); ++it) {
    // Access and modify elements using the iterator
    int element = *it;
    *it = element + 1;
}

```
