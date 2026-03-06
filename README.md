# personal details
ABEDNEGO JEFFA CHITI
EB3/67223/23
## About merge sort
merge sort is an algorithm that is based on the divide and conquer strategy.To divide,you split the array into two halves.To conquer,you
recursively sort each half.Then you combine the sorted halves into one sorted array.This sorting algorithm breaks the array until only 
single elements remain which are already sorted.
## time complexity analysis
### best case
in the best case an array already sorted can still divide,merge and compare.
let time T(n)=time to sort an algorithm of size n
n=size of an array
in dividing it takes constant time to split the array 0(1)
in merging it takes  linear time to merge two arrays of size n/2 each 0(n)
the recurrence relation is:T(n)=2.T(n/2)+n
in level one when it is the whole array,it is n comparisons to merge left and right halves.
in level 2 where the array is split into two halves,each half size has n/2 comparisons to merge.This shows that in each level the total 
work is n and the number of levels =log2(n) because the array is divided in half each until the size is 1.
T(n)=n⋅log2​(n)
so the best time complexity is 0(nlogn)
### worst case
it happens when every comparison during merging leads to maximum work.
the recurence relation is T(n)=2.T(n/2)+n
the total work T(n)=n+n+n.....+n(log2(n)times)
T(n)=n⋅log2​(n)
so the worst case time complexity is 0(nlogn)
### average case
it occurs when the array is randomly ordered.
letting T(n)=time to sort an array of size n
the recurrence=.T(n/2)+n
total work =T(n)=n+n+n.....+n(log2(n)times)
T(n)=n⋅log2​(n)
so the average time complexity is 0(nlogn)
## Algorithm efficiencies
stable sorting-equal elements keep their original order.
it works well with large datasets-its efficient for arrays or linked lists.
good dor external sorting-it can handle data taht doesnt fit in memory.
## algorithm limitations
not adaptive-merge sort doesnt get faster if the array is already partially sorted.
recursive overhead-recursion can add function call overhead for very large arrays.
not in-place by default-it requires additional storage
