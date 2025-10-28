# Triangle Analyzer 🛠️

A Python program to analyze triangles based on the lengths of their three sides. The program determines the type of triangle, calculates its perimeter and area, and visualizes the triangle.

## Features

- Input the three sides of a triangle.
- Validate the input to ensure it forms a triangle.
- Determine the triangle type:
  - Not a triangle
  - Equilateral triangle
  - Right triangle
  - Obtuse triangle
  - Acute triangle
  - Isosceles right triangle
  - Isosceles obtuse triangle
  - Isosceles acute triangle
- Calculate the perimeter.
- Calculate the area using **Heron's formula**.
- Display a visual representation of the triangle.
- Large font style for clear readability.

## Algorithm / Approach

1. **Input Validation:** Check that the inputs are positive numbers and satisfy the triangle inequality.
2. **Triangle Type Determination:**
   - Equilateral: all sides equal
   - Isosceles: two sides equal
   - Right: satisfies Pythagorean theorem
   - Acute / Obtuse: based on angles calculated via the law of cosines
3. **Perimeter Calculation:** Sum of all three sides.
4. **Area Calculation:** Using Heron's formula:
   \[
   s = \frac{a+b+c}{2}, \quad
   \text{Area} = \sqrt{s(s-a)(s-b)(s-c)}
   \]
5. **Visualization:** Draw the triangle using a plotting library.
6. **Output:** Display triangle type, perimeter, area, and the figure.

## Example Usage

```python
from triangle_analyzer import analyze_triangle

# Input triangle sides
a = 5
b = 5
c = 5

# Analyze triangle
analyze_triangle(a, b, c)
