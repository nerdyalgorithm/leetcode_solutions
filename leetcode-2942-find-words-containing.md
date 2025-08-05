## 🔹 [LeetCode 2942 – Find Words Containing Character](https://leetcode.com/problems/find-words-containing-character/)

### 🧠 Approach

Given a list of words and a character `x`, we need to return the indices of the words that contain that character.

I used a basic loop with `enumerate()` to track both the index and the word.
If the character `x` is found in the word (`if x in word:`), I store the index.


### ✅ Solution

```python
class Solution:
    def findWordsContaining(self, words: List[str], x: str) -> List[int]:
        result = []
        for i, word in enumerate(words):
            if x in word:
                result.append(i)
        return result
```

### 💬 Example

```python
words = ["leet", "code"]
x = "e"
# Output: [0, 1] since both "leet" and "code" contain "e"
```

---


