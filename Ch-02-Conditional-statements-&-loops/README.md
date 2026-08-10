### Conditional Statements:

Conditional statements are used to make decisions in a program. They allow the program to execute different blocks of code depending on whether a specified condition is **true** or **false**.

#### if Statement:

The `if` statement executes a block of code only if the given condition is true.

Syntax:

```cpp
if (condition) {
	// code
}
```

```cpp
#include <iostream>
using namespace std;

int main() {
    int n = 20;
     if (n > 10) {
        cout << n << " is greater than 10" << endl;
     }
}

// Output:
// 20 is greater than 10
```

#### if-else Statement:

Used when there are two possible outcomes.

Syntax:

```cpp
if (condition) {
	// code
} else {
		//code
	}
```

```cpp
#include <iostream>
using namespace std;

int main() {
    int n = 20;
     if (n > 10) {
        cout << n << " is greater than 10" << endl;
     } else {
        cout << n << " is smaller than or equal to 10" << endl;
     }
    return 0;
}

// Output:
// 20 is greater than 10
```

#### else-if Ladder:

Used when there are multiple conditions.

Syntax:

```cpp
if (condition) {
	// code
}
else if (condition) {
	//code
} 
else {
	//code
}
```

```cpp
#include <iostream>
using namespace std;

int main() {
    int n = 10;
     if (n > 10) {
        cout << n << " is greater than 10" << endl;
     } else if (n == 10){
        cout << n << " is equal to 10" << endl;
     } else {
        cout << n << " is smaller than 10" << endl;
     }
    return 0;
}

// Output:
// 10 is equal to 10
```

#### Ternary Statement:

They are used to write our if-else statement in a single line.

Syntax:

```cpp
condition ? statement-1 : statement-2;

// If the condition is true then statement-1 will run
// if the condition is false then statement-2 will run.
```

```cpp
#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "Enter a number: ";
    cin >> n;

    n > 0 ? cout << "the number is positive" : "the number is negative or zero";
    return 0;
}

// Output:
// Enter a number: 3
// the number is positive
```

### Loops:

Loops are used to execute a block of code **repeatedly** until a specified condition becomes false.

Instead of writing the same code multiple times, we can use loops to perform repetitive tasks efficiently.

#### **Types of Loops**

C++ provides three types of loops:

- `for` Loop
- `while` Loop
- `do-while` Loop

#### While Loop:

The `while` loop executes as long as the given condition is true.

Syntax:

```cpp
while(condition){
    // code
}
```

```cpp
#include <iostream>
using namespace std;

int main() {
    int count = 1;
    while (count <= 10) {
        cout << count << " ";
        count++;
    }
    return 0;
}

// Output:
// 1 2 3 4 5 6 7 8 9 10 
```

#### For Loop:

The `for` loop is used when the number of iterations is known beforehand.

Syntax:

```cpp
for(initialization; condition; update){
    // code
}
```

```cpp
#include <iostream>
using namespace std;

int main() {
    
    for(int i = 1; i <= 10; i++) {
        cout << i << " ";
    }
    return 0;
}

// Output:
// 1 2 3 4 5 6 7 8 9 10 
```

```
💡Note:

Break Statement:

The `break` statement immediately terminates the nearest loop or `switch` statement.
```

```cpp
    #include <iostream>
    using namespace std;

    int main() {
        
        int n;
        cout << "Enter your number: ";
        cin >> n;
        int sum = 0;
        for(int i = 1; i <= n; i++) {
            sum += i;
            if (i == 5)
            {
                break;
                // by this the statement will automatically stop when i will be equal to 5.
            }
            
        }
        cout << sum;
        return 0;
    }

    // Output:
    // Enter your number: 10
    // 15
```



#### do-While Loop:

The `do-while` loop executes the loop body **at least once**, even if the condition is false.

Syntax:

```cpp
do{

    // code

}while(condition);
```

```cpp
int i = 1;

do{
    cout << i << endl;
    i++;
}while(i <= 5);

// Output:
// 1
// 2
// 3
// 4
// 5
```

#### Nested Loops:

A loop inside another loop is called a nested loop.

Nested loops are commonly used to generate patterns and solve problems involving rows and columns.

```css
#include <iostream>
using namespace std;

int main() {
    
    int n;
    cout << "Enter your number: ";
    cin >> n;

    for (int i = 1; i <= n; i++)
    {
        for (int j = 1; j <= n; j++)
        {
            cout << i;
        }

        cout << endl;
        
    }
    
    return 0;
}

// Output:
// Enter your number: 5
// 11111
// 22222
// 33333
// 44444
// 55555
```