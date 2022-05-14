### Binart Search Tree Project

[7,5,1,8,3,6,0,9,4,2] -> Binary Search Tree

## Steps

First item is selected as the root

Root: 7

Items are compared to the root and according leaf nodes one by one until no items left to compare. 

5 ? 7: 5<7

1 ? 7: 1<7, 1 ? 5: 1<5

8 ? 7: 8>7

3 ? 7: 3<7, 3 ? 5: 3<5, 3 ? 1: 3>1

6 ? 7: 6<7, 6 ? 5: 6>5

0 ? 7: 0<7, 0 ? 5: 0<5, 0 ? 1: 0<1

9 ? 7: 9>7, 9 ? 8: 9>8

4 ? 7: 4<7, 4 ? 5: 4<5, 4 ? 1: 4>1, 4 ? 3: 4>3

2 ? 7: 2<7, 2 ? 5: 2<5, 2 ? 1: 2>1, 2 ? 3: 2<3

       (7) <br />
     (5)  (8) <br />
 (1)    (6)  (9) <br />
(0)  (3) <br />
  (2) (4) <br />