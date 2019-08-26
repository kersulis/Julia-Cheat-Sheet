Standard library: `SparseArrays`

Sparse SVD (svds) and eigen (eigs): `Arpack`

| --------------------------                                        | ----                                                                                                                                                                                                  |
| ----------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Initialize a sparse matrix                                        | `I, J, V = [1; 2; 3], [4; 5; 6], [1; 10; 100]`<br>`S = sparse(I, J, V, 10, 15) # 10-by-15 sparse matrix`                                                                                              |
| Create a sparse matrix by specifying diagonals                    | `subdiag, diag, superdiag = [1; 1; 1], [10; 10; 10; 10], [100; 100; 100]`<br>`S = spdiagm(-1 => subdiag, 0 => diag, 1 => superdiag) # easier to see this matrix by converting to dense with Array(S)` |
| Sparse SVD for computing `k` components (requires `using Arpack`) | `usv, nconv, niter, nmult, resid = svds(A::SparseMatrixCSC; nsv=k)`<br>`U, S, V = usv.U, usv.S, usv.V`                                                                                                |
| Sparse eigendecomposition                                         | `val, vec = eigs(A)`                                                                                                                                                                                  |
| Sparse QR                                                         | `F = qr(S)`<br>`F.R == F.Q' * S[F.prow, F.pcol]`                                                                                                                                                      |
