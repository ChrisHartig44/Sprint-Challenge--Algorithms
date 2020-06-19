#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)  a = 0
    while (a < n * n * n):
      a = a + n * n

#### The runtime complexity of a) is 0(n). The while loop appears to being excecuted 0(n^3) times, but  the value of a is being uppdated n * n times in each iteration. The n squareds cancel each other out, so the runtime complexity is just of 0(n).

b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1 
#### The runtime complexity of b) is 0(n log n) because the outer loop is O(n) and the inner loop is (log n). 

c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
#### The runtime complexity of c) is 0(n) because a recursive call is being made for each element. 

## Exercise II

We are trying to find the first floor where eggs start breaking if dropped from. Because buildings can only be so high, I don't think speed will be an issue. 

I would go through every floor of a hypothetical building and see at what height eggs start breaking.

I would plan to do a linear search, which has a runtime complexity of 0(n).


