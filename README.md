# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
Developed by: M GAYATHIRI ROSHINI
RegisterNumber: 23006823
def selection_sort(nums):
    for i in range(len(nums)):
        lowest_index_value=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest_index_value]:
                lowest_index_value=j
        nums[i],nums[lowest_index_value]=nums[lowest_index_value],nums[i]
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
```
ii)	#Insertion Sort
```
Developed by:M GAYATHIRI ROSHINI
RegisterNumber: 23006823
def insertion_sort(nums):
   for i in range(1,len(nums)):
       item=nums[i]
       j=i-1
       while j>=0 and nums[j]>item:
           nums[j+1]=nums[j]
           j-=1
       nums[j+1]=item
   return nums
list_of_nums=eval(input())
value=insertion_sort(list_of_nums)
print(value)
```
## Output:
![image](https://github.com/23006823/Sorting-Algorithm/assets/138971409/02a54077-c69e-452a-a73f-bce076477e4c)
![image](https://github.com/23006823/Sorting-Algorithm/assets/138971409/774b7472-2aae-4c48-a8a2-82932b4a898b)
## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
