# JavaScript DOM & Events – Interview Questions

This document covers important JavaScript DOM manipulation and event handling concepts commonly asked in interviews.

---

## 1. Difference Between getElementById, getElementsByClassName, and querySelector / querySelectorAll

### getElementById()

- Selects one element by its unique `id`.
- Returns a single element or `null`.
- Faster because IDs are unique.

```javascript
const element = document.getElementById("myId");