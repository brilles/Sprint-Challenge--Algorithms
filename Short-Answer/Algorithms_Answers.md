## Exercise I

```python
a)  a = 0
    while (a < n * n * n): # O(n)
      a = a + n * n        # 0(1)
```

#### Runtime = O(n) \* O(1) = O(n)

#### Justification: this algorithm increases the number of operations linearly with respect to the input size of because of the while loop.

```python
b)  sum = 0 0(c)
    for i in range(n): # O(n)
      i += 1
      for j in range(i + 1, n): # O(n)
        j += 1
        for k in range(j + 1, n): # O(n)
          k += 1
          for l in range(k + 1, 10 + k):
            l += 1
            sum += 1
```

#### Runtime = O(n) \* 3 = O(n^3)

#### Justification: this algorithm increases the number of operations quadratically with respect to the input size of n because of the nested for loops.

```python
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1) # 0(n)
```

#### Runtime = O(n)

#### Justification: this algorithm increases the number of operations linearly with respect to the input size of n because the function is called n times

## Exercise II

```
Suppose that you have an _n_-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor _f_ or higher, and doesn't get broken if dropped off a floor less than floor _f_. Devise a strategy to determine the value of _f_ such that the number of dropped eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode and give the runtime complexity of your solution.
```

```python

# F is a essentially a sorted array. This is why we will use Binary search O(log n) to determine the value of f such that the number of dropped eggs is minimized

# def binary_search(n, f)
#     low = 0, high= n, mid = (high-low) // 2
#     if f == sorted_arr[mid]
#          return mid
#      elif f < sorted_arr[mid]
#          return binary_searh(sorted_arr[:midpoint])
#      else
#         return binary_search(sorted_arr[midpoint:])

#

```
