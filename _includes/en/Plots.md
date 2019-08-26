Install the `Plots` package and initialize plotting with as many default arguments as you like by calling a backend function like `gr` (the one we will use most often). Example:

```julia
using Plots

gr(
    markerstrokecolor=:brown,
    markerstrokewidth=2,
    color=:green,
    markersize=4,
    marker=:square,
    linecolor=:red,
    linewidth=2
)
```

|                                 |                                                                                                                                                                                |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Scatter plot                    | `scatter(1:5, rand(5); markercolor=[:red, :green]) # setting an attribute like markercolor to a vector tells Plots to cycle through its elements`                              |
| Line plot                       | `plot(rand(5), rand(5); xlabel="x-axis", yscale=:log10, ylabel="y-axis (log)", title="my plot")`                                                                               |
| Overlay multiple plots          | `plot(x, y1)`<br>`plot!(x, y2) # add y2 data`<br>`scatter!(x, y3) # add scatterplot of y3 data`                                                                                |
| Multiple subplots in one figure | `p1 = plot(x, y1)`<br>`p2 = plot(x, y2)`<br>`plot(p1, p2; layout=(2, 1), size=(800, 400)) # stack plots as 2 rows and 1 col, and fix overall figure size`                      |
| Heatmap                         | `A = [1 2 3`<br>&emsp;&emsp;`4 5 6]`<br>`heatmap(A; yflip=true, color=:grays) # yflip ensures the first element of each column is at the top, grays ensures grayscale heatmap` |
| Save figure                     | `p = scatter(1:5, rand(5))`<br>`savefig(p, "myfigure.png")`                                                                                                                    |
