# EX 1C Quick Sort
## DATE: 
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of string values.

## Algorithm

1. Select a pivot element from the array (commonly the first element).

2. Rearrange the array so that all elements less than or equal to the pivot are on the left, and all elements greater than the pivot are on the right.

3. After partitioning, determine the final position of the pivot.

4. Apply QuickSort to the subarray to the left of the pivot.

5. Apply QuickSort to the subarray to the right of the pivot.

6. If the subarray has one or no elements, it is already sorted, and the recursion stops.


## Program:

Program to implement implement quick sort using the last element as pivot on the list of string values.

Developed by: POKALA GURAVAIAH

Register Number: 212222040114

```PY
def quickSort(alist, start, end):
    if end - start > 1:
        p = partition(alist, start, end)
        quickSort(alist, start, p)
        quickSort(alist, p + 1, end)
 
def partition(alist, start, end):
    pivot = alist[start]
    i = start + 1
    j = end - 1
    #print("Pivot: ",pivot)
    while True:
        while (i <= j and alist[i] <= pivot):
            i = i + 1
        while (i <= j and alist[j] >= pivot):
            j = j - 1
 
        if i <= j:
            alist[i], alist[j] = alist[j], alist[i]
        else:
            alist[start], alist[j] = alist[j], alist[start]
            return j

arr = []
n=int(input())
for i in range(n):
    arr.append(input())
quickSort(arr, 0, n)
print("Sorted array is:")
for i in arr:
    print(i)
```

## Output:

![image](https://github.com/user-attachments/assets/2dbddd18-1b45-4b93-9411-0885928f27be)


## Result:
Thus the python program to implement quick sort using tha last element as pivot on the list of string values is successfully executed.
