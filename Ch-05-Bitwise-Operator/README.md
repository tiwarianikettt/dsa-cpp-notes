Bitwise operators perform operations directly on the **individual bits** of an integer

### Types of Bitwise Operator:

| Operator | Name | Example |
| --- | --- | --- |
| `&` | Bitwise AND | `5 & 3` |
| `|` | Bitwise OR | Bitwise OR |
| `^` | Bitwise XOR | `5 ^ 3` |
| `~` | Bitwise NOT | `~5` |
| `<<` | Left Shift | `5 << 1` |
| `>>` | Right Shift | `5 >> 1` |

#### Bitwise AND:

Returns `1` only when **both bits are 1**.

```
A  B  A & B
0  0    0
0  1    0
1  0    0
1  1    1
```

```cpp
5 & 3 = 1

// As 5=0101 & B=0011 therefore their AND will be 0001.
```

#### Bitwise OR:

Returns `1` when **at least one bit is 1**.

```
A  B  A | B
0  0    0
0  1    1
1  0    1
1  1    1
```

```cpp
5 | 3 = 7

//Here 5=0101 and 3=0011 therefore their OR will be 0111.
```

#### Bitwise XOR:

Returns `1` when the two bits are **different**.

```
A  B  A ^ B
0  0    0
0  1    1
1  0    1
1  1    0
```

```cpp
5 ^ 3 = 6

// Here 5=0101 and 3=0011 therefore their XOR will be 0110.
```

#### Bitwise NOT:

It flips every bit, converts 1 to 0 and 0 to 1.

```cpp
5 = 00000101
~5 = 11111010
```

#### Left Shift:

Moves all bits to the left & the empty space is filled by 0.

```cpp
5 << 1 = 10

// Here 5=0101 we will shift it left by 1 bit hence the answer will be- 1010 which in decimal count is 10.
```

#### Right Shift:

Moves all bits to the right & the empty space is filled by 0.

```css
5 >> 1 = 2

// Here 5=0101 we will shift it right by 1 bit hence the answer will be- 0010 which in decimal count is 2
```