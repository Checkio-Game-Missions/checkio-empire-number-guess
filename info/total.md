...When you have eliminated all which is impossible, then whatever remains, however improbable, must be the truth.

-- Sir Arthur Conan Doyle "Sherlock Holmes"

We've added the new prediction module in the Laboratory Super Computer.
But before usage we should calibrate it. "Guess Number" game will be nice for this.

You are given an unknown number within the range of 1 to 1000, inclusive.
Your task is to **guess what the number is by performing a series of guesses**

Your solution will need to guess the number by submitting an **integer divisor** and the **number you guessed**.
At each attempt you will get information about previous guesses. 
Each guess is represented as an array which contains the remainder result along with your previous divisor.

You should find the number within minimum guesses (but not more than 13). 
The final result will be defined as an average of attempt numbers. 

**Input:** Information about the previous attempt. Variable number of arguments, each of them is a tuple. 
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

This is a classical prediction and decision problem.
You have some indirect information and should to get hidden by it data.
The skills that go into this problem could help you create a sports bracket for the office pool.

**Precondition:**

```python
0 < hidden_number <= 1000
```

