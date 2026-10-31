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
- [Q49. Promise.allSettled Polyfill](#q49-promiseallsettled-polyfill)
- [Q50. Promise.race Polyfill](#q50-promiserace-polyfill)
- [Q51. Retry with Exponential Backoff](#q51-retry-with-exponential-backoff)
- [Q52. Parse Query String](#q52-parse-query-string)
- [Q53. Object to Query String](#q53-object-to-query-string)
- [Q54. Deep Merge Two Objects](#q54-deep-merge-two-objects)
- [Q55. setInterval Using setTimeout](#q55-setinterval-using-settimeout)
- [Q56. First Non-Repeating Character](#q56-first-non-repeating-character)
- [Q57. Longest Common Prefix](#q57-longest-common-prefix)
- [Q58. Reverse Integer](#q58-reverse-integer)
- [Q59. Palindrome Number](#q59-palindrome-number)
- [Q60. String Compression](#q60-string-compression)
- [Q61. Merge Sort](#q61-merge-sort)
- [Q62. Quick Sort](#q62-quick-sort)
- [Q63. Sort Objects by Multiple Keys](#q63-sort-objects-by-multiple-keys)
- [Q64. 3Sum](#q64-3sum)
- [Q65. Container With Most Water](#q65-container-with-most-water)
- [Q66. Subarray Sum Equals K](#q66-subarray-sum-equals-k)
- [Q67. Rotate Array](#q67-rotate-array)
- [Q68. Majority Element](#q68-majority-element)
- [Q69. Min Stack](#q69-min-stack)
- [Q70. Daily Temperatures](#q70-daily-temperatures)
- [Q71. Search in Rotated Sorted Array](#q71-search-in-rotated-sorted-array)
- [Q72. First and Last Position of an Element](#q72-first-and-last-position-of-an-element)
- [Q73. Insert Interval](#q73-insert-interval)
- [Q74. Meeting Rooms](#q74-meeting-rooms)
- [Q75. Meeting Rooms II](#q75-meeting-rooms-ii)
- [Q76. Middle of the Linked List](#q76-middle-of-the-linked-list)
- [Q77. Remove Nth Node From End of List](#q77-remove-nth-node-from-end-of-list)
- [Q78. Validate Binary Search Tree](#q78-validate-binary-search-tree)
- [Q79. Lowest Common Ancestor of a Binary Tree](#q79-lowest-common-ancestor-of-a-binary-tree)
- [Q80. Diameter of Binary Tree](#q80-diameter-of-binary-tree)
- [Q81. Min Heap](#q81-min-heap)
- [Q82. Kth Largest Element in an Array](#q82-kth-largest-element-in-an-array)
- [Q83. Merge K Sorted Linked Lists](#q83-merge-k-sorted-linked-lists)
- [Q84. Graph BFS and DFS Traversal](#q84-graph-bfs-and-dfs-traversal)
- [Q85. Course Schedule (Topological Sort)](#q85-course-schedule-topological-sort)
- [Q86. Rotting Oranges](#q86-rotting-oranges)
- [Q87. Subsets](#q87-subsets)
- [Q88. Permutations](#q88-permutations)
- [Q89. Combination Sum](#q89-combination-sum)
- [Q90. House Robber](#q90-house-robber)
- [Q91. Coin Change](#q91-coin-change)
- [Q92. Longest Common Subsequence](#q92-longest-common-subsequence)

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

---

## Q49. Promise.allSettled Polyfill

Write your own Promise.allSettled. It waits for every promise to finish (resolve or reject) and returns the status and value/reason of each one, in the same order. It never rejects.

**Example:**

```text
Input:  [Promise.resolve(1), Promise.reject("err")]
Output: [{ status: "fulfilled", value: 1 }, { status: "rejected", reason: "err" }]
```

**Solution:**

```js
function promiseAllSettled(promises) {
  return new Promise(resolve => {
    const results = [];
    let done = 0;
    if (promises.length === 0) return resolve(results);
    promises.forEach((p, i) => {
      Promise.resolve(p)
        .then(value => (results[i] = { status: "fulfilled", value }))
        .catch(reason => (results[i] = { status: "rejected", reason }))
        .finally(() => {
          done++;
          if (done === promises.length) resolve(results);
        });
    });
  });
}
```

---

## Q50. Promise.race Polyfill

Write your own Promise.race. It returns a promise that settles (resolves or rejects) as soon as the first promise in the array settles.

**Example:**

```text
Input:  [wait(500, "slow"), wait(100, "fast")]
Output: resolves to "fast"
```

**Solution:**

```js
function promiseRace(promises) {
  return new Promise((resolve, reject) => {
    for (const p of promises) {
      Promise.resolve(p).then(resolve, reject);
    }
  });
}
```

---

## Q51. Retry with Exponential Backoff

Given an async function, call it. If it fails, retry it up to `retries` times. Wait `delay` ms before the first retry and double the wait each time. If all attempts fail, throw the last error.

**Example:**

```text
Input:  a function that fails twice then succeeds, retries = 3, delay = 100
Output: resolves with the result after waiting 100 ms, then 200 ms
```

**Solution:**

```js
async function retry(fn, retries = 3, delay = 100) {
  try {
    return await fn();
  } catch (err) {
    if (retries === 0) throw err;
    await new Promise(res => setTimeout(res, delay));
    return retry(fn, retries - 1, delay * 2);
  }
}
```

---

## Q52. Parse Query String

Convert a URL query string into an object. Decode encoded characters. If a key appears more than once, store its values in an array.

**Example:**

```text
Input:  "?name=Ravi%20Kumar&age=22&tag=js&tag=node"
Output: { name: "Ravi Kumar", age: "22", tag: ["js", "node"] }
```

**Solution:**

```js
function parseQueryString(str) {
  const res = {};
  const query = str.startsWith("?") ? str.slice(1) : str;
  if (!query) return res;
  for (const pair of query.split("&")) {
    const [rawKey, rawVal = ""] = pair.split("=");
    const key = decodeURIComponent(rawKey);
    const val = decodeURIComponent(rawVal);
    if (key in res) {
      res[key] = Array.isArray(res[key]) ? [...res[key], val] : [res[key], val];
    } else {
      res[key] = val;
    }
  }
  return res;
}
```

---

## Q53. Object to Query String

Convert an object into a URL query string. Encode special characters. Array values become repeated keys.

**Example:**

```text
Input:  { name: "Ravi Kumar", tag: ["js", "node"] }
Output: "name=Ravi%20Kumar&tag=js&tag=node"
```

**Solution:**

```js
function toQueryString(obj) {
  const parts = [];
  for (const key in obj) {
    const values = Array.isArray(obj[key]) ? obj[key] : [obj[key]];
    for (const val of values) {
      parts.push(`${encodeURIComponent(key)}=${encodeURIComponent(val)}`);
    }
  }
  return parts.join("&");
}
```

---

## Q54. Deep Merge Two Objects

Merge source into target and return a new object. If both have an object at the same key, merge those objects too. Otherwise the source value wins.

**Example:**

```text
Input:  { a: 1, b: { x: 1, y: 2 } }, { b: { y: 3, z: 4 }, c: 5 }
Output: { a: 1, b: { x: 1, y: 3, z: 4 }, c: 5 }
```

**Solution:**

```js
function deepMerge(target, source) {
  const isObj = v => v !== null && typeof v === "object" && !Array.isArray(v);
  const res = { ...target };
  for (const key in source) {
    if (isObj(res[key]) && isObj(source[key])) {
      res[key] = deepMerge(res[key], source[key]);
    } else {
      res[key] = source[key];
    }
  }
  return res;
}
```

---

## Q55. setInterval Using setTimeout

Implement mySetInterval(fn, delay) that calls fn every `delay` ms, using only setTimeout. It should return a function that stops the interval.

**Example:**

```text
Input:  const stop = mySetInterval(() => console.log("tick"), 1000);
        stop() after 3.5 seconds
Output: logs "tick" 3 times
```

**Solution:**

```js
function mySetInterval(fn, delay) {
  let timer;
  let active = true;
  function run() {
    timer = setTimeout(() => {
      if (!active) return;
      fn();
      run();
    }, delay);
  }
  run();
  return function clear() {
    active = false;
    clearTimeout(timer);
  };
}
```

---

## Q56. First Non-Repeating Character

Return the index of the first character that appears only once in the string. Return -1 if there is none.

**Example:**

```text
Input:  "leetcode"
Output: 0   ("l")
Input:  "aabb"
Output: -1
```

**Solution:**

```js
function firstUniqChar(s) {
  const count = new Map();
  for (const ch of s) count.set(ch, (count.get(ch) || 0) + 1);
  for (let i = 0; i < s.length; i++) {
    if (count.get(s[i]) === 1) return i;
  }
  return -1;
}
```

---

## Q57. Longest Common Prefix

Return the longest starting part that all strings share. Return "" if there is none.

**Example:**

```text
Input:  ["flower", "flow", "flight"]
Output: "fl"
```

**Solution:**

```js
function longestCommonPrefix(strs) {
  if (strs.length === 0) return "";
  let prefix = strs[0];
  for (const s of strs) {
    while (!s.startsWith(prefix)) prefix = prefix.slice(0, -1);
  }
  return prefix;
}
```

---

## Q58. Reverse Integer

Reverse the digits of an integer. Keep the sign. If the result goes outside the 32-bit signed integer range, return 0.

**Example:**

```text
Input:  123     Output: 321
Input:  -120    Output: -21
```

**Solution:**

```js
function reverseInteger(x) {
  const sign = x < 0 ? -1 : 1;
  const rev = sign * parseInt(String(Math.abs(x)).split("").reverse().join(""));
  if (rev > 2 ** 31 - 1 || rev < -(2 ** 31)) return 0;
  return rev;
}
```

---

## Q59. Palindrome Number

Return true if the integer reads the same forwards and backwards, without converting it to a string. Negative numbers are not palindromes.

**Example:**

```text
Input:  121    Output: true
Input:  -121   Output: false
```

**Solution:**

```js
function isPalindromeNumber(x) {
  if (x < 0) return false;
  let original = x, rev = 0;
  while (x > 0) {
    rev = rev * 10 + (x % 10);
    x = Math.floor(x / 10);
  }
  return rev === original;
}
```

---

## Q60. String Compression

Replace each group of repeated characters with the character followed by its count. If the compressed string is not shorter, return the original.

**Example:**

```text
Input:  "aaabbbcc"
Output: "a3b3c2"
Input:  "abc"
Output: "abc"
```

**Solution:**

```js
function compressString(s) {
  let res = "";
  let count = 1;
  for (let i = 1; i <= s.length; i++) {
    if (s[i] === s[i - 1]) {
      count++;
    } else {
      res += s[i - 1] + count;
      count = 1;
    }
  }
  return res.length < s.length ? res : s;
}
```

---

## Q61. Merge Sort

Sort an array of numbers using merge sort: split the array in half, sort each half, then merge the two sorted halves. Time O(n log n).

**Example:**

```text
Input:  [5, 2, 4, 6, 1, 3]
Output: [1, 2, 3, 4, 5, 6]
```

**Solution:**

```js
function mergeSort(arr) {
  if (arr.length <= 1) return arr;
  const mid = Math.floor(arr.length / 2);
  const left = mergeSort(arr.slice(0, mid));
  const right = mergeSort(arr.slice(mid));
  const res = [];
  let i = 0, j = 0;
  while (i < left.length && j < right.length) {
    if (left[i] <= right[j]) res.push(left[i++]);
    else res.push(right[j++]);
  }
  return [...res, ...left.slice(i), ...right.slice(j)];
}
```

---

## Q62. Quick Sort

Sort an array of numbers in place using quick sort: pick a pivot, move smaller elements to its left and larger ones to its right, then sort both sides. Average time O(n log n).

**Example:**

```text
Input:  [10, 7, 8, 9, 1, 5]
Output: [1, 5, 7, 8, 9, 10]
```

**Solution:**

```js
function quickSort(arr, low = 0, high = arr.length - 1) {
  if (low < high) {
    const pivot = arr[high];
    let i = low;
    for (let j = low; j < high; j++) {
      if (arr[j] < pivot) {
        [arr[i], arr[j]] = [arr[j], arr[i]];
        i++;
      }
    }
    [arr[i], arr[high]] = [arr[high], arr[i]];
    quickSort(arr, low, i - 1);
    quickSort(arr, i + 1, high);
  }
  return arr;
}
```

---

## Q63. Sort Objects by Multiple Keys

Sort an array of users by age ascending. If ages are equal, sort by name alphabetically.

**Example:**

```text
Input:  [{ name: "Ravi", age: 25 }, { name: "Amit", age: 22 }, { name: "Neha", age: 22 }]
Output: [{ Amit, 22 }, { Neha, 22 }, { Ravi, 25 }]
```

**Solution:**

```js
function sortUsers(users) {
  return [...users].sort((a, b) => a.age - b.age || a.name.localeCompare(b.name));
}
```

---

## Q64. 3Sum

Return all unique triplets in the array whose sum is 0.

**Example:**

```text
Input:  [-1, 0, 1, 2, -1, -4]
Output: [[-1, -1, 2], [-1, 0, 1]]
```

**Solution:**

```js
function threeSum(nums) {
  nums.sort((a, b) => a - b);
  const res = [];
  for (let i = 0; i < nums.length - 2; i++) {
    if (i > 0 && nums[i] === nums[i - 1]) continue;
    let l = i + 1, r = nums.length - 1;
    while (l < r) {
      const sum = nums[i] + nums[l] + nums[r];
      if (sum === 0) {
        res.push([nums[i], nums[l], nums[r]]);
        while (l < r && nums[l] === nums[l + 1]) l++;
        while (l < r && nums[r] === nums[r - 1]) r--;
        l++;
        r--;
      } else if (sum < 0) {
        l++;
      } else {
        r--;
      }
    }
  }
  return res;
}
```

---

## Q65. Container With Most Water

height[i] is the height of a vertical line at position i. Pick two lines that, together with the x-axis, hold the most water. Return that amount.

**Example:**

```text
Input:  [1, 8, 6, 2, 5, 4, 8, 3, 7]
Output: 49
```

**Solution:**

```js
function maxArea(height) {
  let l = 0, r = height.length - 1, best = 0;
  while (l < r) {
    best = Math.max(best, Math.min(height[l], height[r]) * (r - l));
    if (height[l] < height[r]) l++;
    else r--;
  }
  return best;
}
```

---

## Q66. Subarray Sum Equals K

Count the number of continuous subarrays whose sum equals k.

**Example:**

```text
Input:  nums = [1, 2, 3], k = 3
Output: 2   ([1, 2] and [3])
```

**Solution:**

```js
function subarraySum(nums, k) {
  const prefixCount = new Map([[0, 1]]);
  let sum = 0, count = 0;
  for (const n of nums) {
    sum += n;
    count += prefixCount.get(sum - k) || 0;
    prefixCount.set(sum, (prefixCount.get(sum) || 0) + 1);
  }
  return count;
}
```

---

## Q67. Rotate Array

Rotate the array to the right by k steps, in place.

**Example:**

```text
Input:  nums = [1, 2, 3, 4, 5, 6, 7], k = 3
Output: [5, 6, 7, 1, 2, 3, 4]
```

**Solution:**

```js
function rotate(nums, k) {
  k %= nums.length;
  const reverse = (l, r) => {
    while (l < r) {
      [nums[l], nums[r]] = [nums[r], nums[l]];
      l++;
      r--;
    }
  };
  reverse(0, nums.length - 1);
  reverse(0, k - 1);
  reverse(k, nums.length - 1);
  return nums;
}
```

---

## Q68. Majority Element

Return the element that appears more than n / 2 times. It always exists.

**Example:**

```text
Input:  [2, 2, 1, 1, 1, 2, 2]
Output: 2
```

**Solution:**

```js
function majorityElement(nums) {
  let candidate = null, count = 0;
  for (const n of nums) {
    if (count === 0) candidate = n;
    count += n === candidate ? 1 : -1;
  }
  return candidate;
}
```

---

## Q69. Min Stack

Design a stack that supports these operations in O(1) time:

- `push(val)`: add an element
- `pop()`: remove the top element
- `top()`: return the top element
- `getMin()`: return the smallest element in the stack

**Example:**

```text
Input:  push(-2), push(0), push(-3), getMin(), pop(), top(), getMin()
Output: getMin() = -3, top() = 0, getMin() = -2
```

**Solution:**

```js
class MinStack {
  constructor() {
    this.stack = [];
    this.minStack = [];
  }
  push(val) {
    this.stack.push(val);
    const min = this.minStack.length ? Math.min(val, this.getMin()) : val;
    this.minStack.push(min);
  }
  pop() {
    this.stack.pop();
    this.minStack.pop();
  }
  top() {
    return this.stack[this.stack.length - 1];
  }
  getMin() {
    return this.minStack[this.minStack.length - 1];
  }
}
```

---

## Q70. Daily Temperatures

For each day, return how many days you have to wait for a warmer temperature. Use 0 if there is no warmer day later.

**Example:**

```text
Input:  [73, 74, 75, 71, 69, 72, 76, 73]
Output: [1, 1, 4, 2, 1, 1, 0, 0]
```

**Solution:**

```js
function dailyTemperatures(temps) {
  const res = new Array(temps.length).fill(0);
  const stack = [];
  for (let i = 0; i < temps.length; i++) {
    while (stack.length && temps[i] > temps[stack[stack.length - 1]]) {
      const prev = stack.pop();
      res[prev] = i - prev;
    }
    stack.push(i);
  }
  return res;
}
```

---

## Q71. Search in Rotated Sorted Array

A sorted array was rotated at some unknown point. Find the index of the target, or return -1. Must run in O(log n).

**Example:**

```text
Input:  nums = [4, 5, 6, 7, 0, 1, 2], target = 0
Output: 4
```

**Solution:**

```js
function searchRotated(nums, target) {
  let l = 0, r = nums.length - 1;
  while (l <= r) {
    const mid = Math.floor((l + r) / 2);
    if (nums[mid] === target) return mid;
    if (nums[l] <= nums[mid]) {
      if (target >= nums[l] && target < nums[mid]) r = mid - 1;
      else l = mid + 1;
    } else {
      if (target > nums[mid] && target <= nums[r]) l = mid + 1;
      else r = mid - 1;
    }
  }
  return -1;
}
```

---

## Q72. First and Last Position of an Element

In a sorted array, find the first and last index of the target. Return [-1, -1] if it is not present. Must run in O(log n).

**Example:**

```text
Input:  nums = [5, 7, 7, 8, 8, 10], target = 8
Output: [3, 4]
```

**Solution:**

```js
function searchRange(nums, target) {
  function findBound(isFirst) {
    let l = 0, r = nums.length - 1, ans = -1;
    while (l <= r) {
      const mid = Math.floor((l + r) / 2);
      if (nums[mid] === target) {
        ans = mid;
        if (isFirst) r = mid - 1;
        else l = mid + 1;
      } else if (nums[mid] < target) {
        l = mid + 1;
      } else {
        r = mid - 1;
      }
    }
    return ans;
  }
  return [findBound(true), findBound(false)];
}
```

---

## Q73. Insert Interval

Given sorted, non-overlapping intervals and a new interval, insert the new interval and merge any overlaps.

**Example:**

```text
Input:  intervals = [[1, 3], [6, 9]], newInterval = [2, 5]
Output: [[1, 5], [6, 9]]
```

**Solution:**

```js
function insertInterval(intervals, newInterval) {
  const res = [];
  let [start, end] = newInterval;
  let i = 0;
  while (i < intervals.length && intervals[i][1] < start) res.push(intervals[i++]);
  while (i < intervals.length && intervals[i][0] <= end) {
    start = Math.min(start, intervals[i][0]);
    end = Math.max(end, intervals[i][1]);
    i++;
  }
  res.push([start, end]);
  while (i < intervals.length) res.push(intervals[i++]);
  return res;
}
```

---

## Q74. Meeting Rooms

Given meeting time intervals [start, end], return true if one person can attend all meetings (no two meetings overlap).

**Example:**

```text
Input:  [[0, 30], [5, 10], [15, 20]]
Output: false
Input:  [[7, 10], [2, 4]]
Output: true
```

**Solution:**

```js
function canAttendMeetings(intervals) {
  intervals.sort((a, b) => a[0] - b[0]);
  for (let i = 1; i < intervals.length; i++) {
    if (intervals[i][0] < intervals[i - 1][1]) return false;
  }
  return true;
}
```

---

## Q75. Meeting Rooms II

Given meeting time intervals [start, end], return the minimum number of rooms needed so that all meetings can happen.

**Example:**

```text
Input:  [[0, 30], [5, 10], [15, 20]]
Output: 2
```

**Solution:**

```js
function minMeetingRooms(intervals) {
  const starts = intervals.map(i => i[0]).sort((a, b) => a - b);
  const ends = intervals.map(i => i[1]).sort((a, b) => a - b);
  let rooms = 0, maxRooms = 0, e = 0;
  for (let s = 0; s < starts.length; s++) {
    while (ends[e] <= starts[s]) {
      rooms--;
      e++;
    }
    rooms++;
    maxRooms = Math.max(maxRooms, rooms);
  }
  return maxRooms;
}
```

---

## Q76. Middle of the Linked List

Return the middle node of a linked list. If there are two middle nodes, return the second one.

**Example:**

```text
Input:  1 -> 2 -> 3 -> 4 -> 5
Output: node 3
Input:  1 -> 2 -> 3 -> 4 -> 5 -> 6
Output: node 4
```

**Solution:**

```js
function middleNode(head) {
  let slow = head, fast = head;
  while (fast && fast.next) {
    slow = slow.next;
    fast = fast.next.next;
  }
  return slow;
}
```

---

## Q77. Remove Nth Node From End of List

Remove the nth node from the end of the linked list and return the head.

**Example:**

```text
Input:  1 -> 2 -> 3 -> 4 -> 5, n = 2
Output: 1 -> 2 -> 3 -> 5
```

**Solution:**

```js
function removeNthFromEnd(head, n) {
  const dummy = new ListNode(0, head);
  let fast = dummy, slow = dummy;
  for (let i = 0; i < n; i++) fast = fast.next;
  while (fast.next) {
    fast = fast.next;
    slow = slow.next;
  }
  slow.next = slow.next.next;
  return dummy.next;
}
```

---

## Q78. Validate Binary Search Tree

Return true if the tree is a valid BST: every node in the left subtree is smaller than the node, and every node in the right subtree is larger.

**Example:**

```text
Input:      5
           / \
          1   4
             / \
            3   6
Output: false   (4 is in the right subtree of 5 but is smaller than 5)
```

**Solution:**

```js
function isValidBST(root, min = -Infinity, max = Infinity) {
  if (!root) return true;
  if (root.val <= min || root.val >= max) return false;
  return isValidBST(root.left, min, root.val) && isValidBST(root.right, root.val, max);
}
```

---

## Q79. Lowest Common Ancestor of a Binary Tree

Given two nodes p and q, return their lowest common ancestor: the deepest node that has both p and q in its subtree (a node can be its own ancestor).

**Example:**

```text
Input:        3
             / \
            5   1
           / \
          6   2
p = 5, q = 1  ->  Output: 3
p = 5, q = 2  ->  Output: 5
```

**Solution:**

```js
function lowestCommonAncestor(root, p, q) {
  if (!root || root === p || root === q) return root;
  const left = lowestCommonAncestor(root.left, p, q);
  const right = lowestCommonAncestor(root.right, p, q);
  if (left && right) return root;
  return left || right;
}
```

---

## Q80. Diameter of Binary Tree

Return the length (number of edges) of the longest path between any two nodes in the tree. The path does not have to pass through the root.

**Example:**

```text
Input:      1
           / \
          2   3
         / \
        4   5
Output: 3   (4 -> 2 -> 1 -> 3)
```

**Solution:**

```js
function diameterOfBinaryTree(root) {
  let best = 0;
  function height(node) {
    if (!node) return 0;
    const l = height(node.left);
    const r = height(node.right);
    best = Math.max(best, l + r);
    return 1 + Math.max(l, r);
  }
  height(root);
  return best;
}
```

---

## Q81. Min Heap

JavaScript has no built-in heap. Build a MinHeap class that takes an optional compare function and supports:

- `push(val)`: add a value in O(log n)
- `pop()`: remove and return the smallest value in O(log n)
- `peek()`: return the smallest value without removing it
- `size()`: return the number of values

**Example:**

```text
Input:  push(5), push(1), push(3), pop(), pop()
Output: 1, 3
```

**Solution:**

```js
class MinHeap {
  constructor(compare = (a, b) => a - b) {
    this.heap = [];
    this.compare = compare;
  }
  size() {
    return this.heap.length;
  }
  peek() {
    return this.heap[0];
  }
  push(val) {
    this.heap.push(val);
    let i = this.heap.length - 1;
    while (i > 0) {
      const parent = Math.floor((i - 1) / 2);
      if (this.compare(this.heap[i], this.heap[parent]) >= 0) break;
      [this.heap[i], this.heap[parent]] = [this.heap[parent], this.heap[i]];
      i = parent;
    }
  }
  pop() {
    if (this.heap.length === 0) return undefined;
    const top = this.heap[0];
    const last = this.heap.pop();
    if (this.heap.length > 0) {
      this.heap[0] = last;
      let i = 0;
      while (true) {
        const l = 2 * i + 1, r = 2 * i + 2;
        let smallest = i;
        if (l < this.heap.length && this.compare(this.heap[l], this.heap[smallest]) < 0) smallest = l;
        if (r < this.heap.length && this.compare(this.heap[r], this.heap[smallest]) < 0) smallest = r;
        if (smallest === i) break;
        [this.heap[i], this.heap[smallest]] = [this.heap[smallest], this.heap[i]];
        i = smallest;
      }
    }
    return top;
  }
}
```

---

## Q82. Kth Largest Element in an Array

Return the kth largest element in the array (not the kth distinct one).

**Example:**

```text
Input:  nums = [3, 2, 1, 5, 6, 4], k = 2
Output: 5
```

**Solution:**

```js
function findKthLargest(nums, k) {
  const heap = new MinHeap();
  for (const n of nums) {
    heap.push(n);
    if (heap.size() > k) heap.pop();
  }
  return heap.peek();
}
```

---

## Q83. Merge K Sorted Linked Lists

Given k sorted linked lists, merge them into one sorted linked list.

**Example:**

```text
Input:  [1 -> 4 -> 5, 1 -> 3 -> 4, 2 -> 6]
Output: 1 -> 1 -> 2 -> 3 -> 4 -> 4 -> 5 -> 6
```

**Solution:**

```js
function mergeKLists(lists) {
  const heap = new MinHeap((a, b) => a.val - b.val);
  for (const node of lists) if (node) heap.push(node);
  const dummy = new ListNode(0);
  let tail = dummy;
  while (heap.size()) {
    const node = heap.pop();
    tail.next = node;
    tail = node;
    if (node.next) heap.push(node.next);
  }
  return dummy.next;
}
```

---

## Q84. Graph BFS and DFS Traversal

Given a graph as an adjacency list and a start node, return the order in which nodes are visited using BFS (level by level) and DFS (go deep first).

**Example:**

```text
Input:  graph = { A: ["B", "C"], B: ["D"], C: ["E"], D: [], E: [] }, start = "A"
Output: BFS = ["A", "B", "C", "D", "E"]
        DFS = ["A", "B", "D", "C", "E"]
```

**Solution:**

```js
function bfs(graph, start) {
  const visited = new Set([start]);
  const queue = [start];
  const order = [];
  let head = 0;
  while (head < queue.length) {
    const node = queue[head++];
    order.push(node);
    for (const next of graph[node]) {
      if (!visited.has(next)) {
        visited.add(next);
        queue.push(next);
      }
    }
  }
  return order;
}

function dfs(graph, start, visited = new Set(), order = []) {
  visited.add(start);
  order.push(start);
  for (const next of graph[start]) {
    if (!visited.has(next)) dfs(graph, next, visited, order);
  }
  return order;
}
```

---

## Q85. Course Schedule (Topological Sort)

There are numCourses courses labeled 0 to numCourses - 1. prerequisites[i] = [a, b] means you must take course b before course a. Return true if you can finish all courses (there is no cycle).

**Example:**

```text
Input:  numCourses = 2, prerequisites = [[1, 0]]
Output: true
Input:  numCourses = 2, prerequisites = [[1, 0], [0, 1]]
Output: false
```

**Solution:**

```js
function canFinish(numCourses, prerequisites) {
  const graph = Array.from({ length: numCourses }, () => []);
  const inDegree = new Array(numCourses).fill(0);
  for (const [course, pre] of prerequisites) {
    graph[pre].push(course);
    inDegree[course]++;
  }
  const queue = [];
  for (let i = 0; i < numCourses; i++) if (inDegree[i] === 0) queue.push(i);
  let taken = 0, head = 0;
  while (head < queue.length) {
    const node = queue[head++];
    taken++;
    for (const next of graph[node]) {
      inDegree[next]--;
      if (inDegree[next] === 0) queue.push(next);
    }
  }
  return taken === numCourses;
}
```

---

## Q86. Rotting Oranges

In a grid, 0 = empty, 1 = fresh orange, 2 = rotten orange. Every minute, fresh oranges next to a rotten one (up/down/left/right) become rotten. Return the minutes until no fresh orange is left, or -1 if impossible.

**Example:**

```text
Input:  [[2, 1, 1],
         [1, 1, 0],
         [0, 1, 1]]
Output: 4
```

**Solution:**

```js
function orangesRotting(grid) {
  const rows = grid.length, cols = grid[0].length;
  let queue = [];
  let fresh = 0;
  for (let r = 0; r < rows; r++) {
    for (let c = 0; c < cols; c++) {
      if (grid[r][c] === 2) queue.push([r, c]);
      if (grid[r][c] === 1) fresh++;
    }
  }
  let minutes = 0;
  const dirs = [[1, 0], [-1, 0], [0, 1], [0, -1]];
  while (queue.length && fresh > 0) {
    const next = [];
    for (const [r, c] of queue) {
      for (const [dr, dc] of dirs) {
        const nr = r + dr, nc = c + dc;
        if (nr >= 0 && nc >= 0 && nr < rows && nc < cols && grid[nr][nc] === 1) {
          grid[nr][nc] = 2;
          fresh--;
          next.push([nr, nc]);
        }
      }
    }
    queue = next;
    minutes++;
  }
  return fresh === 0 ? minutes : -1;
}
```

---

## Q87. Subsets

Return all possible subsets of an array of unique numbers.

**Example:**

```text
Input:  [1, 2, 3]
Output: [[], [1], [1, 2], [1, 2, 3], [1, 3], [2], [2, 3], [3]]
```

**Solution:**

```js
function subsets(nums) {
  const res = [];
  function backtrack(start, path) {
    res.push([...path]);
    for (let i = start; i < nums.length; i++) {
      path.push(nums[i]);
      backtrack(i + 1, path);
      path.pop();
    }
  }
  backtrack(0, []);
  return res;
}
```

---

## Q88. Permutations

Return all possible orderings of an array of unique numbers.

**Example:**

```text
Input:  [1, 2, 3]
Output: [[1, 2, 3], [1, 3, 2], [2, 1, 3], [2, 3, 1], [3, 1, 2], [3, 2, 1]]
```

**Solution:**

```js
function permute(nums) {
  const res = [];
  const used = new Array(nums.length).fill(false);
  function backtrack(path) {
    if (path.length === nums.length) {
      res.push([...path]);
      return;
    }
    for (let i = 0; i < nums.length; i++) {
      if (used[i]) continue;
      used[i] = true;
      path.push(nums[i]);
      backtrack(path);
      path.pop();
      used[i] = false;
    }
  }
  backtrack([]);
  return res;
}
```

---

## Q89. Combination Sum

Given unique positive numbers and a target, return all unique combinations that add up to the target. The same number can be used any number of times.

**Example:**

```text
Input:  candidates = [2, 3, 6, 7], target = 7
Output: [[2, 2, 3], [7]]
```

**Solution:**

```js
function combinationSum(candidates, target) {
  const res = [];
  function backtrack(start, path, remaining) {
    if (remaining === 0) {
      res.push([...path]);
      return;
    }
    for (let i = start; i < candidates.length; i++) {
      if (candidates[i] > remaining) continue;
      path.push(candidates[i]);
      backtrack(i, path, remaining - candidates[i]);
      path.pop();
    }
  }
  backtrack(0, [], target);
  return res;
}
```

---

## Q90. House Robber

Each house has some money. You cannot rob two houses next to each other. Return the maximum money you can rob.

**Example:**

```text
Input:  [2, 7, 9, 3, 1]
Output: 12   (2 + 9 + 1)
```

**Solution:**

```js
function rob(nums) {
  let prev = 0, cur = 0;
  for (const n of nums) {
    [prev, cur] = [cur, Math.max(cur, prev + n)];
  }
  return cur;
}
```

---

## Q91. Coin Change

Given coin values and an amount, return the fewest coins needed to make that amount. Each coin can be used any number of times. Return -1 if the amount cannot be made.

**Example:**

```text
Input:  coins = [1, 2, 5], amount = 11
Output: 3   (5 + 5 + 1)
Input:  coins = [2], amount = 3
Output: -1
```

**Solution:**

```js
function coinChange(coins, amount) {
  const dp = new Array(amount + 1).fill(Infinity);
  dp[0] = 0;
  for (let a = 1; a <= amount; a++) {
    for (const coin of coins) {
      if (coin <= a) dp[a] = Math.min(dp[a], dp[a - coin] + 1);
    }
  }
  return dp[amount] === Infinity ? -1 : dp[amount];
}
```

---

## Q92. Longest Common Subsequence

Return the length of the longest sequence of characters that appears in both strings in the same order (not necessarily next to each other).

**Example:**

```text
Input:  text1 = "abcde", text2 = "ace"
Output: 3   ("ace")
```

**Solution:**

```js
function longestCommonSubsequence(text1, text2) {
  const m = text1.length, n = text2.length;
  const dp = Array.from({ length: m + 1 }, () => new Array(n + 1).fill(0));
  for (let i = 1; i <= m; i++) {
    for (let j = 1; j <= n; j++) {
      if (text1[i - 1] === text2[j - 1]) dp[i][j] = dp[i - 1][j - 1] + 1;
      else dp[i][j] = Math.max(dp[i - 1][j], dp[i][j - 1]);
    }
  }
  return dp[m][n];
}
```
