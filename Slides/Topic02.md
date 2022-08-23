# CSCI100
# Dr. Ning Zhang
# Topic 2: Binary and Digital Image

# Part I: Binary 

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
+ 2 bit: $2^2 = 4$ patterns.
+ 3 bit: $2^3 = 8$ patterns.
+ 4 bit: $2^4 = 16$ patterns.
+ 5 bit: $2^5 = 32$ patterns.
+ 6 bit: $2^6 = 64$ patterns.
+ 7 bit: $2^7 = 128$ patterns.
+ 8 bit: $2^8 = 256$ patterns.
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


+ Binary vs. Decimal

![binary vs decimal](http://shortrope.com/wp-content/uploads/2015/04/Binary-Primer.png)

### 2.3.3 ASCII
+ ASCII Table

![ASCII](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/ASCII-Table-wide.svg/875px-ASCII-Table-wide.svg.png)

+ Example

![ASCII example](https://computerscienceiseasy.com/wp-content/uploads/2021/01/ASCII-example.png)

## 2.4 Kilobyte, Megabyte, Gigabyte, Terabyte

![kb mb....](http://itcflm.weebly.com/uploads/5/8/3/5/58352013/560677_orig.png)

### 2.4.1 Kilobyte or KB
+ Kilobyte KB - about 1 thousand bytes.
+ A small email text is about 2KB.
+ Text does not take a lot of bytes to store compared to image or video.

### 2.4.2 Megabyte or MB
+ Megabyte MB - about 1 million bytes.
+ MP3 audio is about 1 megabyte per minute.
+ A high quality digital picture is about 2-5 megabytes.

### 2.4.3 Gigabyte or GB
+ Gigabyte GB - about 1 billion bytes
+ A standard definition (SD) movie that you download to your device for streaming tends to be between 1 GB and 2 GBs, while high definition (HD) videos are twice that, ranging from 2 to 4 Gigabytes.
+ An ordinary computer might have 8GB RAM.

### 2.4.4 Terabyte or TB
+ Terabyte TB - about 1,000,000,000,000 bytes
+ You can buy TB hard drives today.
+ We are just beginning the time.

### 2.4.5 Why Does My SSD Show up as Smaller than Advertised?
[Link](https://www.crucial.com/support/articles-faq-ssd/ssd-showing-smaller-than-advertised)

## 2.5 More Number Systems
### 2.5.1 Octal numbers
+ Octal notation uses 8 digits: **0,1,2,3,4,5,6,7**

![octal](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200918224440/Octal-to-Decimal-Conversion1.png)

### 2.5.2 Hexadecimal numbers

![hex in computer](https://cdn.sparkfun.com/assets/learn_tutorials/2/1/0/hex-intro.png)

+ Hex notation uses 15 digits: **0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F**
+ Software developers and system designers widely use hexadecimal numbers because they provide a human-friendly representation of binary-coded values. Each hexadecimal digit represents four bits (binary digits), also known as a nibble (or nybble).

![HEX](https://www.w3resource.com/w3r_images/csharp-basic-image-exercise-30.png)


# Part II: Digital Image
+ Digital images are everywhere.
+ Digital image: lots of numbers in the computer.

![digital image](https://www.dspguide.com/graphics/F_23_1.gif)

## 2.6 Pixels
+ An image is made of many pixels.
+ Each pixel is a small square that shows a single color.
+ An image of 800 pixels wide and 600 pixels high has 800 × 600 = 480,000 pixels.

![pixel](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRYeigAiVh9qBkI4UjfUpXXxDlQxUIXkKka5WWYHx5Gd7UO4BftaNnIRuOWoscMz26iBHk&usqp=CAU)

### 2.6.1 How to represent the color of a pixel?
+ The `red/green/blue(RGB)` scheme/model is one popular way of representing a color in the computer.
+ In RGB, every color is defined as a particular combination of pure red, green, and blue light.
+ Each pixel has 3 numbers to define its RGB color.

![RGB](https://cdn.educba.com/academy/wp-content/uploads/2019/05/RGB-Color-Model.jpg)

#### 2.6.1.1 RGB – three numbers
+ Any color can be made by combining red/green/blue.
+ Any color can be represented by three numbers.
+ A number is in the range [0,255].
+ Each of the red, green and blue light levels is encoded as a number in the range 0..255, with 0 meaning zero light and 255 meaning maximum light.

![rgb table](https://excelatfinance.com/xlf/media/xlf-colindx2ws.png)

+ [Try more combinations](https://www.w3schools.com/colors/colors_picker.asp)

#### 2.6.1.2 Mystery of digital image
+ We can start with a whole digital image of something. Then break it down into small square pixels.
+ Then each pixel breaks down to 3 numbers in the range of [0, 255].
+ This is a typical computer pattern – something whole is broken down and represented as a lot of little numbers.

### 2.6.2 Other Color Systems
+ [CMYK](https://en.wikipedia.org/wiki/CMYK_color_model)
+ [Pantone](https://en.wikipedia.org/wiki/Pantone)
+ [RAL](https://en.wikipedia.org/wiki/RAL_colour_standard)
+ [RGB vs. CMYL vs. Pantone vs. RAL](https://snowball.digital/blog/color-systems-cmyk-pantone-rgb-and-ral-explained)


# References
[Stanford CS101](https://web.stanford.edu/class/cs101/bits-bytes.html)
[why are text files 4kb?](http://unix.stackexchange.com/questions/62049/why-are-text-files-4kb)
