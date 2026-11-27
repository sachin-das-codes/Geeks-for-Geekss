## 01. Reverse a String

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-a-string/1)

### Problem Description

**Task:** Given a string s, reverse the string.Examples:Input: s = "Geeks"

#### Examples

##### Example 1

- **Output:**
```text
"skeeG"
```

##### Example 2

- **Input:**
```text
s = "for"
```
- **Output:**
```text
"a"
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (C++)

- **Submitted:** 2026-11-27 19:58:50
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    string reverseString(string& s) {
        int i = 0;
        int j = s.size() - 1;

        while (i < j) {
            // Swap characters at indices i and j
            char temp = s[i];
            s[i] = s[j];
            s[j] = temp;

            // Move pointers toward the center
            i++;
            j--;
        }

        return s;
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-11-27 19:50:12
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string reverseString(string& s) {
        int i = 0;
        int j = s.size() - 1;

        while (i < j) {
            // Swap characters at indices i and j
            char temp = s[i];
            s[i] = s[j];
            s[j] = temp;

            // Move pointers toward the center
            i++;
            j--;
        }

        return s;
    }
};
```

*Generated on: 11/27/2026, 7:59:53 PM*