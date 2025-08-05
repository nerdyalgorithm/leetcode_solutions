## 🔹 [LeetCode 1920 – Build Array from Permutation](https://leetcode.com/problems/build-array-from-permutation/)

### QUESTION

Given a zero-based permutation nums (0-indexed), build an array ans of the same length 
where ans[i] = nums[nums[i]] for each 0 <= i < nums.length and return it.

### APPROACH

The problem says to return an array where ans[i] = nums[nums[i]].
So for every index i, I just needed to find nums[i], 
then use that result as a new index to get the final value.

Since nums is a 0-based permutation (values from 0 to n−1).

### IMPLEMENTATION
```python3
 Solution:
    def buildArray(self, nums: List[int]) -> List[int]:
        return [nums[nums[i]] for i in range(len(nums))]


