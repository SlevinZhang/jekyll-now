---
layout: post
title: Algorithm
---
### 寻找第K大的元素  
1. Sort and output the Kth, O(n^2)
2. Sort K element and compare with other elements, O(n*k)  
3. build a heap and delete min element K times, O(n * logn)  
4. 找最大元素，建立最大堆，找最小元素建立最小堆  

### 练习总结  
1. 所有题，无论有没有思路都要注意条件，往往很多小陷阱就在条件判断不清楚上  
2. 有了想法，不要着急实现，先解释一下思路，然后尝试在例子上面测试一下
