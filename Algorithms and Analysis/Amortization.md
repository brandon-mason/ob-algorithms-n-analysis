**Focus on interactions between operations rather than the individual operations**

Studies the run time of a series of operations

Amortized Runtime: worst case running time of a series of operations divided by the total number of operations available to the algorithm. (If unspecified, operations are assumed to just be the standard data structure operations)

## Techniques
### Accounting method
Basic operations to be used in an algorithm are said to have(**constant**) cost 1(even though operations may actually have a different cost, it isn't really important)
- Cost of 1 = insert into array
- Cost of 3 = insert into array, expand table, move value into new expanded array

The difficulty with problems that require amortized analysis is that, in general, some of the operations will require greater than constant cost. This means that no constant payment will be enough to cover the worst case cost of an operation, in and of itself. With proper selection of payment, however, this is no longer a difficulty; the expensive operations will only occur when there is sufficient payment in the pool to cover their costs.

Amortization presents difficulty because some operations will be above the constant cost. This derails the constant cost assumption which occurs in the worst case, but 

For an operation to be performed, the already spent cost must be greater than or equal to the cost of the current operation.

### Potential Functions
Use energy state? Represented with **0/** but only in my notes

Operations contribute some an "amortized time" to **0/** and also extracts value from **0/** proportional to time actually spent.

The main idea of using the potential function argument is to use the change in potential for the *i*th operation, **0/**'i - **0/**'i-1, to characterize the amortized time needed for that operation.

