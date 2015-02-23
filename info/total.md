...When you have eliminated all which is impossible, then whatever remains, however improbable, must be the truth.

-- Sir Arthur Conan Doyle "Sherlock Holmes"

We've added a new prediction module in the Laboratory Super Computer.
But before we can use it, it needs to be calibrated. We can use the "Guess the Number" game to ensure the calibrations are working correctly.

You are given an unknown number ranging from 1 to 1000, inclusive.
Your task is to **find the number by performing a series of guesses**

Your solution will need to guess the number by submitting an **integer divisor** and the **number guessed**.
On each attempt you will get information about previous guesses. 
Each guess is represented as an array which contains the remainder result along with your previous divisor.

You should find the number with a minimum number of guesses (but not more than 13). 
The final result will be defined as an average of the attempted numbers. 

**Input:** Information about the previous attempt. A variable number of arguments, each of them is a tuple. 
           Each tuple contains its remainder and the previous divisor. 

**Output:** A list of integer divisors and your best guess. A list of two integers.

**Example:**

```python
guess()                                 # just hypothesis
guess((1,5))                            # the number has a remainder 1
guess((1,5),(1,2))                      # the number has a remainder 1
guess((1,5),(1,2),(2,3))                # the number has a remainder 2
guess((1,5),(1,2),(2,3),(5,6))          # the number has a remainder 5
guess((1,5),(1,2),(2,3),(5,6),(3,4))    # the number has a remainder 3
```
**How it is used:**

This is a classical prediction and decision problem. You are given some indirect information and need to find the solution hidden within the data.
The skills that go into this problem could help you create a sports bracket for an office pool.

**Precondition:**

```python
0 < hidden_number <= 1000
```

