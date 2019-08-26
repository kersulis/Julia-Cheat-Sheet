|                                            |                                                                                                                                      |
| ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| Apply f to all elements of collection coll | `map(f, coll)` or<br>`map(coll) do elem`<br>`    # do stuff with elem`<br>`    # must contain return`<br>`end`                       |
| Filter coll for true values of f           | `filter(f, coll)`                                                                                                                    |
| List comprehension                         | `arr = [f(elem) for elem in coll]`<br>`A = [i + j for i in 1:3, j in 1:4] # example of creating a 3-by-4 array with a comprehension` |
