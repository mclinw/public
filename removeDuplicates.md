# Remove Duplicates from Sorted Array
Given a sorted array nums, remove the duplicates in-place such that each element appear only once and return the new length.
Do not allocate extra space for another array, you must do this by modifying the input array in-place with O(1) extra memory.

Example 1:
Given nums = [1,1,2],
Your function should return length = 2, with the first two elements of nums being 1 and 2 respectively.
It doesn't matter what you leave beyond the returned length.

Example 2:
Given nums = [0,0,1,1,1,2,2,3,3,4],
Your function should return length = 5, with the first five elements of nums being modified to 0, 1, 2, 3, and 4 respectively.
It doesn't matter what values are set beyond the returned length.

```python
# python online 
# https://www.onlinegdb.com/online_python_compiler
# https://repl.it/languages/python
def removeDuplicates(nums):
    """
    :type nums: List[int]
    :rtype: int
    """
    pass 

# test your code 
examples = [
    [1,1,2] ,               #length = 2 :[1, 2]
    [0,0,1,1,1,2,2,3,3,4] , #length = 5 :[0, 1, 2, 3, 4]
]
for nums in examples :
    length = removeDuplicates( nums  )
    print("length = %d :%s"%(length , nums[:length] ) ) #  nums = [1,1,2]  -> length = 2 :[1, 2]
  
```

```C++
// C++
#include <iostream>
using namespace std;

int removeDuplicates(int nums[] /*IO*/, const int size)
{
    // TODO: update nums array & return length of updated nums array
}

int main()
{
// Example 1:
// Given nums = [1,1,2],
// Your function should return length = 2, with the first two elements of nums being 1 and 2 respectively.
    int arr[] = {1, 1, 2};
    // size = 2 : 1 2
    int end = removeDuplicates(arr, 3);
    cout << "size =" << end << ":";
    for (int i = 0; i < end; ++i)
        cout << arr[i] << " ";
    cout << endl;

// Example 2:
// Given nums = [0,0,1,1,1,2,2,3,3,4],
// Your function should return length = 5, with the first five elements of nums being modified to 0, 1, 2, 3, and 4 respectively.
    int arr2[] = {0, 0, 1, 1, 1, 2, 2, 3, 3, 4};
    // size = 5 : 0 1 2 3 4
    end = removeDuplicates(arr2, 10);
    cout << "size =" << end << ":";
    for (int i = 0; i < end; ++i)
        cout << arr2[i] << " ";
    cout << endl;
    return 0;
}
```
