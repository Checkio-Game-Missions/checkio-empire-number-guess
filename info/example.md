**Example:**

```python
guess()                                 # just hypothesis
guess((1,5))                            # the number has a remainder 1
guess((1,5),(1,2))                      # the number has a remainder 1
guess((1,5),(1,2),(2,3))                # the number has a remainder 2
guess((1,5),(1,2),(2,3),(5,6))          # the number has a remainder 5
guess((1,5),(1,2),(2,3),(5,6),(3,4))    # the number has a remainder 3
```