Add your answers to the Algorithms exercises here.

a) O(2n)
    - the limit for the while loop is n^3
    - however the conditional parameter, 'a', is growing by order 2n^2


b) O(n^3)
    - starting from the inner most loop 'for l in range(k + 1, 10 + k)', for any given k the range will only give 9 iterations. this is a constanst
    - 'for k in range(j + 1, n)' depends on n so it will be O(n)
    - 'for j in range(i + 1, n)' depends on n so it will be O(n)
    - 'for i in range(n)' depends on n so it will be O(n)

c) O(n)
    - the recursive function is decreasing n on each iteration. So we do not have to compute things we already have.
    - the 'bunnyEars' function will be called 'n' this and we will have to add them up.



Exercise II: O(nlog(n))
    Iterate this logic:
    - pick a random floor 'f' from the '_n_' set 
    - if the egg breaks, remove all floors to the right of 'f' 
    - else if the egg does not break, and 'f+1' also does not break, remove all floors to the left of 'f'
    - else return 'f' as '_f_'
    