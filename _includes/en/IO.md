|                   |                                                                                                                                                                              |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Read stream       | `stream = stdin`<br>`for line in eachline(stream)`<br>`    # do stuff`<br>`end`                                                                                              |
| Read file         | `open(filename) do file`<br>`    for line in eachline(file)`<br>`        # do stuff`<br>`    end`<br>`end`                                                                   |
| Read CSV file     | `using CSV`<br>`data = CSV.read(filename)`                                                                                                                                   |
| Write CSV file    | `using CSV`<br>`CSV.write(filename, data)`                                                                                                                                   |
| Save Julia Object | `using JLD`<br>`save(filename, "object_key", object, ...)`                                                                                                                   |
| Load Julia Object | `using JLD`<br>`d = load(filename) # Returns a dict of objects`                                                                                                              |
| Save HDF5         | `using HDF5`<br>`h5write(filename, "key", object)`                                                                                                                           |
| Load HDF5         | `using HDF5`<br>`h5read(filename, "key")`                                                                                                                                    |
| Read MAT file     | `using MAT`<br>`vars = matread(path::String)`                                                                                                                                |
| Read CSV file     | `using CSV`<br>`CSV.File(path::String)`{:.julia}<br><br>`# load into DataFrame`<br>`using CSV, DataFrames`{: .language-julia}<br>`df = CSV.File(path::String) |> DataFrame!` |
| Read image file   | `using FileIO`<br>`img = load(path::String)`                                                                                                                                 |
