# RecuesiveArraySumOfInteger
A program to calculate the sum of all integer elements in an integer array by implementing a recursive sum method/ function in Python

def recursive_sum(arr, index=0):
    # Base case: if index reaches the end of the array
    if index == len(arr):
        return 0
    # Recursive case: add current element to sum of rest
    return arr[index] + recursive_sum(arr, index + 1)

# Example usage
array = [5, 10, 15, 20, 25]
print("Array:", array)

total_sum = recursive_sum(array)
print("Sum of all elements:", total_sum)


# Output
Array: [5, 10, 15, 20, 25]
Sum of all elements: 75
