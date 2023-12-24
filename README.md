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
```''' 
Program for linear search method to match the item in a list
Developed by:SRISHANTH J
RegisterNumber:212223240160 
'''
def linearSearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1        
    
array = eval(input())
array=sorted(array)
n=len(array)
k = eval(input()) 
res= linearSearch(array,n,k)
if(res==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index: ",res)
    




```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:SRISHANTH J
RegisterNumber:212223240160 
'''
def binarySearch(array, x, low, high):
    while low<=high:
        mid= low+(high-low)//2
        if array[mid]==x:
            return mid
        elif array[mid]<x:
            low=mid+1
        else:    
            high=mid+1
    else:
        return -1
array=eval(input())
x=eval(input())
array.sort ()
low=0
high=len(array)-1
result=binarySearch(array,x,low,high)
if result==-1:
    print(array,"\nElement not found")
else:
     print(array)
     print("Element found at index: ", result)
    





```
iii)	# Find the element in a list using Binary Search (recursive Method).
```

Program to find the element in a list using Binary Search (recursive Method).
Developed by: your name:SRISHANTH J
RegisterNumber: 212223240160
'''
def BinarySearch(arr, k, low, high):
    if high>=low:
        mid=low+(high-low)//2
        if arr[mid]==k:
            return mid
        elif arr[mid]>k:
            return BinarySearch(arr,k,low,mid-1)
        else:
            return BinarySearch(arr,k,mid+1,high)
    else:
        return -1
arr=eval(input())
arr.sort()
k=eval(input())
result=BinarySearch(arr,k,0,len(arr)-1)
if(result==-1):
    print(arr,"\nElement not found")
else:
    print(arr,"\nElement found at index: ",result)


```
## Sample Input and Output
<img width="648" alt="Screenshot 2023-12-24 204810" src="https://github.com/srishanth2006/Search-Algorithm/assets/150319470/e63502a4-f2b6-4a3b-9f7e-e5759973be64">

<img width="663" alt="Screenshot 2023-12-24 204831" src="https://github.com/srishanth2006/Search-Algorithm/assets/150319470/7ee654b1-f2ba-444c-9ae0-a59ddf936cff">

<img width="649" alt="Screenshot 2023-12-24 204846" src="https://github.com/srishanth2006/Search-Algorithm/assets/150319470/f7df3349-732f-4797-906c-79bd2081ab6f">



## Result
Thus the linear search and binary search algorithm is implemented using python programming.
