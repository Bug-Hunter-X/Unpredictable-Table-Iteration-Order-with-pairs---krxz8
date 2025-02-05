# Lua Table Iteration Order Bug

This repository demonstrates a common error in Lua involving the unpredictable order of iteration when using `pairs()` on tables.  Modifying a table while iterating over it with `pairs()` can lead to unexpected results because the order of iteration is not guaranteed.

The `bug.lua` file contains code that recursively traverses a nested table using `pairs()`.  The order of visiting nested tables may differ across Lua implementations or even across different runs of the same code.

The `bugSolution.lua` file presents a solution demonstrating safe table traversal using a different approach (e.g., a manual iteration with indexing or a copy of the table).