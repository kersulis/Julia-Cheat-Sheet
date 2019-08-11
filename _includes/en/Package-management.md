In Julia 1.0, there are two ways to work with the package manager:
either with `using Pkg` and using `Pkg` functions, or by typing `]` in the REPL to
enter the special interactive package management mode. (To return to regular REPL, just
hit `BACKSPACE` on an empty line in package management mode).

|                                          |                                                    |
| ---------------------------------------- | -------------------------------------------------- |
| List installed packages (human-readable) | `Pkg.status()` or `]status`                        |
| Update all packages                      | `Pkg.update()` or `up`                             |
| Install `PackageName`                    | `Pkg.add("PackageName")` or `]add PackageName`     |
| Rebuild `PackageName`                    | `Pkg.build("PackageName")` or `]build PackageName` |
| Use `PackageName` (after install)        | `using PackageName`                                |
| Remove `PackageName`                     | `Pkg.rm("PackageName")` or `rm PackageName`        |
