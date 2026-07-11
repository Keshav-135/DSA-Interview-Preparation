# Move Zeroes

## 📌 Problem

Given an integer array `nums`, move all `0`s to the end while maintaining the relative order of the non-zero elements.

The operation must be performed **in-place** without making a copy of the array.

---

## 🔍 Pattern

**Two Pointers (Fast & Slow)**

---

## 💡 Approach

Use two pointers:

- **left (Slow Pointer):** Points to the position where the next non-zero element should be placed.
- **right (Fast Pointer):** Traverses the array from left to right.

Whenever a non-zero element is found, swap it with the element at the `left` pointer and increment `left`.

After traversing the entire array, all non-zero elements remain in their original order, and all zeroes are automatically moved to the end.

---

## ⏱️ Time Complexity

**O(n)**

Each element is visited exactly once.

---

## 💾 Space Complexity

**O(1)**

The array is modified in-place without using any extra memory.

---

## 💻 Language

Java

---

## 🎯 Key Learning

- Fast Pointer scans the entire array.
- Slow Pointer keeps track of the next position for a non-zero element.
- Swapping allows the array to be modified in-place.
- Two Pointers help solve the problem in a single traversal with constant extra space.

---

## 🧩 Pattern Category

**Two Pointers**

---

## 🏷️ LeetCode

**283. Move Zeroes**

---

## 📊 Difficulty

🟢 Easy

---

## ✅ Status

✔️ Solved
