# JavaScript DSA Interview Questions and Solutions

## Questions List

- [Q1. Flatten a Nested Object](#q1-flatten-a-nested-object)
- [Q2. Unflatten an Object](#q2-unflatten-an-object)
- [Q3. Flatten a Nested Array](#q3-flatten-a-nested-array)
- [Q4. Deep Clone](#q4-deep-clone)
- [Q5. Deep Equality Check](#q5-deep-equality-check)
- [Q6. Group By](#q6-group-by)
- [Q7. Get Value by Path](#q7-get-value-by-path)
- [Q8. Remove Duplicate Objects by Key](#q8-remove-duplicate-objects-by-key)
- [Q9. Character Frequency](#q9-character-frequency)
- [Q10. Debounce](#q10-debounce)
- [Q11. Throttle](#q11-throttle)
- [Q12. Promise.all Polyfill](#q12-promiseall-polyfill)
- [Q13. map, filter, reduce Polyfills](#q13-map-filter-reduce-polyfills)
- [Q14. bind Polyfill](#q14-bind-polyfill)
- [Q15. Currying Sum](#q15-currying-sum)
- [Q16. Memoize](#q16-memoize)
- [Q17. Chunk Array](#q17-chunk-array)
- [Q18. Convert snake_case Keys to camelCase](#q18-convert-snake_case-keys-to-camelcase)
- [Q19. Two Sum](#q19-two-sum)
- [Q20. Contains Duplicate](#q20-contains-duplicate)
- [Q21. Valid Anagram](#q21-valid-anagram)
- [Q22. Group Anagrams](#q22-group-anagrams)
- [Q23. Top K Frequent Elements](#q23-top-k-frequent-elements)
- [Q24. Move Zeroes](#q24-move-zeroes)
- [Q25. Valid Palindrome](#q25-valid-palindrome)
- [Q26. Remove Duplicates from Sorted Array](#q26-remove-duplicates-from-sorted-array)
- [Q27. Best Time to Buy and Sell Stock](#q27-best-time-to-buy-and-sell-stock)
- [Q28. Longest Substring Without Repeating Characters](#q28-longest-substring-without-repeating-characters)
- [Q29. Maximum Subarray (Kadane's Algorithm)](#q29-maximum-subarray-kadanes-algorithm)
- [Q30. Valid Parentheses](#q30-valid-parentheses)
- [Q31. Binary Search](#q31-binary-search)
- [Q32. Merge Intervals](#q32-merge-intervals)
- [Q33. Merge Two Sorted Arrays](#q33-merge-two-sorted-arrays)
- [Q34. Missing Number](#q34-missing-number)
- [Q35. Product of Array Except Self](#q35-product-of-array-except-self)
- [Q36. Reverse Words in a String](#q36-reverse-words-in-a-string)
- [Q37. Climbing Stairs](#q37-climbing-stairs)
- [Q38. Reverse Linked List](#q38-reverse-linked-list)
- [Q39. Merge Two Sorted Linked Lists](#q39-merge-two-sorted-linked-lists)
- [Q40. Linked List Cycle](#q40-linked-list-cycle)
- [Q41. Maximum Depth of Binary Tree](#q41-maximum-depth-of-binary-tree)
- [Q42. Invert Binary Tree](#q42-invert-binary-tree)
- [Q43. Level Order Traversal](#q43-level-order-traversal)
- [Q44. Number of Islands](#q44-number-of-islands)
- [Q45. LRU Cache](#q45-lru-cache)
- [Q46. Rate Limiter](#q46-rate-limiter)
- [Q47. Run Async Tasks with Concurrency Limit](#q47-run-async-tasks-with-concurrency-limit)
- [Q48. Event Emitter](#q48-event-emitter)

---

## Q1. Flatten a Nested Object

Given an object that can contain other objects inside it, convert it into a single-level object. Nested keys are joined with a dot.

**Example:**

```text
Input:  { a: { b: 1, c: { d: 2 } }, e: 3 }
Output: { "a.b": 1, "a.c.d": 2, "e": 3 }
```

**Solution:**

```js
function flattenObject(obj, prefix = "", res = {}) {
  for (const key in obj) {
    const newKey = prefix ? `${prefix}.${key}` : key;
    const val = obj[key];
    if (val !== null && typeof val === "object" && !Array.isArray(val)) {
      flattenObject(val, newKey, res);
    } else {
      res[newKey] = val;
    }
  }
  return res;
}
```

[ ](#table-of-contents)

---

## Q2. Unflatten an Object

Reverse of flatten. Given an object whose keys are dot-separated paths, build the nested object back.

**Example:**

```text
Input:  { "a.b": 1, "a.c.d": 2 }
Output: { a: { b: 1, c: { d: 2 } } }
```

**Solution:**

```js
function unflattenObject(obj) {
  const res = {};
  for (const path in obj) {
    const keys = path.split(".");
    let cur = res;
    for (let i = 0; i < keys.length - 1; i++) {
      if (!cur[keys[i]]) cur[keys[i]] = {};
      cur = cur[keys[i]];
    }
    cur[keys[keys.length - 1]] = obj[path];
  }
  return res;
}
```

[ ](#table-of-contents)

---

## Q3. Flatten a Nested Array

Given an array that can contain arrays inside it, return a single array. Only flatten up to the given depth (default: flatten completely).

**Example:**

```text
Input:  [1, [2, [3, [4]]]], depth = 1
Output: [1, 2, [3, [4]]]
Input:  [1, [2, [3, [4]]]], depth = Infinity
Output: [1, 2, 3, 4]
```

**Solution:**

```js
function flattenArray(arr, depth = Infinity) {
  const res = [];
  for (const item of arr) {
    if (Array.isArray(item) && depth > 0) {
      res.push(...flattenArray(item, depth - 1));
    } else {
      res.push(item);
    }
  }
  return res;
}
```

[ ](#table-of-contents)

---

## Q4. Deep Clone

Create a full copy of an object so that changing the copy (even its nested objects/arrays) does not change the original. Handle arrays, Dates, null and circular references.

**Example:**

```text
Input:  const a = { x: { y: 1 } }; const b = deepClone(a); b.x.y = 5;
Output: a.x.y is still 1
```

**Solution:**

```js
function deepClone(obj, seen = new Map()) {
  if (obj === null || typeof obj !== "object") return obj;
  if (obj instanceof Date) return new Date(obj);
  if (seen.has(obj)) return seen.get(obj);
  const copy = Array.isArray(obj) ? [] : {};
  seen.set(obj, copy);
  for (const key in obj) copy[key] = deepClone(obj[key], seen);
  return copy;
}
```

[ ](#table-of-contents)

---

## Q5. Deep Equality Check

Check whether two values are equal by comparing their contents, not their references. Nested objects and arrays must also match.

**Example:**

```text
Input:  { a: [1, { b: 2 }] }, { a: [1, { b: 2 }] }
Output: true
Input:  { a: 1 }, { a: 2 }
Output: false
```

**Solution:**

```js
function deepEqual(a, b) {
  if (a === b) return true;
  if (a === null || b === null || typeof a !== "object" || typeof b !== "object") return false;
  const keysA = Object.keys(a);
  const keysB = Object.keys(b);
  if (keysA.length !== keysB.length) return false;
  for (const key of keysA) {
    if (!deepEqual(a[key], b[key])) return false;
  }
  return true;
}
```

[ ](#table-of-contents)

---

## Q6. Group By

Given an array of objects and a key, group the objects by the value of that key.

**Example:**

```text
Input:  [{ name: "A", city: "Delhi" }, { name: "B", city: "Pune" }, { name: "C", city: "Delhi" }], "city"
Output: { Delhi: [{A}, {C}], Pune: [{B}] }
```

**Solution:**

```js
function groupBy(arr, key) {
  return arr.reduce((acc, item) => {
    const k = item[key];
    if (!acc[k]) acc[k] = [];
    acc[k].push(item);
    return acc;
  }, {});
}
```

[ ](#table-of-contents)

---

## Q7. Get Value by Path

Given an object and a path string, return the value at that path. If the path does not exist, return the default value instead of throwing an error.

**Example:**

```text
Input:  { a: { b: [{ c: 5 }] } }, "a.b[0].c"
Output: 5
Input:  { a: 1 }, "a.x.y", "N/A"
Output: "N/A"
```

**Solution:**

```js
function get(obj, path, defaultValue) {
  const keys = path.replace(/\[(\d+)\]/g, ".$1").split(".");
  let cur = obj;
  for (const key of keys) {
    if (cur == null) return defaultValue;
    cur = cur[key];
  }
  return cur === undefined ? defaultValue : cur;
}
```

[ ](#table-of-contents)

---

## Q8. Remove Duplicate Objects by Key

Given an array of objects, keep only the first object for each unique value of the given key.

**Example:**

```text
Input:  [{ id: 1 }, { id: 2 }, { id: 1 }], "id"
Output: [{ id: 1 }, { id: 2 }]
```

**Solution:**

```js
function uniqueBy(arr, key) {
  const seen = new Set();
  return arr.filter(item => {
    if (seen.has(item[key])) return false;
    seen.add(item[key]);
    return true;
  });
}
```

[ ](#table-of-contents)

---

## Q9. Character Frequency

Count how many times each character appears in a string.

**Example:**

```text
Input:  "hello"
Output: Map { h: 1, e: 1, l: 2, o: 1 }
```

**Solution:**

```js
function charFrequency(str) {
  const map = new Map();
  for (const ch of str) map.set(ch, (map.get(ch) || 0) + 1);
  return map;
}
```

[ ](#table-of-contents)

---

## Q10. Debounce

Return a function that delays calling fn until `delay` ms have passed since the LAST call. If it is called again before that, the timer resets. Used for search boxes so an API call happens only after the user stops typing.

**Example:**

```text
Input:  type "a", "ab", "abc" quickly with delay = 300
Output: fn runs once with "abc", 300 ms after the last keystroke
```

**Solution:**

```js
function debounce(fn, delay) {
  let timer;
  return function (...args) {
    clearTimeout(timer);
    timer = setTimeout(() => fn.apply(this, args), delay);
  };
}
```

[ ](#table-of-contents)

---

## Q11. Throttle

Return a function that calls fn at most once every `limit` ms, no matter how many times it is triggered. Used for scroll/resize events.

**Example:**

```text
Input:  called 100 times in 1 second with limit = 500
Output: fn runs about 2 times
```

**Solution:**

```js
function throttle(fn, limit) {
  let last = 0;
  return function (...args) {
    const now = Date.now();
    if (now - last >= limit) {
      last = now;
      fn.apply(this, args);
    }
  };
}
```

[ ](#table-of-contents)

---

## Q12. Promise.all Polyfill

Write your own Promise.all. It takes an array of promises and returns one promise that resolves with all results in the same order, or rejects as soon as any one promise rejects.

**Example:**

```text
Input:  [Promise.resolve(1), 2, Promise.resolve(3)]
Output: resolves to [1, 2, 3]
```

**Solution:**

```js
function promiseAll(promises) {
  return new Promise((resolve, reject) => {
    const results = [];
    let done = 0;
    if (promises.length === 0) return resolve(results);
    promises.forEach((p, i) => {
      Promise.resolve(p).then(val => {
        results[i] = val;
        done++;
        if (done === promises.length) resolve(results);
      }).catch(reject);
    });
  });
}
```

[ ](#table-of-contents)

---

## Q13. map, filter, reduce Polyfills

Write your own versions of Array.prototype.map, filter and reduce without using the built-in ones.

**Example:**

```text
Input:  [1, 2, 3].myMap(x => x * 2)            Output: [2, 4, 6]
Input:  [1, 2, 3].myFilter(x => x > 1)         Output: [2, 3]
Input:  [1, 2, 3].myReduce((a, b) => a + b, 0) Output: 6
```

**Solution:**

```js
Array.prototype.myMap = function (cb) {
  const res = [];
  for (let i = 0; i < this.length; i++) res.push(cb(this[i], i, this));
  return res;
};

Array.prototype.myFilter = function (cb) {
  const res = [];
  for (let i = 0; i < this.length; i++) if (cb(this[i], i, this)) res.push(this[i]);
  return res;
};

Array.prototype.myReduce = function (cb, initial) {
  let acc = initial;
  let start = 0;
  if (acc === undefined) {
    acc = this[0];
    start = 1;
  }
  for (let i = start; i < this.length; i++) acc = cb(acc, this[i], i, this);
  return acc;
};
```

[ ](#table-of-contents)

---

## Q14. bind Polyfill

Write your own Function.prototype.bind. It returns a new function with `this` fixed to the given context, and can also pre-fill some arguments.

**Example:**

```text
Input:  function greet(g) { return g + " " + this.name; }
        greet.myBind({ name: "Ravi" }, "Hi")()
Output: "Hi Ravi"
```

**Solution:**

```js
Function.prototype.myBind = function (context, ...args1) {
  const fn = this;
  return function (...args2) {
    return fn.apply(context, [...args1, ...args2]);
  };
};
```

[ ](#table-of-contents)

---

## Q15. Currying Sum

Write a function sum that can be called like sum(1)(2)(3)() and returns the total when called with no argument.

**Example:**

```text
Input:  sum(1)(2)(3)()
Output: 6
```

**Solution:**

```js
function sum(a) {
  return function (b) {
    if (b === undefined) return a;
    return sum(a + b);
  };
}
```

[ ](#table-of-contents)

---

## Q16. Memoize

Return a version of fn that caches results. If it is called again with the same arguments, return the cached result instead of recomputing.

**Example:**

```text
Input:  const slowSquare = memoize(n => n * n); slowSquare(4); slowSquare(4);
Output: 16 both times, but the calculation runs only once
```

**Solution:**

```js
function memoize(fn) {
  const cache = new Map();
  return function (...args) {
    const key = JSON.stringify(args);
    if (cache.has(key)) return cache.get(key);
    const result = fn.apply(this, args);
    cache.set(key, result);
    return result;
  };
}
```

[ ](#table-of-contents)

---

## Q17. Chunk Array

Split an array into smaller arrays of the given size. The last chunk can be smaller.

**Example:**

```text
Input:  [1, 2, 3, 4, 5], 2
Output: [[1, 2], [3, 4], [5]]
```

**Solution:**

```js
function chunk(arr, size) {
  const res = [];
  for (let i = 0; i < arr.length; i += size) res.push(arr.slice(i, i + size));
  return res;
}
```

[ ](#table-of-contents)

---

## Q18. Convert snake_case Keys to camelCase

Convert every key of an object (including nested objects and objects inside arrays) from snake_case to camelCase.

**Example:**

```text
Input:  { user_name: "a", user_info: { first_name: "b" } }
Output: { userName: "a", userInfo: { firstName: "b" } }
```

**Solution:**

```js
function toCamel(obj) {
  if (Array.isArray(obj)) return obj.map(toCamel);
  if (obj === null || typeof obj !== "object") return obj;
  const res = {};
  for (const key in obj) {
    const newKey = key.replace(/_([a-z])/g, (_, c) => c.toUpperCase());
    res[newKey] = toCamel(obj[key]);
  }
  return res;
}
```

[ ](#table-of-contents)

---

## Q19. Two Sum

Given an array of numbers and a target, return the indices of the two numbers that add up to the target. Exactly one answer exists.

**Example:**

```text
Input:  nums = [2, 7, 11, 15], target = 9
Output: [0, 1]   (2 + 7 = 9)
```

**Solution:**

```js
function twoSum(nums, target) {
  const map = new Map();
  for (let i = 0; i < nums.length; i++) {
    const need = target - nums[i];
    if (map.has(need)) return [map.get(need), i];
    map.set(nums[i], i);
  }
  return [];
}
```

[ ](#table-of-contents)

---

## Q20. Contains Duplicate

Return true if any value appears at least twice in the array.

**Example:**

```text
Input:  [1, 2, 3, 1]
Output: true
Input:  [1, 2, 3]
Output: false
```

**Solution:**

```js
function containsDuplicate(nums) {
  return new Set(nums).size !== nums.length;
}
```

[ ](#table-of-contents)

---

## Q21. Valid Anagram

Return true if string t is an anagram of s (same letters, same counts, different order allowed).

**Example:**

```text
Input:  s = "listen", t = "silent"
Output: true
Input:  s = "rat", t = "car"
Output: false
```

**Solution:**

```js
function isAnagram(s, t) {
  if (s.length !== t.length) return false;
  const count = {};
  for (const ch of s) count[ch] = (count[ch] || 0) + 1;
  for (const ch of t) {
    if (!count[ch]) return false;
    count[ch]--;
  }
  return true;
}
```

[ ](#table-of-contents)

---

## Q22. Group Anagrams

Given an array of strings, group the words that are anagrams of each other.

**Example:**

```text
Input:  ["eat", "tea", "tan", "ate", "nat", "bat"]
Output: [["eat", "tea", "ate"], ["tan", "nat"], ["bat"]]
```

**Solution:**

```js
function groupAnagrams(strs) {
  const map = new Map();
  for (const s of strs) {
    const key = s.split("").sort().join("");
    if (!map.has(key)) map.set(key, []);
    map.get(key).push(s);
  }
  return [...map.values()];
}
```

[ ](#table-of-contents)

---

## Q23. Top K Frequent Elements

Return the k numbers that appear most often in the array.

**Example:**

```text
Input:  nums = [1, 1, 1, 2, 2, 3], k = 2
Output: [1, 2]
```

**Solution:**

```js
function topKFrequent(nums, k) {
  const count = new Map();
  for (const n of nums) count.set(n, (count.get(n) || 0) + 1);
  const buckets = Array.from({ length: nums.length + 1 }, () => []);
  for (const [num, freq] of count) buckets[freq].push(num);
  const res = [];
  for (let i = buckets.length - 1; i >= 0 && res.length < k; i--) res.push(...buckets[i]);
  return res.slice(0, k);
}
```

[ ](#table-of-contents)

---

## Q24. Move Zeroes

Move all 0s to the end of the array while keeping the order of the other numbers. Do it in place.

**Example:**

```text
Input:  [0, 1, 0, 3, 12]
Output: [1, 3, 12, 0, 0]
```

**Solution:**

```js
function moveZeroes(nums) {
  let pos = 0;
  for (let i = 0; i < nums.length; i++) {
    if (nums[i] !== 0) {
      [nums[pos], nums[i]] = [nums[i], nums[pos]];
      pos++;
    }
  }
  return nums;
}
```

[ ](#table-of-contents)

---

## Q25. Valid Palindrome

After converting to lowercase and removing everything except letters and digits, check if the string reads the same forwards and backwards.

**Example:**

```text
Input:  "A man, a plan, a canal: Panama"
Output: true
Input:  "race a car"
Output: false
```

**Solution:**

```js
function isPalindrome(s) {
  const clean = s.toLowerCase().replace(/[^a-z0-9]/g, "");
  let l = 0, r = clean.length - 1;
  while (l < r) {
    if (clean[l] !== clean[r]) return false;
    l++;
    r--;
  }
  return true;
}
```

[ ](#table-of-contents)

---

## Q26. Remove Duplicates from Sorted Array

Given a sorted array, remove duplicates in place so each value appears once. Return the count of unique values (they must be at the front).

**Example:**

```text
Input:  [1, 1, 2, 3, 3]
Output: 3   (array starts with [1, 2, 3, ...])
```

**Solution:**

```js
function removeDuplicates(nums) {
  if (nums.length === 0) return 0;
  let k = 1;
  for (let i = 1; i < nums.length; i++) {
    if (nums[i] !== nums[k - 1]) nums[k++] = nums[i];
  }
  return k;
}
```

[ ](#table-of-contents)

---

## Q27. Best Time to Buy and Sell Stock

prices[i] is the stock price on day i. Buy on one day and sell on a later day. Return the maximum profit, or 0 if no profit is possible.

**Example:**

```text
Input:  [7, 1, 5, 3, 6, 4]
Output: 5   (buy at 1, sell at 6)
```

**Solution:**

```js
function maxProfit(prices) {
  let min = Infinity, profit = 0;
  for (const p of prices) {
    min = Math.min(min, p);
    profit = Math.max(profit, p - min);
  }
  return profit;
}
```

[ ](#table-of-contents)

---

## Q28. Longest Substring Without Repeating Characters

Return the length of the longest continuous part of the string that has no repeated characters.

**Example:**

```text
Input:  "abcabcbb"
Output: 3   ("abc")
Input:  "pwwkew"
Output: 3   ("wke")
```

**Solution:**

```js
function lengthOfLongestSubstring(s) {
  const lastSeen = new Map();
  let left = 0, best = 0;
  for (let right = 0; right < s.length; right++) {
    if (lastSeen.has(s[right]) && lastSeen.get(s[right]) >= left) {
      left = lastSeen.get(s[right]) + 1;
    }
    lastSeen.set(s[right], right);
    best = Math.max(best, right - left + 1);
  }
  return best;
}
```

[ ](#table-of-contents)

---

## Q29. Maximum Subarray (Kadane's Algorithm)

Find the continuous subarray with the largest sum and return that sum.

**Example:**

```text
Input:  [-2, 1, -3, 4, -1, 2, 1, -5, 4]
Output: 6   ([4, -1, 2, 1])
```

**Solution:**

```js
function maxSubArray(nums) {
  let cur = nums[0], best = nums[0];
  for (let i = 1; i < nums.length; i++) {
    cur = Math.max(nums[i], cur + nums[i]);
    best = Math.max(best, cur);
  }
  return best;
}
```

[ ](#table-of-contents)

---

## Q30. Valid Parentheses

Given a string of brackets ()[]{}, return true if every opening bracket is closed by the same type of bracket in the correct order.

**Example:**

```text
Input:  "([]{})"
Output: true
Input:  "(]"
Output: false
```

**Solution:**

```js
function isValid(s) {
  const stack = [];
  const pairs = { ")": "(", "]": "[", "}": "{" };
  for (const ch of s) {
    if (ch === "(" || ch === "[" || ch === "{") stack.push(ch);
    else if (stack.pop() !== pairs[ch]) return false;
  }
  return stack.length === 0;
}
```

[ ](#table-of-contents)

---

## Q31. Binary Search

Given a sorted array and a target, return the index of the target, or -1 if it is not present. Must run in O(log n).

**Example:**

```text
Input:  nums = [-1, 0, 3, 5, 9, 12], target = 9
Output: 4
```

**Solution:**

```js
function binarySearch(nums, target) {
  let l = 0, r = nums.length - 1;
  while (l <= r) {
    const mid = Math.floor((l + r) / 2);
    if (nums[mid] === target) return mid;
    if (nums[mid] < target) l = mid + 1;
    else r = mid - 1;
  }
  return -1;
}
```

[ ](#table-of-contents)

---

## Q32. Merge Intervals

Given a list of [start, end] intervals, merge all overlapping intervals.

**Example:**

```text
Input:  [[1, 3], [2, 6], [8, 10], [15, 18]]
Output: [[1, 6], [8, 10], [15, 18]]
```

**Solution:**

```js
function mergeIntervals(intervals) {
  intervals.sort((a, b) => a[0] - b[0]);
  const res = [];
  for (const [start, end] of intervals) {
    if (res.length && start <= res[res.length - 1][1]) {
      res[res.length - 1][1] = Math.max(res[res.length - 1][1], end);
    } else {
      res.push([start, end]);
    }
  }
  return res;
}
```

[ ](#table-of-contents)

---

## Q33. Merge Two Sorted Arrays

Given two sorted arrays, return one sorted array containing all elements.

**Example:**

```text
Input:  [1, 3, 5], [2, 4, 6]
Output: [1, 2, 3, 4, 5, 6]
```

**Solution:**

```js
function mergeSortedArrays(a, b) {
  const res = [];
  let i = 0, j = 0;
  while (i < a.length && j < b.length) {
    if (a[i] <= b[j]) res.push(a[i++]);
    else res.push(b[j++]);
  }
  while (i < a.length) res.push(a[i++]);
  while (j < b.length) res.push(b[j++]);
  return res;
}
```

[ ](#table-of-contents)

---

## Q34. Missing Number

The array contains n distinct numbers from the range 0 to n. One number is missing. Return it.

**Example:**

```text
Input:  [3, 0, 1]
Output: 2
```

**Solution:**

```js
function missingNumber(nums) {
  const n = nums.length;
  let total = (n * (n + 1)) / 2;
  for (const x of nums) total -= x;
  return total;
}
```

[ ](#table-of-contents)

---

## Q35. Product of Array Except Self

Return an array where each position holds the product of all other elements. Do not use division.

**Example:**

```text
Input:  [1, 2, 3, 4]
Output: [24, 12, 8, 6]
```

**Solution:**

```js
function productExceptSelf(nums) {
  const res = new Array(nums.length).fill(1);
  let prefix = 1;
  for (let i = 0; i < nums.length; i++) {
    res[i] = prefix;
    prefix *= nums[i];
  }
  let suffix = 1;
  for (let i = nums.length - 1; i >= 0; i--) {
    res[i] *= suffix;
    suffix *= nums[i];
  }
  return res;
}
```

[ ](#table-of-contents)

---

## Q36. Reverse Words in a String

Reverse the order of words. Remove extra spaces at the start, end and between words.

**Example:**

```text
Input:  "  the sky   is blue "
Output: "blue is sky the"
```

**Solution:**

```js
function reverseWords(s) {
  return s.trim().split(/\s+/).reverse().join(" ");
}
```

[ ](#table-of-contents)

---

## Q37. Climbing Stairs

You can climb 1 or 2 steps at a time. In how many different ways can you reach the top of n stairs?

**Example:**

```text
Input:  n = 3
Output: 3   (1+1+1, 1+2, 2+1)
```

**Solution:**

```js
function climbStairs(n) {
  let a = 1, b = 1;
  for (let i = 2; i <= n; i++) [a, b] = [b, a + b];
  return b;
}
```

[ ](#table-of-contents)

---

## Q38. Reverse Linked List

Reverse a singly linked list and return the new head.

**Example:**

```text
Input:  1 -> 2 -> 3 -> 4 -> null
Output: 4 -> 3 -> 2 -> 1 -> null
```

**Solution:**

```js
// Helper: linked list node
class ListNode {
  constructor(val, next = null) {
    this.val = val;
    this.next = next;
  }
}

function reverseList(head) {
  let prev = null, cur = head;
  while (cur) {
    const next = cur.next;
    cur.next = prev;
    prev = cur;
    cur = next;
  }
  return prev;
}
```

[ ](#table-of-contents)

---

## Q39. Merge Two Sorted Linked Lists

Merge two sorted linked lists into one sorted linked list.

**Example:**

```text
Input:  1 -> 2 -> 4,  1 -> 3 -> 4
Output: 1 -> 1 -> 2 -> 3 -> 4 -> 4
```

**Solution:**

```js
function mergeTwoLists(l1, l2) {
  const dummy = new ListNode(0);
  let tail = dummy;
  while (l1 && l2) {
    if (l1.val <= l2.val) {
      tail.next = l1;
      l1 = l1.next;
    } else {
      tail.next = l2;
      l2 = l2.next;
    }
    tail = tail.next;
  }
  tail.next = l1 || l2;
  return dummy.next;
}
```

[ ](#table-of-contents)

---

## Q40. Linked List Cycle

Return true if the linked list has a cycle (some node's next points back to an earlier node).

**Example:**

```text
Input:  3 -> 2 -> 0 -> -4 -> (back to 2)
Output: true
```

**Solution:**

```js
function hasCycle(head) {
  let slow = head, fast = head;
  while (fast && fast.next) {
    slow = slow.next;
    fast = fast.next.next;
    if (slow === fast) return true;
  }
  return false;
}
```

[ ](#table-of-contents)

---

## Q41. Maximum Depth of Binary Tree

Return the number of nodes on the longest path from the root down to a leaf.

**Example:**

```text
Input:      3
           / \
          9  20
             / \
            15  7
Output: 3
```

**Solution:**

```js
// Helper: binary tree node
class TreeNode {
  constructor(val, left = null, right = null) {
    this.val = val;
    this.left = left;
    this.right = right;
  }
}

function maxDepth(root) {
  if (!root) return 0;
  return 1 + Math.max(maxDepth(root.left), maxDepth(root.right));
}
```

[ ](#table-of-contents)

---

## Q42. Invert Binary Tree

Swap the left and right child of every node (mirror the tree).

**Example:**

```text
Input:      4            Output:     4
           / \                      / \
          2   7                    7   2
         / \ / \                  / \ / \
        1  3 6  9                9  6 3  1
```

**Solution:**

```js
function invertTree(root) {
  if (!root) return null;
  [root.left, root.right] = [invertTree(root.right), invertTree(root.left)];
  return root;
}
```

[ ](#table-of-contents)

---

## Q43. Level Order Traversal

Return the values of a binary tree level by level, from top to bottom.

**Example:**

```text
Input:      3
           / \
          9  20
             / \
            15  7
Output: [[3], [9, 20], [15, 7]]
```

**Solution:**

```js
function levelOrder(root) {
  if (!root) return [];
  const res = [];
  let queue = [root];
  while (queue.length) {
    const level = [];
    const next = [];
    for (const node of queue) {
      level.push(node.val);
      if (node.left) next.push(node.left);
      if (node.right) next.push(node.right);
    }
    res.push(level);
    queue = next;
  }
  return res;
}
```

[ ](#table-of-contents)

---

## Q44. Number of Islands

Given a grid of "1" (land) and "0" (water), count the islands. An island is land connected up/down/left/right.

**Example:**

```text
Input:  [["1","1","0"],
         ["0","1","0"],
         ["0","0","1"]]
Output: 2
```

**Solution:**

```js
function numIslands(grid) {
  const rows = grid.length, cols = grid[0].length;
  let count = 0;
  function dfs(r, c) {
    if (r < 0 || c < 0 || r >= rows || c >= cols || grid[r][c] !== "1") return;
    grid[r][c] = "0";
    dfs(r + 1, c);
    dfs(r - 1, c);
    dfs(r, c + 1);
    dfs(r, c - 1);
  }
  for (let r = 0; r < rows; r++) {
    for (let c = 0; c < cols; c++) {
      if (grid[r][c] === "1") {
        count++;
        dfs(r, c);
      }
    }
  }
  return count;
}
```

[ ](#table-of-contents)

---

## Q45. LRU Cache

Design a cache with a fixed capacity.

- `get(key)`: return the value if present, else -1.
- `put(key, value)`: insert or update. If the cache is over capacity, remove the
least recently used key. Both operations should be O(1).

**Example:**

```text
Input:  capacity 2: put(1,1), put(2,2), get(1), put(3,3), get(2)
Output: get(1) = 1, get(2) = -1 (key 2 was evicted)
```

**Solution:**

```js
class LRUCache {
  constructor(capacity) {
    this.capacity = capacity;
    this.map = new Map();
  }
  get(key) {
    if (!this.map.has(key)) return -1;
    const val = this.map.get(key);
    this.map.delete(key);
    this.map.set(key, val);
    return val;
  }
  put(key, value) {
    if (this.map.has(key)) this.map.delete(key);
    this.map.set(key, value);
    if (this.map.size > this.capacity) {
      this.map.delete(this.map.keys().next().value);
    }
  }
}
```

[ ](#table-of-contents)

---

## Q46. Rate Limiter

Allow each user at most `limit` requests in any `windowMs` time window. allow(userId) returns true if the request is allowed, else false.

**Example:**

```text
Input:  limit = 3, windowMs = 1000, user calls allow() 4 times in 1 second
Output: true, true, true, false
```

**Solution:**

```js
class RateLimiter {
  constructor(limit, windowMs) {
    this.limit = limit;
    this.windowMs = windowMs;
    this.requests = new Map();
  }
  allow(userId) {
    const now = Date.now();
    const times = (this.requests.get(userId) || []).filter(t => now - t < this.windowMs);
    if (times.length >= this.limit) {
      this.requests.set(userId, times);
      return false;
    }
    times.push(now);
    this.requests.set(userId, times);
    return true;
  }
}
```

[ ](#table-of-contents)

---

## Q47. Run Async Tasks with Concurrency Limit

Given an array of functions that return promises, run them so that at most `limit` tasks are running at the same time. Return all results in the original order.

**Example:**

```text
Input:  5 tasks, limit = 2
Output: tasks run 2 at a time; resolves to [r1, r2, r3, r4, r5]
```

**Solution:**

```js
async function runWithLimit(tasks, limit) {
  const results = [];
  let index = 0;
  async function worker() {
    while (index < tasks.length) {
      const i = index++;
      results[i] = await tasks[i]();
    }
  }
  const workers = Array.from({ length: Math.min(limit, tasks.length) }, worker);
  await Promise.all(workers);
  return results;
}
```

[ ](#table-of-contents)

---

## Q48. Event Emitter

Build a class with:

- `on(event, fn)`: subscribe fn to an event
- `off(event, fn)`: unsubscribe fn
- `emit(event, ...args)`: call all subscribers with args
- `once(event, fn)`: subscribe fn so it runs only the first time

**Example:**

```text
Input:  e.on("msg", console.log); e.emit("msg", "hi");
Output: logs "hi"
```

**Solution:**

```js
class EventEmitter {
  constructor() {
    this.events = {};
  }
  on(event, listener) {
    (this.events[event] ||= []).push(listener);
  }
  off(event, listener) {
    this.events[event] = (this.events[event] || []).filter(l => l !== listener);
  }
  emit(event, ...args) {
    (this.events[event] || []).slice().forEach(l => l(...args));
  }
  once(event, listener) {
    const wrapper = (...args) => {
      listener(...args);
      this.off(event, wrapper);
    };
    this.on(event, wrapper);
  }
}
```

[ ](#table-of-contents)
