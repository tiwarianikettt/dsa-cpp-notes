A number system is a way of representing numbers using a set of digits.

| Number System | Base | Digits |
| --- | --- | --- |
| Decimal | 10 | `0–9` |
| Binary | 2 | `0, 1` |
| Octal | 8 | `0–7` |
| Hexadecimal | 16 | `0–9, A–F` |

### Binary:

The binary number system has a base of 2 and it only use 0 and 1.

#### Place values in binary:

In decimal, the place values are the powers of 10.

```
10⁰  10¹  10²  10³
 1   10   100  1000
```

In binary, they are powers of 2.

```
2⁰  2¹  2²  2³  2⁴
 1   2   4   8   16
```

For example: 1011
The decimal value of this binary digit will be :

```
  1    0    1    1
  ↓    ↓    ↓    ↓
  8    4    2    1
  
  1011₂
= 1×8 + 0×4 + 1×2 + 1×1
= 8 + 0 + 2 + 1
= 11₁₀
```

#### Binary to Decimal value:

To convert binary to decimal we multiply each binary digit by its corresponding power of 2 and add the results.

Example: 11001 into decimal

```
= 1×2⁴ + 1×2³ + 0×2² + 0×2¹ + 1×2⁰
= 16 + 8 + 0 + 0 + 1
= 25

11001₂ = 25₁₀
```

#### Decimal to Binary:

To convert decimal into binary, we repeatedly divide the number by 2 until the quotient becomes 0.

Then, The remainders are read from bottom to top to obtain the binary number.

Example: 13 into binary:

```
13 ÷ 2 = 6 remainder 1
6 ÷ 2 = 3 remainder 0
3 ÷ 2 = 1 remainder 1
1 ÷ 2 = 0 remainder 1

Now we go from down to up.
the binary will be: 1101.
```

```
💡Note:

When converting decimal to binary using division, **read the remainders from bottom to top**.

```

#### Binary Counting:

```
Decimal    Binary
0          000
1          001
2          010
3          011
4          100
5          101
6          110
7          111
8          1000

Leading zeros are added to maintain a fixed number of bits.
```

Binary counting works just like decimal counting, but there are only two digits.