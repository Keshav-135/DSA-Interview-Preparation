# Remove Duplicates from Sorted Array

---

## 📌 Problem

Given a sorted integer array `nums`, remove the duplicates **in-place** such that each unique element appears only once.

Return the number of unique elements (`k`). The first `k` elements of the array should contain the unique values in their original order.

---

## 🔍 Pattern

- Two Pointers (Fast & Slow)

---

## 💡 Approach

- Since the array is already **sorted**, duplicate elements always appear together.
- Use two pointers:
  - **`i` (Slow Pointer):** Tracks the position of the last unique element.
  - **`j` (Fast Pointer):** Traverses the array to find the next unique value.
- Whenever `nums[i] != nums[j]`, move `i` one step ahead and copy `nums[j]` to `nums[i]`.
- Continue until the end of the array.
- Return `i + 1`, which represents the number of unique elements.

---

## ⏱️ Time Complexity

**O(n)**

Each element is visited exactly once.

---

## 💾 Space Complexity

**O(1)**

The array is modified in-place without using extra memory.

---

## 💻 Language

**Java**

---

## 🎯 Key Learning

- Fast Pointer scans the array.
- Slow Pointer stores only unique elements.
- Sorted arrays allow duplicate removal without extra space.
- In-place modification saves memory.

---

## 📝 Revision Notes

🧠 **Remember this in one line:**

> **Fast pointer finds the next unique element, Slow pointer stores it.**

### When should this pattern come to mind?

✅ Array is **sorted**

✅ Need to **remove duplicates**

✅ Need **in-place modification**

✅ Extra space is **not allowed**

### Pointer Movement

```text
i = Slow Pointer (Last Unique)

j = Fast Pointer (Scan Array)

1 1 2 2 3 4 4

i
↓

j
↓
```

If

```text
nums[i] == nums[j]
```

➡️ Ignore duplicate.

If

```text
nums[i] != nums[j]
```

➡️ Move `i++`

➡️ Copy

```text
nums[i] = nums[j]
```

### Interview Trick

If you hear:

- Sorted Array
- Remove Duplicates
- In-place

👉 Think **Fast & Slow Two Pointers** immediately.

---

## 🧩 Pattern Category

**Two Pointers**

---

## 🏷️ LeetCode

**26. Remove Duplicates from Sorted Array**

---

## 📊 Difficulty

🟢 Easy

---

## ✅ Status

✔️ Solved

---

## 📅 Date Solved

10-07-2026
