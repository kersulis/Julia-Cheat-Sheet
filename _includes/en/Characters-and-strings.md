|                                                |                                             |
| ---------------------------------------------- | ------------------------------------------- |
| Character                                      | `chr = 'C'`                                 |
| String                                         | `str = "A string"`                          |
| Loop through characters                        | `for c in str`<br>&emsp;`println(c)`<br>`end` |
| Concatenation                                  | `str = "Learn" * " " * "Julia"`             |
| String interpolation                           | `a = b = 2`<br>`println("a * b = $(a*b)")`  |
| First matching character or regular expression | `findfirst(isequal('i'), "Julia") == 4`     |
| Replace substring or regular expression        | `replace("Julia", "a" => "us") == "Julius"` |
| Last index (of collection)                     | `lastindex("Hello") == 5`                   |
| Number of characters                           | `length("Hello") == 5`                      |
| Regular expression                             | `pattern = r"l[aeiou]"`                     |
| Subexpressions                                 | `str = "+1 234 567 890"`<br>`pat = r"\+([0-9]) ([0-9]+)"`<br>`m = match(pat, str)`<br>`m.captures == ["1", "234"]` |
| All occurrences                                | `[m.match for m = eachmatch(pat, str)]`     |
| All occurrences (as iterator)                  | `eachmatch(pat, str)`                       |

Strings are immutable.
