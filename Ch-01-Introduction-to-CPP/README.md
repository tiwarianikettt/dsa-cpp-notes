- **CH-01 Introduction to C++**
    
    ### What is C++ ?
    
    C++ is a **general-purpose, high-level programming language** developed by **Bjarne Stroustrup** at Bell Labs in **1979** as an extension of the C programming language.
    
    It is used to build fast and efficient software ranging from operating systems to games and competitive programming solutions.
    
    #### Features of C++ :
    
    - It is an Object Oriented Programming language.
    - C++ is very high performing it is a compiled language and provides direct memory access.
    - Portable- Programs written in C++ can run on different operating systems with little or no modification.
    - C++ provides the **Standard Template Library (STL)**, which includes ready-to-use data structures and algorithms.
    
    #### Applications of C++ :
    
    C++ is widely used in many industries because of its speed and efficiency.
    
    Common applications are:
    
    | Field | Examples |
    | --- | --- |
    | Operating Systems | Windows, Linux |
    | Game Development | Unreal Engine |
    | Web Browsers | Google Chrome (parts), Firefox (parts) |
    | Databases | MySQL |
    | Embedded Systems | IoT Devices |
    | Finance | High-Frequency Trading Software |
    | Competitive Programming | DSA & Coding Contests |
    | Graphics Software | Adobe Photoshop (parts), Blender (parts) |
    
    #### Structure of C++ program:
    
    ```cpp
    #include <iostream>      // Header File
    
    using namespace std;     // Standard Namespace
    
    int main()               // Main Function
    {
        cout << "Hello World!";
    
        return 0;
    }
    ```
    
    #### Explanation:
    
     #include <iostream>  - Includes the Input-Output Stream library.
    It allows us to use functions like cout, cin.
    
     using namespace std;  - Allows us to use standard library objects without writing `std::` every time.
    
    Without this command:
    
    ```cpp
    std::cout << "Hello";
    ```
    
    With this command:
    
    ```cpp
    cout << "Hello";
    ```
    
     int main()  - The entry point of every C++ program.
    
    Execution starts from the `main()` function.
    
     {  }  - Curly braces define the body of the function.
    
     cout  - It helps in display output.
    
     return0;  - Indicates that the program executed successfully and returns control to the operating system.
    
    ### Flowchart:
    
    A flowchart is a graphical representation of an algorithm or process. It uses standard symbols connected by arrows to show the sequence of steps required to solve the given problem.
    
    Flowcharts help us:
    
    - Understand the logic of a program.
    - Plan a solution before coding.
    - Identify errors in the logic.
    - Explain algorithms more easily.
    
    #### Common symbols of a flowchart:
    
    | Symbol | Name | Purpose |
    | --- | --- | --- |
    | 🟢 Oval | Start/End (Terminal) | Indicates where the program begins or ends. |
    | ▭ Rectangle | Process | Represents calculations, assignments, or processing steps. |
    | ⏢ Parallelogram | Input/Output | Used to take input or display output. |
    | ◇ Diamond | Decision | Represents a condition with two or more possible paths (Yes/No, True/False). |
    | ➜ Arrow | Flow Line | Shows the direction of execution. |
    | ○ Circle | Connector | Connects different parts of a flowchart (used mainly in large flowcharts). |
    
    #### Rules for Drawing a Flowchart:
    
    - Every flowchart should have **one Start** and **one End**.
    - Use arrows to indicate the direction of flow.
    - Keep the flow from **top to bottom** or **left to right**.
    - Every decision should have at least **two branches** (Yes/No or True/False).
    - Keep the flowchart neat and avoid unnecessary crossing arrows.
    
    ### Pseudocode:
    
    It is an informal way to write a code in simple English mixed with programming concepts. Pseudocode does not follow any fixed syntax or programming language rules. It focuses on explaining the logic in simple English.
    
    ### Variables:
    
    They are the containers to store data.
    
    ```cpp
    int age = 25;
    char grade = 'A';
    string name = "Aniket";
    
    // Here age, grade, name are the variables which contains the given value.
    ```
    
    ```
    💡NOTE :
    
    While writing numbers in the variables we don’t use quotes but while writing other alphabets and characters we have to use quotes, for single character we use single quotes ‘ ‘ and for multiple characters we use double quotes “ ”.
    
    Before using variables we have to give the data type to the variable otherwise it will be shown as error in the code. 
    
    ```
    
    ### Identifier:
    
    The name given to the variable container is known as the identifier.
    
    for ex- age=25 here, age is the name given to the container hence it is an identifier.
    
    ### Data Types:
    
    A data type signifies the type of data we are entering in a variable container.
    
    #### Why do we use Data Types?
    
    - To store different kinds of data.
    - To allocate memory efficiently.
    - To perform operations according to the type of data.
    - To improve program accuracy and performance.
    
    #### Different data types in C++ :
    
    | Data Type | Description | Example |
    | --- | --- | --- |
    | `int` | Stores whole numbers | 25 |
    | `float` | Stores decimal values (single precision) | 15.7 |
    | `double` | Stores larger decimal values (double precision) | 25.789654 |
    | `char` | Stores a single character | 'A' |
    | `bool` | Stores logical values | true / false |
    | `void` | Represents no value or no return type | `void display()` |
    
    #### Sizes of different data types:\
    
    | Type | Size (Typical) |
    | --- | --- |
    | int | 4 Bytes |
    | float | 4 Bytes |
    | double | 8 Bytes |
    | char | 1 Byte |
    | bool | 1 Byte |
    
    #### Type Casting:
    
    Converting data from one type to another.
    
    There are two ways for this:
    
    - Conversion: It is an implicit function which means it is the done by the compiler itself.
    
    ```cpp
    float x = 10;
    // Here the compliler will automatically convert x=10 into float data type.
    ```
    
    - Casting: It is an explicit function which means it has to be done by ourselves.
    
    ```cpp
    int x = (int)3.14;
    // Here we have asigned a float data type as integer value data type.
    ```
    
    ### Operators:
    
    Operators are special symbols used to perform mathematical, logical, and data-manipulation operations on variables and values.
    
    Types of Operators:
    
    1. Arithmetic Operator: +, -, *, /, %
    2. Relational Operator: ==, <, ≤, >,≥, ≠
    3. Logical Operator: or ( | | ), and ( && ), not ( ! )
    
    ### Keywords:
    
    Keywords are reserved words that have predefined meanings in C++ and cannot be used as identifiers.
    
    Examples: int, float, if, else, while, for, return, class.