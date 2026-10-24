# Python Numerical Methods Coursework

Two individual coursework notebooks demonstrate polynomial basis approximation and a small PageRank/Markov-chain iteration. The owner confirms they wrote the substantive implementation. The proposed release contains no cell outputs or execution counts; the separate neural-network teaching/verification companion and unrelated notebooks are excluded.

## Notebooks

- `notebooks/polynomial_basis_approximation.ipynb` builds a polynomial basis, approximates coefficients through numerical integration and a linear solve, adds synthetic noise, and compares the approximation with a target signal.
- `notebooks/pagerank_markov_chain.ipynb` illustrates iteration over a three-node stochastic matrix; it is an educational example, not a production search engine.

The notebooks use NumPy and Matplotlib. Install those dependencies and Jupyter in a Python environment, then open either notebook with JupyterLab. Dependency versions are not pinned. No notebook was executed as part of this review.

## Target-expression discrepancy

The polynomial notebook's executable code sets `true_signal = (t - 2.0/np.pi)**2`, and its code comments and plot labels describe `(t - 2/π)^2`. The opening markdown reference instead states `(t - π/2)^2`. No separate assignment specification resolving the difference was found in the reviewed archive. The release copy preserves both historical statements and does not assert which one was intended; no numerical result is presented as verified against the assignment target.

## Attribution and starter-material review

The owner confirms this was an individual assignment and that they authored the substantive implementation. The archived Project 1 notebook corresponds to this work. A synthetic time-series illustration contains a comment saying its noise scaling is “like professor’s”; this attribution cue is retained, and the review did not locate a separate instructor source file or a marked instructor implementation block. NumPy and Matplotlib are referenced dependencies, not vendored code. No dataset is included. The owner recalls starter/template use in coursework generally, but no additional specific instructor material was identifiable in this release copy. No license is included.

## Limitations

Results depend on the notebook's actual coded target and generated noise. The mathematical target discrepancy remains unresolved, dependency versions are unpinned, and the notebooks have not been run or numerically validated. This is coursework, not a production numerical-analysis package.
