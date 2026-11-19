# Bug reports for exercise2.py

Line: 13
Problem: The `clamp` function incorrectly uses `max(low, min(x, low))`. It should use `max(low, min(x, high))` to ensure the value is bounded between `low` and `high`, not between `low` and `low`. This causes the function to always return `low` if `x` is less than or equal to `low`, which is correct, but when `x` is greater than `low`, it incorrectly clamps to `low` instead of `high`.
Example: For `clamp(10, 5, 15)`, the current code returns `max(5, min(10, 5)) = max(5, 5) = 5`, but it should return `10`. For `clamp(20, 5, 15)`, it returns `max(5, min(20, 5)) = 5`, which is correct, but the logic is flawed because `min(x, low)` is always `low` when `x >= low`, so it never uses `high`.
Fix: Line 13 should be `return max(low, min(x, high))`
