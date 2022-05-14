### Insertion Sort Project

[22,27,16,2,18,6] -> Insertion Sort

## 1- Steps  

[**22**,27,16,2,18,6]  

[22,**27**,16,2,18,6] 22<27? +  

[22,27,**16**,2,18,6] 27<16? -;  
[22,**16**,27,2,18,6] 22<16? -;  
[**16**,22,27,2,18,6]  

[16,22,27,**2**,18,6] 27<2? -;  
[16,22,**2**,27,18,6] 22<2? -;  
[16,**2**,22,27,18,6] 16<2? -;  
[**2**,16,22,27,18,6]  

[2,16,22,27,**18**,6] 27<18? -;  
[2,16,22,**18**,27,6] 22<18? -;  
[2,16,**18**,22,27,6] 16<18? +  

[2,16,18,22,27,**6**] 27<6? -;  
[2,16,18,22,**6**,27] 22<6? -;  
[2,16,18,**6**,22,27] 18<6? -;  
[2,16,**6**,18,22,27] 16<6? -;  
[2,**6**,16,18,22,27] 2<6? +  

[2,6,16,18,22,27] 


## 2- Big-O Notation  

O(n^2)  

## 3- Time Complexity

**Worst Case**: The list is the exact opposite order of the needed order.
1st term: 0 comparisons  
2nd term: 1 comparison  
...  
nth term: n-1 comparisons  

total comparisons: 0+1+2+...+n-1 = ((n-1)*(n)) / 2 = (n^2 - n) / 2  
Since n^2 dominates the complexity growth, big-o notation for worst case scenario is O(n^2)  

**Best Case**: The list is in the exactly desired order.
In this case, algorith compares every item with the preceding item with the exception of the first item. 
For n items, n-1 comparisons are made. In this case, big-o notation is O(n)

**Average Case**: The average of best case and worst case. The average is {[ (n^2 - n) / 2 ] + n-1 }/2 which gives us 
a quadratic function. n^2 is the dominating term so big-o notation is O(n^2)


## 4- What is the Case for the number 18?

The number 18 is in the scope of average case since it has been moved but it has not been 
needed to be compared to every single preceding item. 

## 5- First 4 Insertion sort steps for [7,3,5,8,2,9,4,15,6]

[**7**,3,5,8,2,9,4,15,6] no actions  

[7,**3**,5,8,2,9,4,15,6] 7<3? -;  
[**3**,7,5,8,2,9,4,15,6]  

[3,7,**5**,8,2,9,4,15,6] 7<5? -;  
[3,**5**,7,8,2,9,4,15,6] 3<5? +  

[3,5,**7**,8,2,9,4,15,6] 5<7? +  


