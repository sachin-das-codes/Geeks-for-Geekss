## 01. Kth Smallest

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/kth-smallest-element5635/1)

### Problem Description

**Task:** Given an integer array arr[] and an integer k, find and return the k^th smallest element in the given array.Examples :Input: arr[] = [10, 5, 4, 3, 48, 6, 2, 33, 53, 10], k = 4Output: 5

#### Examples

##### Example 1

- **Explanation:** 3rd smallest element in the given array is 7.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n log k)
- **Expected Auxiliary Space Complexity:** O(k)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-28 07:55:19
- **Status:** Correct
- **Marks:** 4

```cpp
class Solution {
  public:
    int kthSmallest(vector<int> &arr, int k) {
        // code here
        priority_queue<int> maxHeap;

        for (int num : arr) {
            maxHeap.push(num);
            if (maxHeap.size() > k) {
                maxHeap.pop();
            }
        }

        return maxHeap.top();
    }
};
```

*Generated on: 11/28/2026, 7:56:03 AM*