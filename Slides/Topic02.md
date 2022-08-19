# CSCI100
# Dr. Ning Zhang
# Topic 2: Binary and Digital Images

![binary joke](https://i.imgur.com/zzyXX5m.jpg)

# 2.1 Bit
+ Bit – **Bi**nary Digi**t**
+ Bit is the smallest unit of storage.
+ Bit is a digit that can have only two values: 0 or 1.

### 2.1.1 How Many Patterns Can One Bit Hold?

|Number of bits|Distinct Patterns|
|----|----|
|1|0,1|

### 2.1.2 How Many Patterns Can Two Bits Hold?
|Number of bits|Distinct Patterns|
|----|----|
|1|0,1|
|2|00,01,10,11|

### 2.1.3 How Many Patterns Can Three Bits Hold?
|Number of bits|Distinct Patterns|
|----|----|
|1|0,1|
|2|00,01,10,11|
|3|000,001,010,011 <br> 100,101,110,111|

+ Q: Can you find the formula? 
<details>
    <summary>Click to see the answer!</summary>
  
    **2^n**, 2 to the power of n, where n is the number of bits.
</details>

## 2.2 Bit v.s. Byte
+ Bit is too small to be much use.
+ Group `8 bits` into a `byte`.

![bit vs byte](https://4.bp.blogspot.com/-17MDkedGL_8/WfwkTk_-4LI/AAAAAAAABL0/RGhGT5X5SaMSezBJkFETdHt1BkT0YTv3ACLcBGAs/w1200-h630-p-k-no-nu/bytes-wide-768x238.png)

### 2.2.1 How Many Patterns Can One Byte Hold?
+ 1 bit: $2^1 = 2$ patterns.
+ 2 bit: $2^1 = 4$ patterns.
+ 3 bit: $2^1 = 8$ patterns.
+ 4 bit: $2^1 = 16$ patterns.
+ 5 bit: $2^1 = 32$ patterns.
+ 6 bit: $2^1 = 64$ patterns.
+ 7 bit: $2^1 = 128$ patterns.
+ 8 bit: $2^1 = 256$ patterns.
+ Mathematically, n bits yields $2^n$ patterns ( 2 to the nth power).

### 2.2.2 How to store a number in a byte?
+ Start with 0, go up, **one pattern per number**, until run out of patterns(256).
+ 0,1,2,3,4,5,...,254,255
+ One byte holds a number from 0...255.

## 2.3 Binary vs. Decimal
### 2.3.1 Decimal
+ Decimal notation uses 10 digits: **0,1,2,3,4,5,6,7,8,9**

![decimal](https://www.dlsweb.rmit.edu.au/Toolbox/Calculations/resources/ref_calc/images/ref_decimals.gif)

### 2.3.2 Binary

+ Binary notation uses 2 digits: **0,1**

![binary](https://www.mathsisfun.com/numbers/images/binary-number.svg)
