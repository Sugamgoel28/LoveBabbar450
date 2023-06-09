<h1 align="center">INSERTION SORT</h1>
<h4>ALGORITHM</h4>
<ul>
  <li>The intuition behind this algorithm is to iterate the array like an expanding window. In every iteration we'll keep inserting the array elements at right position.</li>
  <li>Step 1: Consider the first element as an array. Keep increasing the size of the array by one in every iteration.</li>
  <li>Step 2: Iterate another loop for the rest of the elements, and figure out if any element is smaller.</li>
  <li>Step 3: Every iteration should have a sorted array.</li>
<img src="https://i.ibb.co/X3Jz7Cn/image.png" alt="image" border="0">
<br>
<h4>INSERTION SORT - CODE</h4>

```cpp

#include <bits/stdc++.h> 
void insertionSort(int n, vector<int> &arr){
    // Write your code here.
    for(int i = 0; i < n; i++){
        int j = i;
        while(j>0 && arr[j-1] > arr[j]){
            swap(arr[j-1],arr[j]);
            j--;
        }
    }
}

```

<h4>COMPLEXITIES</h4>
<ul>
  <li>Av. Time Complexity - O(n<sup>2</sup>)</li>
  <li>Space Complexity - O(1)</li>
  <li>Best Case Time Complexity - O(n<sup>2</sup>)</li>
  <li>Worst Case Time Complexity - O(n<sup>2</sup>)</li>
</ul>
