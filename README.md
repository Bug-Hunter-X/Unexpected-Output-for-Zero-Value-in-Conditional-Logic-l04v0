# Unexpected Output for Zero Value in Conditional Logic
This repository demonstrates a common JavaScript bug related to the incorrect handling of the zero value in conditional logic. The `foo` function intends to classify numbers as negative, zero, or positive; however, it incorrectly classifies zero as positive.

## Bug
The bug lies in the `else` block of the conditional statement. When the input `x` is 0, the condition `x < 0` is false, leading the code to execute the `else` block and return 1 (positive), not 0 (zero).

## Solution
The solution is to explicitly check if `x` equals 0 as part of the conditional logic before checking if it's negative.