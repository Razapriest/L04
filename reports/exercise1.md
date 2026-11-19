# Bug reports for exercise1.py

Line: 3
Problem: The condition `n % 2 == 1` checks if a number is odd, not even. For even numbers, the remainder when divided by 2 should be 0, not 1.
Example: is_even(4) returns False (correct), but is_even(2) returns False (incorrect — 2 is even and should return True); is_even(3) returns True (incorrect — 3 is odd and should return False).
Fix: return n % 2 == 0

Line: 8
Problem: The function calculates the sum of width and height, not the area of a rectangle, which should be width multiplied by height.
Example: rectangle_area(4, 5) returns 9 (incorrect), expected 20.
Fix: return width * height

Line: 13
Problem: The function adds 2 to n, but it should return twice the number (i.e., n multiplied by 2).
Example: double(3) returns 5 (incorrect), expected 6.
Fix: return n * 2
