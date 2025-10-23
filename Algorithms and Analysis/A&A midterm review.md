## 1.2
### Big-Omega and Big-Theta
##### Big-Omega(Best Case)
- Gives a **guaranteed minimum growth rate** for a function.
- For every n ≥ n0: f(n) ≥ c⋅g(n).
- This means: For all sufficiently large n, f(n) is **at least** a constant * g(n).

##### Big-Theta 
- Means two functions are **asymptotically equal**, up to a constant factor.
- f(n) grows as fast as g(n).
- c'⋅g(n) ≤ f(n) ≤ c''⋅g(n)

### Little-Oh and Little-Omega
##### Little-Oh 
- Means grows **strictly slower** than g(n)g(n) as n gets large.
- f(n) = o(g(n)) if for every constant c>0, there is an n0 such that f(n) < c⋅g(n) for all n ≥ n0
- As n→∞, f(n)/g(n)→0.

##### Little-Omega(Average Case/ Tight Bound)
- Means grows strictly faster than g(n)g(n) as n gets large.
- f(n)=ω(g(n)) if for every constant c>0, there is an n0 such that c⋅g(n) < f(n) for all n ≥ n0
- As n→∞, f(n)/g(n)→∞.

## 1.4
### Amortization
Rather than focusing on each operation separately, it considers the interactions between all the operations by studying the running time of a series of these operations.


## 10.4
For a Huffman tree to be complete, it must be _perfectly balanced_ given the number of symbols, and their frequencies must allow the algorithm to keep merging pairs in such a way that the tree remains complete at every step. This usually happens when **all frequencies are the same** or can be paired evenly at each step.