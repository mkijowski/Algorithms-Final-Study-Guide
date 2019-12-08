##### Problem 1: Big Oh
Consider four graph algorithms with the following worst case running
times (where *n* is the size of the node set and *m* is the size of the edge set):
`n lg n`, `n lg m`, `m lg n`, and `m lg m`. Using the big-Oh criteria, determine
which ones are equivalent, and on that basis, order the equivalence classes.

##### Problem 2: Recurrences
Are there values of n for which repeated square rooting *n*
`(sqrt(sqrt(...(sqrt(n)...))' can yield integers? 

Either argue that such arbitrarily long finite sequence of
integers do not exist, or provide a general formula/schema for constructing
such sequences. (FYI: Such problems arise while solving recurrences.)

##### Problem 3: Big Oh
Provide closed form and/or order-theoretic solutions to
the following recurrences. (Assume `T(1) = 1`)
1. `T(n) = 16 T(n/4) + n`
2. `T(n) = 16 T(n/4) + n2`
3. `T(n) = 16 T(n/4) + n3`
4. `T(n) = T(n-1) + n2`

##### Problem 4: Dynamic Programming
Use dynamic programming to find least-cost alignment
of the two strings CAT and ACGC under the operation cost model where
*insert*, *delete* and *substitute* cost **+1** and *match* costs **-2**.

1. Clearly state the recurrence relation and 
2. fill the appropriate table.
3. Give an explicit list of operations to align the two strings or display the
   strings in such a way that the details of the alignment are clear.
4. Is the least-cost alignment unique (or are there multiple ways of achieving it)?

##### Problem 5: Network Flow (needs diagram)
1. Determine the maximum flow from node s to node t in the
   following network. The labels on the edges indicate their capacity.
2. Show the actual flow through each edge of the network so as to realize
   the maximum flow. (Note that c-e edge goes both ways.)

##### Problem 6: The Clique problem
Given a graph G = (N, E) and an integer k,
determine if G contains a clique of size k. A clique is a set of nodes such that
every pair of nodes is connected by an edge.

Prove that the Clique Problem CP is NP-Complete in two steps:
1. Select a suitable NP-Complete problem NPC discussed in the class and
   specify the direction of reduction.
2. State and justify the validity of the construction/reduction that relates
   instances of CP and NPC.
