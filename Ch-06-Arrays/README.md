An **array** is a collection of elements of the **same data type**, stored in **contiguous memory locations**.
    
    ```cpp
    int arr[5] = {10, 20, 30, 40, 50};
    
    // Here:
    // arr → name of the array
    // 5 → size of the array
    // 10, 20, 30, 40, 50 → elements
    // Indexing starts from 0
    ```
    
    ### Declaring an Array:
    
    Syntax:
    
    ```cpp
    data_type array_name[sizze];
    ```
    
    Example:
    
    ```cpp
    int arr[5];
    
    // This creates an integer array capable of storing 5 integers.
    ```
    
    ### Initializing an Array:
    
    Method 1: Initialize while declaring
    
    ```cpp
    int arr[5] = {10, 20, 30, 40, 50};
    ```
    
    Method 2: Let C++ determine the size
    
    ```cpp
    int arr[] = {10, 20, 30, 40, 50};
    ```
    
    Here the compiler automatically determines that the size is `5`.
    
    ### Accessing Elements:
    
    Use the index of the element.
    
    ```cpp
    cout << arr[0];
    ```
    
    ### Updating an Element:
    
    You can change an element using its index.
    
    ```cpp
    int arr[5] = {10 20 30 40 50}
    arr[2] = 100;
    
    // It will become:
    // 10, 20, 100, 40, 50
    ```
    
    ### Traversing an Array:
    
    To visit every element, we commonly use aa loop:
    
    ```cpp
    int arr[] = {10, 20, 30, 40, 50};
    int size = 5;
    
    for (int i = 0; i < size; i++)
    {
        cout << arr[i] << " ";
    }
    
    // Output:
    // 10 20 30 40 50
    ```
    
    ### Taking Array Input:
    ```jsx
    int arr[5];

        for (int i = 0; i < 5; i++)
        {
            cin >> arr[i];
        }
    ```
