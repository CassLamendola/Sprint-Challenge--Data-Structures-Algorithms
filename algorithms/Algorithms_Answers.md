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

    b) If I'm understanding right, f is not a pre-determined value, but a value chosen to minimize the number of broken eggs (says "dropped", but I assume it means "broken"). So if it can be arbitrarily chosen, it should be set to equal n (the number of stories). Then an egg will only be broken if it's dropped from the top floor (assuming f can't be greater than n, otherwise set f to n+1). Is this a trick question?

Exercise III.

    a) O(n^2) because quicksort will be recursively called for every element in the array, and every call loops over the remaining elements.

    b) O(log n) because each iteration deals with a list that is half the size of the previous list.