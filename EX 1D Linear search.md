# EX 1D Linear search
## DATE: 
## AIM:
To write a python program for a search function with parameter list name and the value to be searched.

## Algorithm
1. Start

2. Read the number of elements x and populate List with x elements.

3. Read the value n that you want to search for in the list.

4. Start a loop to iterate through each element in List.

5. For each element, check if it is equal to n.

6. If a match is found, return the index of the element.

7. If the loop completes without finding n, return -1 and indicate that the value was not found.

8. End

## Program:

Program to implement a search function with parameter list name and the value to be searched.

Developed by: POKALA GURAVAIAH

Register Number: 212222040114

```PY
def search(List1,n):
    for i in range(len(List1)):
        if (List1[i]==n):
            return i
    return -1
List = [] 
x=int(input())
for i in range(x):
    List.append(input())
n =input()
value = search(List, n)
if value!=-1:
	print("Found")
else:
	print("Not Found")
```

## Output:

<img width="400" alt="image" src="https://github.com/user-attachments/assets/019556e3-eb2f-475f-9bda-a3b0f81bbd0b" />


## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
