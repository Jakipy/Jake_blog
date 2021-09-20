---
layout: post
---
{% highlight ruby %}
def binarysearch(arr,target):
    low = 0
    high = len(arr)
    mid = 0
    while(low < high):
        mid = (low + high)/2
        mid = round(mid)
        if(arr[mid] < target):
            low = mid + 1
        elif(arr[mid] > target):
            high = mid -1
        else:
            return mid
    return -1




arr = [1,7,9,11,13,17,21,44,55,67,68]
target = 68
result = (binarysearch(arr,target))
print(target, "is on index",result+1)
{% highlight ruby %}

This is bineary search algorithm

Binary search has a time complexity of O(log N)

should be sorted array

3 variables low, mid, high 

each iteration neglect middle of a array or sub array where their can be a target value

ex target value = 6
arr = [1, 2, 3, 4, 5, 6, 7, 8 ,9 ,10]
get rid of 1 2 3 4 5 becuase they are smaller than 6
find middle in rest of array and reapeat this process log n times

If their is not trarget value return -1