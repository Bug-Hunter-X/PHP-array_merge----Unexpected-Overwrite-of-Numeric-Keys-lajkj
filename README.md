# PHP array_merge() Unexpected Behavior with Numeric Keys

This repository demonstrates a subtle issue in PHP's `array_merge()` function when dealing with arrays containing numeric keys.  When merging arrays with overlapping numeric keys, `array_merge()` overwrites values from the first array with those from the second, instead of preserving both values.  This can lead to unexpected data loss and errors if not carefully considered.

The `bug.php` file showcases the problematic behavior. The `bugSolution.php` demonstrates a solution using `array_replace()` which handles overlapping keys differently.

This example highlights the importance of understanding how PHP handles array key collisions when merging arrays.