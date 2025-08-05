
---

### ✅ Simplest Insertion Sort Logic

```python
def insertion_sort(arr):
    for i in range(1, len(arr)):
        key = arr[i]
        j = i - 1

        while j >= 0 and arr[j] > key:
            arr[j + 1] = arr[j]
            j -= 1

        arr[j + 1] = key

    return arr

arr = [5, 3, 8, 4, 2]
print("Sorted array:", insertion_sort(arr))
```

---

### 🧾 Output:

```
Sorted array: [2, 3, 4, 5, 8]
```

---

