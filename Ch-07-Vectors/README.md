A **vector** is a dynamic array provided by the C++ Standard Template Library (STL).

Unlike a normal array, a vector can **automatically grow or shrink in size** during program execution.

To use vectors, include:

```cpp
#include <vector>
```

### Creating a Vector:

Syntax:

```cpp
vector<data_type> vector_name;
```

Example:

```cpp
vector<int> v;
```

This creates an empty integer vector.

You can also initialize it with values:

```cpp
vector<int> v = {10, 20, 30, 40};
```

### Array vs Vector:

| Array | Vector |
| --- | --- |
| Fixed size | Dynamic size |
| Size generally decided at creation | Can grow/shrink |
| Built-in data structure | STL container |
| `int arr[5]` | `vector<int> v` |
| Limited built-in operations | Provides many useful functions |

Example:

Array:

```cpp
int arr[5];
```

Vector:

```cpp
vector<int> v;
```

The vector can later have elements added to it.

### Adding Elements — `push_back()` :

`push_back()` adds an element to the **end of the vector**.

```cpp
vector<int> v;

v.push_back(10);
v.push_back(20);
v.push_back(30);
```

The vector becomes:

```cpp
// 10 20 30
```

Example:

```cpp
#include <iostream>
#include <vector>
using namespace std;

int main()
{
    vector<int> v;

    v.push_back(10);
    v.push_back(20);
    v.push_back(30);

    return 0;
}

// v will be: [10, 20, 30]
```

### Accessing Elements:

Vectors use **indexing**, just like arrays.

```cpp
vector<int> v = {10, 20, 30, 40};

cout << v[0];

// Output:
// 10
```

Indexes:

```
Index:   0   1   2   3
Value:  10  20  30  40
```

So:

```cpp
v[2]
```

gives:

```
30
```

### `size()` :

The `size()` function returns the **number of elements currently present in the vector**.

```cpp
vector<int> v = {10, 20, 30, 40};

cout << v.size();

// Output:
// 4
```

You can use it while traversing:

```cpp
for (int i = 0; i < v.size(); i++)
{
    cout << v[i] << " ";
}
```

### Taking Vector Input:

You can use `push_back()` with a loop:

```cpp
vector<int> v;
int n;

cout << "Enter the number of elements: ";
cin >> n;

for (int i = 0; i < n; i++)
{
    int x;
    cin >> x;

    v.push_back(x);
}
```

### `pop_back()` :

`pop_back()` removes the **last element** of the vector.

```cpp
vector<int> v = {10, 20, 30, 40};

v.pop_back();
```

Now:

```
v will become: 10 20 30
```

Important:

> `pop_back()` removes the element but **does not return the removed element**.
> 

### `front()` and `back()` :

#### `front()` :

Returns the first element:

```cpp
cout << v.front();
```

#### `back()` :

Returns the last element:

```cpp
cout << v.back();
```

For:

```cpp
vector<int> v = {10, 20, 30, 40};
```

```
front() → 10
back()  → 40
```

### Checking Whether a Vector is Empty:

Use:

```cpp
v.empty();
```

It returns:

```
true  → vector is empty
false → vector is not empty
```

#### Traversing a Vector:

Using normal `for` loop

```
for (int i = 0; i < v.size(); i++)
{
    cout << v[i] << " ";
}
```

Using range-based `for` loop

```cpp
for (int value : v)
{
    cout << value << " ";
}
```

### `resize()` :

`resize()` changes the **number of elements** in the vector.

#### Increase the size:

```cpp
vector<int> v = {10, 20, 30};

v.resize(5);
```

Now the vector has 5 elements:

```
10 20 30 0 0
```

The newly created integer elements are initialized to `0`.

#### Decrease the size:

```cpp
v.resize(2);
```

Now:

```
10 20
```

The extra elements are removed.

### `insert()` :

`insert()` adds an element at a **specific position**.

Example:

```cpp
vector<int> v = {10, 20, 30};

v.insert(v.begin() + 1, 15);
```

Now:

```
10 15 20 30
```

Here:

```cpp
v.begin() + 1
```

represents the position of index `1`.

So:

```
Index:   0   1   2
Before:  10  20  30

Insert 15 at index 1

Index:   0   1   2   3
After:   10  15  20  30
```

### `erase()` :

`erase()` removes an element from a specific position.

Example:

```cpp
vector<int> v = {10, 20, 30, 40};

v.erase(v.begin() + 1);
```

The element at index `1` (`20`) is removed.

#### Removing a range:

You can also remove multiple elements:

```cpp
v.erase(v.begin() + 1, v.begin() + 3);
```

This removes elements from the first iterator **up to, but not including, the second iterator**.

### `capacity()` :

`capacity()` tells you how many elements the vector can currently hold **without allocating additional memory**.

Example:

```cpp
vector<int> v;

v.push_back(10);
v.push_back(20);

cout << v.capacity();
```

The exact capacity is implementation-dependent, so **don't rely on a specific number**.

### `size()` vs `capacity()` :

This distinction is important:

```
size()     → number of elements currently present
capacity() → number of elements that can currently fit
```

For example, conceptually:

```
size = 3
capacity = 4
```

means:

```
Elements currently stored → 3
Space currently available → 1 more element
```

### `v[i]` — Accessing an Element:

`v[i]` is used to **access the element at index `i`** in a vector.

Example:

```cpp
vector<int> v = {10, 20, 30, 40, 50};

cout << v[2];

// Output:
// 30
```

### Functions Table:
| Function / Syntax | Purpose                                           | Example                     |
| ----------------- | ------------------------------------------------- | --------------------------- |
| `v[i]`            | Access or modify element at index `i`             | `v[2]`                      |
| `push_back()`     | Adds an element at the end                        | `v.push_back(10)`           |
| `pop_back()`      | Removes the last element                          | `v.pop_back()`              |
| `size()`          | Returns the number of elements                    | `v.size()`                  |
| `front()`         | Returns the first element                         | `v.front()`                 |
| `back()`          | Returns the last element                          | `v.back()`                  |
| `empty()`         | Checks whether the vector is empty                | `v.empty()`                 |
| `clear()`         | Removes all elements                              | `v.clear()`                 |
| `resize()`        | Changes the number of elements                    | `v.resize(5)`               |
| `insert()`        | Adds an element at a specific position            | `v.insert(v.begin()+1, 15)` |
| `erase()`         | Removes element(s) from a specific position/range | `v.erase(v.begin()+1)`      |
| `capacity()`      | Returns the current storage capacity              | `v.capacity()`              |


### Static vs Dynamic Allocation:

#### Static Allocation:

In **static allocation**, the memory size is fixed and generally decided before the program runs.

Example:

```cpp
int arr[5] = {10, 20, 30, 40, 50};
```

Here:

- Size = `5`
- The size cannot be changed during execution.
- Memory is allocated for 5 integers.

You cannot do:

```cpp
arr[5] = 60;  // outside the array
```

#### Dynamic Allocation:

In **dynamic allocation**, memory can be allocated during program execution, and the size can be determined at runtime.

A vector is a common C++ DSA example:

```cpp
vector<int> v;

v.push_back(10);
v.push_back(20);
v.push_back(30);
```

The vector can grow as elements are added.