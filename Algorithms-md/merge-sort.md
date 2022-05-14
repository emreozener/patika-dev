### Merge Sort Project

[16,21,11,8,12,22] -> Merge Sort

## 1- Steps

[16,21,11,8,12,22]  
[16,21,11] [8,12,22]  
[16,21] [11] [8,12] [22]  
[16] [21] [11] [8] [12] [22]  

Divided until every member is single

[16,21] [11] [8,12] [22]  
[11,16,21] [8,12,22]  
[8,11,12,16,21,22]  

Merged until final array is same as starting size

## 2- Big-O Notation

O(nlogn)