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
