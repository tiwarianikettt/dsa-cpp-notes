A **function** is a block of code designed to perform a specific task.

Instead of writing the same code repeatedly, we can put it inside a function and **call the function whenever needed**.

### Uses of Functions:

- Reduces code repetition.
- Makes code easier to understand.
- Allow us to reuse a code.

#### Syntax:

```cpp
returnType functionName(Parameters)
{
	//code
}
```

#### Example:

```cpp
void printHello()
{
	cout << "Hello";
}

int main()
{
	printHello();
}

// Output:
// Hello
```

```
💡Note:

The functions helps in reducing redundancy in our program.

Redundancy-  Repetion of same thing again & again.

```

### Parameters:

Parameters allows us to pass information into a function.

```cpp
int sum(int a, int b)
{
	int s = a + b;
	return s;
}

int main()
{
	cout << sum(20,30) << endl;
}

// Output:
// 50
```

```
💡Note:

The `return` statement immediately terminates the current function and optionally sends a value back to the caller.

A `return` statement inside a loop immediately terminates the entire function, not just the loop.

When we don’t want to return any value in the function then the return type of that function is named as- void.

```