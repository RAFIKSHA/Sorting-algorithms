
---

## 🔷 Selection Sort Algorithm

This repository contains a simple Python implementation of the **Selection Sort** algorithm with code, explanation, and sample output.

---

### 📌 What is Selection Sort?

**Selection Sort** is a comparison-based sorting algorithm. It works by repeatedly finding the **minimum element** from the unsorted part and placing it at the beginning.

🔁 **Process:**

1. Select the minimum value from the unsorted array.
2. Swap it with the value at the current position.
3. Repeat for all positions until the array is sorted.

---

### 🔢 Example

**Input:**
`[5, 3, 8, 4, 2]`

**Sorted Output:**
`[2, 3, 4, 5, 8]`

---

### 🧠 Time and Space Complexity

| Case       | Time Complexity |
| ---------- | --------------- |
| Best Case  | O(n²)           |
| Average    | O(n²)           |
| Worst Case | O(n²)           |

* **Space Complexity:** O(1) (in-place algorithm)
* **Stable:** ❌ No (can be modified to make stable)

---

### 🧾 Python Code

```python
def selection_sort(arr):
    n = len(arr)
    
    for i in range(n):
        min_index = i  # Assume current index is minimum
        
        for j in range(i+1, n):
            if arr[j] < arr[min_index]:
                min_index = j  # Find actual minimum
        
        # Swap the found minimum with the first unsorted element
        arr[i], arr[min_index] = arr[min_index], arr[i]

    return arr

# Example usage
arr = [5, 3, 8, 4, 2]
sorted_arr = selection_sort(arr)
print("Sorted array:", sorted_arr)
```

---

### ✅ Output

```
Sorted array: [2, 3, 4, 5, 8]
```

---

### 📂 Files

* `selection_sort.py` – Python implementation of selection sort
* `README.md` – Explanation and documentation

---

---

### 👨‍💻 Author

**Rafik Shah**
*Trainer | Developer | Educator*


---
