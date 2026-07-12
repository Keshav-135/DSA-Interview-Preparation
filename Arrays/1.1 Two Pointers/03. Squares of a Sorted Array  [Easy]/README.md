# Squares of a Sorted Array

## 📌 Problem

Given an integer array `nums` sorted in non-decreasing order, return an array of the squares of each number, also sorted in non-decreasing order.

---

## 🔍 Pattern

Two Pointers

---

## 💡 Approach

Since the input array is already sorted, the largest square will always come from either the leftmost negative number or the rightmost positive number.

- Use two pointers:
  - `left` starts from the beginning.
  - `right` starts from the end.
- Compare the absolute values of both elements.
- Place the larger square at the end of the result array.
- Move the corresponding pointer inward.
- Repeat until both pointers meet.

---

## 📝 Algorithm

1. Create a result array of the same size.
2. Initialize:
   - `left = 0`
   - `right = n - 1`
   - `index = n - 1`
3. Compare `abs(nums[left])` and `abs(nums[right])`.
4. Store the larger square at `ans[index]`.
5. Move the corresponding pointer.
6. Decrease `index`.
7. Continue until `left > right`.
8. Return the result array.

---

## ⏱️ Time Complexity

**O(n)**

Each element is processed exactly once.

---

## 💾 Space Complexity

**O(n)**

An additional array is used to store the sorted squares.

---

## 💻 Language

Java

---

## 🎯 Key Learning

- Two Pointers can efficiently solve problems on sorted arrays.
- Comparing absolute values helps determine the largest square.
- Filling the answer array from the end avoids extra sorting.
- This approach improves the time complexity from **O(n log n)** (sorting) to **O(n)**.

---

## 🧩 Pattern Category

Two Pointers

---

## 🏷️ LeetCode

977. Squares of a Sorted Array

---

## 📊 Difficulty

🟢 Easy

---

## ✅ Status

✔️ Solved
