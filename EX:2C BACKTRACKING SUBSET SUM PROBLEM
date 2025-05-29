# EX:2C BACKTRACKING SUBSET SUM PROBLEM

### DATE:

## AIM:
To demonstrate that the sum of the subset of a given set is equal to the given sum.

## ALGORITHM:

1. Define a recursive function subsetSum(arr, n, i, sum, count):

    a. i: current index
   
    b. sum: remaining target sum
   
    c. count: number of valid subsets found so far

2. If i == n (end of array):

    a. If sum == 0, increment count

    b. Return count

3. Recur twice:

    a. Include arr[i] in the sum → sum - arr[i]

    b. Exclude arr[i] from the sum → sum remains the same

4. Return the total count of both recursive calls.
5. Call the function from main with i = 0 and count = 0.

## PROGRAM:

```
# Program to implement Subset sum problem.
# Developed by: SWATHI D
# Register Number: 212222230154
```
```

def subsetSum(arr, n, i,sum, count):
    if i==n:
        if sum==0:
            return count+1
        return count
    count = subsetSum(arr, n, i+1,sum-arr[i], count)
    count = subsetSum(arr, n, i+1,sum, count)
    return count
arr=[]
size=int(input())
for j in range(size):
    value=int(input())
    arr.append(value)
sum = int(input())
n = len(arr)
print(subsetSum(arr, n, 0, sum, 0))
```

## OUTPUT:

![image](https://github.com/user-attachments/assets/6940c284-cdb9-4f68-a7ef-bb4997caa840)

## RESULT:
The Subset Sum Problem was successfully implemented using recursion. The program correctly counted and displayed the number of subsets whose sum equals the given target.
