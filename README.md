## Overview
This project involves designing a digital circuit that calculates the floor of the square root of an 8-bit binary input. The circuit uses the Binary Search algorithm to achieve efficient computation with minimal clock cycles. The result is output in Binary Coded Decimal (BCD) format and displayed on a 7-segment display.

## Task
To find the floor of the square root of a binary number (8-bits maximum).

## Skills
Digital Circuit Design, Proteus, Algorithm, Optimization.

## Approach
+ Set Initial Bounds: Start by setting the lower bound (low) to 0 and the upper bound (high) to the given number (or 0 if the number is 0).
+ Find the Midpoint: Calculate the midpoint of the current bounds.
+ Compare and Adjust:
  + If the square of this midpoint equals the given number, you’ve found the exact square root.
  + If the square of the midpoint is less than the given number, move the lower bound up to just above the midpoint.
  + If the square of the midpoint is greater than the given number, move the upper bound down to just below the midpoint.
+ Repeat the Process: Continue adjusting the bounds and finding new midpoints until the lower bound exceeds the upper bound.
+ Determine the Result: When the loop ends, the upper bound will be the largest integer whose square is less than or equal to the given number. This value is the floor of the square root.
+ Convert the result to Binary Coded Decimal (BCD) format.
+ Output the BCD result to a 7-segment display for visualization.

## Main Circuit
![image](https://github.com/user-attachments/assets/d93f447d-9917-4c0f-b372-45ea0c532d18)

![image](https://github.com/user-attachments/assets/1854beea-5b1b-4749-a225-5970769b9a70)

## Sub Circuit
![image](https://github.com/user-attachments/assets/18de234b-f554-438f-9d9e-a87fe180b5ef)

![image](https://github.com/user-attachments/assets/d8ea1631-9403-4cc9-a40a-2f7b5e3c4fce)
