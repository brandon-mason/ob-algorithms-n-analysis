## Terms to google
- Local Optimum

## Note 
Simple Subproblem: VERY SIMPLE. Could just be a value comparison.

![[Pasted image 20251008120156.png]]
total cost for one unit of component D: 
	7 = D (D has no subcomponents)
total cost for one unit of component E: 
	25 = 2D + 3E + B

### Memoization
Keep a table of known values, so that if we are ever asked for a known value, we can simply look it up in the table, rather than spending an inordinate amount of time recomputing the number.

Only requirement is that we have a way of parameterizing known results to allow efficient lookup in the table.

