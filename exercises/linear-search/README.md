# Linear Search

## 📝 Challenge Description

Your task is to implement a **Linear Search** algorithm in the Rust programming language. Linear Search is a simple search technique used to find a specific element in a list by checking each element one by one from the beginning to the end.

This challenge is designed to test your understanding of:

- Iteration and indexing in Rust
- Use of generics and traits like `PartialEq`
- Handling different input scenarios (e.g., empty arrays, missing targets)
- Writing and running unit tests

---

## 🎯 Requirements

- Implement a function named `linear_search` that:
  - Accepts a **slice** of items (`&[T]`)
  - Accepts a **target** item to search for
  - Returns the **index** of the target item if found (`Some(index)`)
  - Returns `None` if the item is not present

```rust
fn linear_search<T: PartialEq>(arr: &[T], target: T) -> Option<usize>
```

---

## ✅ Example
```rust
let numbers = vec![10, 20, 30, 40];
let target = 30;

let result = linear_search(&numbers, target);
// result should be Some(2)
```

---

## 🧪 Bonus: Add Unit Tests

Include test cases that verify your implementation against:
- A list containing the target element
- A list that does not contain the target element
- An empty list
- Target element being the first or last item

Use Rust’s built-in test framework (#[cfg(test)]) to structure your tests.

