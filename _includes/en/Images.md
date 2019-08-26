|                                  |                                                                                                                                                            |
| -------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Convert RGB image to grayscale   | `using Images, FileIO`<br>`img = load("myphoto.png")`<br>`gray_img = Gray.(img)`                                                                           |
| Convert grayscale image to array | (continuing previous example):<br>`gray_img_mat = Array{Float64}(gram_img)`<br>could also use pip operator:<br>`gray_img_mat = gray_img |> Array{Float64}` |
