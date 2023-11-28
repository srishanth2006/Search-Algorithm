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
```def max_marks(marks):
    marks.sort()
    large=marks[-1]
    return large
    



```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```def max_marks(marks):
    maxi=max(marks)
    return maxi
    





```
iii)	# Find the element in a list using Binary Search (recursive Method).
```

def max_marks(list1):
    max=list1[0]
    for i in list1:
        if(i>max):
            max=i
    return max



```
## Sample Input and Output



<img width="590" alt="Screenshot 2023-11-28 233432" src="https://github.com/srishanth2006/Search-Algorithm/assets/150319470/863962d0-fab4-4ff9-bc7f-e77c63073005">
<img width="546" alt="Screenshot 2023-11-28 233503" src="https://github.com/srishanth2006/Search-Algorithm/assets/150319470/1db1999d-5c2a-45a9-82d1-f1bc8f38a34b">


<img width="597" alt="Screenshot 2023-11-28 233525" src="https://github.com/srishanth2006/Search-Algorithm/assets/150319470/322d2f3a-ebab-41e7-93ec-d97dad45a897">



## Result
Thus the linear search and binary search algorithm is implemented using python programming.
