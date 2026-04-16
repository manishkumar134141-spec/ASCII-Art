# ASCII-Art
A technical deep dive into image processing, pixel mapping, and metaprogramming for the Minor II Project.

# ASCII-Art Generator

## 📌 Overview
This repository contains the **Minor II Project**, an exploration into computer graphics and text-based image representation. It is a technical deep dive into **image processing**, **pixel mapping**, and **metaprogramming** using Python. The project takes standard image files (like `.ppm`) and translates their visual data into ASCII art by evaluating pixel intensity and mapping it to a corresponding typographic character.

## ✨ Features
* **Image Processing:** Reads and parses image files to extract RGB pixel data.
* **Luminance Evaluation:** Converts color pixels into grayscale values to determine the relative brightness of each pixel.
* **Pixel-to-ASCII Mapping:** Maps the brightness values to a carefully selected string of ASCII characters (from dark to light) to recreate the image using text.
* **Algorithmic Efficiency:** Utilizes metaprogramming and efficient data handling to process the image arrays and generate the output quickly.

## 🛠️ Technologies Used
* **Python 3:** The primary programming language used for scripting and logic.

## ⚙️ How it Works
1. **Input:** The script accepts an image file (e.g., `karina kappor.ppm`).
2. **Read & Resize:** The image data is loaded into memory. Depending on the terminal or output size constraints, the image may be scaled down while maintaining its aspect ratio.
3. **Grayscale Conversion:** Each pixel's RGB (Red, Green, Blue) values are averaged or weighted to find its overall luminance (brightness).
4. **Character Assignment:** The grayscale value (typically ranging from 0 to 255) is mapped to an index in an ASCII character string (e.g., `` `^",:;Il!i~+_-?][}{1)(|\\/tfjrxnuvczXYUJCLQ0OZmwqpdbkhao*#MW&8%B@$ ``). Darker pixels are assigned denser characters (like `@` or `#`), while lighter pixels are assigned sparser characters (like `.` or ` `).
5. **Output:** The resulting characters are printed line by line, rendering the final ASCII art.

## 🚀 Usage
*(You can add instructions here on how someone can run your `minor2_project.py` script locally!)*
