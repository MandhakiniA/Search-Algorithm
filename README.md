# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
''' 
Program for linear search method to match the item in a list
Developed by:A.Mandhakini
RegisterNumber: 23010115
'''
def linearsearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
array=eval(input())
k=eval(input())
n=len(array)
array.sort()
result=linearsearch(array,n,k)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)



```
ii)	# Find the element in a list using Binary Search(Iterative Method).

```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:A.Mandhakini
RegisterNumber: 23010115
'''
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if(array[mid]==k):
            return mid
        elif(array[mid]<k):
            low=mid+1
        else:
            high=mid-1
    return -1
array=eval(input())
array.sort()
k=eval(input())
result=binarySearchIter(array,k,0,len(array)-1)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
    




```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
''' 
Program to find the element in a list using Binary Search (recursive Method).
Developed by: your name:A.Mandhakini
RegisterNumber: 23010115
'''
def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if(array[mid]==k):
            return mid
        elif(array[mid]<k):
            low=mid+1
        else:
            high=mid-1
    return -1
array=eval(input())
array.sort()
k=eval(input())
result=binarySearchIter(array,k,0,len(array)-1)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",result)
    
        




```
## Sample Input 
![image](https://github.com/MandhakiniA/Search-Algorithm/assets/150005194/ecd9b341-55e8-4321-9fae-fa20c25645f0)


## Output
i)
![image](https://github.com/MandhakiniA/Search-Algorithm/assets/150005194/a7eed07c-edda-4981-a604-696cd400e8aa)
ii)
![image](https://github.com/MandhakiniA/Search-Algorithm/assets/150005194/2dd8968a-7934-4f6d-afc5-bab86798b37b)
iii)
![image](https://github.com/MandhakiniA/Search-Algorithm/assets/150005194/6e9d5fe0-81ca-4345-8c46-2b3fb10131e8)









## Result
Thus the linear search and binary search algorithm is implemented using python programming.
