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
  
    $$2^n$$, 2 to the power of n, where n is the number of bits.
</details>

## 2.2 Bit v.s. Byte
+ Bit is too small to be much use.
+ Group `8 bits` into a `byte`.

![bit vs byte](https://4.bp.blogspot.com/-17MDkedGL_8/WfwkTk_-4LI/AAAAAAAABL0/RGhGT5X5SaMSezBJkFETdHt1BkT0YTv3ACLcBGAs/w1200-h630-p-k-no-nu/bytes-wide-768x238.png)

### 2.2.1 How Many Patterns Can One Byte Hold?
+ 1 bit: $2^1 = 2$ patterns.
