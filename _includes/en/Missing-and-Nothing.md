|                               |                                                                                         |
| ----------------------------- | --------------------------------------------------------------------------------------- |
| Null value                    | `nothing`<br>`ismissing.(A) # boolean matrix indicating missing elements of Array A`    |
| Missing data                  | `missing`<br>`isnothing.(A) # boolean matrix indicating elements of A that are nothing` |
| Not a Number (floating point) | `NaN`                                                                                   |
| Filter missings               | `collect(skipmissing([1, 2, missing])) == [1, 2]`                                       |
| Replace missings              | `collect((df[:col], 1))`                                                                |
| Check if missing              | `ismissing(x)` (**not** `x == missing`)                                                 |
