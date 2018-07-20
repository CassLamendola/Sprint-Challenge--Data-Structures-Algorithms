Add your answers to the Algorithms exercises here.

Exercise I.

    a) O(n^3)

    b) O(n)

    c) O(64 * sqrt(n)/2) => O(sqrt(n))

    d) O(n * sqrt(n))

    e) O(10n^3) => O(n^3)

    f) O(n)
    
    g) O(n)

Exercise II.
    
    a)
```python
def biggest_diff(a):
    j = a.index(max(a))
    i = a.index(min(a))
    return max([a[j] - min(a[:j]), max(a[i+1:]) - a[i]])
```

    b) Start by dropping an egg from the middle floor `math.floor(n/2)`, then if the egg doesn't break, check the floor halfway between the current floor and the top. If it breaks, check the floor halfway between the current floor and the ground. Stop when, on two floors that are consecutive, the egg breaks dropped from one and doesn't break when dropped from the other. `f` equals the floor from which the egg dropped in that last step.

Exercise III.

    a) O(n^2) because quicksort will be recursively called for every element in the array, and every call loops over the remaining elements.

    b) O(log n) because each iteration deals with a list that is half the size of the previous list.