#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a). a = 0 
    while a < n * n * n: 0(n^3)
        a = a + n * n


 Time Complexity = 0(n)
 `a` is set to zeros, while `a` is less than n
 increment `a` by `^n`. We are using `n^2` in the incrementation. What that means is
 that `n * n * n` in the while loop doesnt matter which makes the runtime `0(n)`



b) sum = 0
    for i in range(n):O(n * 1) = 0(n *(1 + (log n))) = 0(n * log n) = 0(n log n)
      j = 1
      while j < n: 0(log n)
        j *= 2
        sum += 1
Time Complexity = 0(n log n)
first loop traverses up to the `n` value and set `j` to 1 which is `0(1)`.
The inter while loop check to see if j is less than input `n` we want to 
double the size of `n`. Essentially we are doubling the size of n the complexity 
will be `0(log n)` because it is halving the number on computations.





c. def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
      
Time Complexity = 0(n)
The bunny function checks to see if `n(bunnies)` is equal to 0. if it is return 0.
if `n` is greater than 0 take away 1 bunny til it reaches 0 bunnies. The complexity of the recursive is
`0(n)' because it is going through each elements and decreasing the value of `n` unitl it reaches 0


## Exercise II

def floor_game(f):
    egg_count = 10

    for i in range(f + 1): 0(n * (1 + 1)) 
        if i < 6: `0(1)`
            egg_count -= 1
            print('Egg didnt break', i)
      
    else:
        if i > 5: 0(1)
            egg_count -= 1
            print('Egg did break', i)
            
Time Complexity = 0(n)


