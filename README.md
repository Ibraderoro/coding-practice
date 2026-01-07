# 🧠 Coding Practice Repository
A structured collection of my daily practice in algorithms, data structures, and problem‑solving.  
This repo tracks my progress through NeetCode, LeetCode, and core CS fundamentals.

My goal: Build elite problem‑solving skills and become a world‑class engineer.

---

## 📁 Folder Structure
This repository is organized by topic, following the NeetCode roadmap:

coding-practice/
│── arrays/
│── hashing/
│── two-pointers/
│── sliding-window/
│── stack/
│── binary-search/
│── linked-list/
│── trees/
│── graphs/
│── dynamic-programming/
│── math/
│── notes/
│── README.md

Each folder contains:
- Problem file (Python/JS/Java)
- My solution
- Time & space complexity
- Notes or thought process

---

## 🚀 Progress Tracker

### Arrays & Hashing
- [ ] Contains Duplicate  
- [ ] Valid Anagram  
- [ ] Two Sum  
- [ ] Group Anagrams  
- [ ] Top K Frequent Elements  

### Two Pointers
- [ ] Valid Palindrome  
- [ ] Two Sum II  
- [ ] 3Sum  

### Sliding Window
- [ ] Best Time to Buy and Sell Stock  
- [ ] Longest Substring Without Repeating Characters  

### Stack
- [ ] Valid Parentheses  
- [ ] Min Stack  

### Binary Search
- [ ] Binary Search  
- [ ] Search Rotated Sorted Array  

### Linked List
- [ ] Reverse Linked List  
- [ ] Merge Two Lists  

### Trees
- [ ] Invert Binary Tree  
- [ ] BFS / DFS basics  

### Graphs
- [ ] Number of Islands  
- [ ] Clone Graph  

### Dynamic Programming
- [ ] Climbing Stairs  
- [ ] House Robber  

---

## 🧩 Example Problem Template

### Problem: Two Sum  
**Category:** Arrays & Hashing  
**Difficulty:** Easy  
**Date:** 2026‑MM‑DD  

#### 🧠 Thought Process
- Use a hash map to store seen numbers  
- Check if `target - num` exists  
- Return indices  

#### ✅ Solution (Python)
```python
# Time: O(n)
# Space: O(n)

class Solution:
    def twoSum(self, nums, target):
        seen = {}
        for i, n in enumerate(nums):
            diff = target - n
            if diff in seen:
                return [seen[diff], i]
            seen[n] = i
