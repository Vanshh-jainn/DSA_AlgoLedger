# 231. Power of Two

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-brightgreen) ![Topic](https://img.shields.io/badge/Topic-Math-blue) ![Topic](https://img.shields.io/badge/Topic-Bit_Manipulation-blue) ![Topic](https://img.shields.io/badge/Topic-Recursion-blue) ![Language](https://img.shields.io/badge/Language-cpp-orange)

## Metadata

| Field | Value |
| --- | --- |
| Runtime | 0 ms |
| Memory | 7.9 MB |
| Submission Date | 2026-10-24T14:14:42.716Z |
| Platform | leetcode |

## Problem Statement

<p>Given an integer <code>n</code>, return <em><code>true</code> if it is a power of two. Otherwise, return <code>false</code></em>.</p>

<p>An integer <code>n</code> is a power of two, if there exists an integer <code>x</code> such that <code>n == 2<sup>x</sup></code>.</p>

<p>&nbsp;</p>
<p>

## Examples

**Example 1:**

```
</p>

<pre>
<strong>Input:</strong> n = 1
<strong>Output:</strong> true
<strong>Explanation: </strong>2<sup>0</sup> = 1
</pre>

<p>
```

**Example 2:**

```
</p>

<pre>
<strong>Input:</strong> n = 16
<strong>Output:</strong> true
<strong>Explanation: </strong>2<sup>4</sup> = 16
</pre>

<p>
```

**Example 3:**

```
</p>

<pre>
<strong>Input:</strong> n = 3
<strong>Output:</strong> false
</pre>

<p>&nbsp;</p>
```

## Constraints

- <code>-2<sup>31</sup> &lt;= n &lt;= 2<sup>31</sup> - 1</code>

## Solution

```cpp
class Solution {
public:
    bool isPowerOfTwo(int n) {
        if(n<1)
        return 0;
        

        while(n!=1){
            if(n%2==1)
            return 0;
            
            n = n/2;
        } return 1;
    }
};
```

[View on LeetCode](https://leetcode.com/problems/power-of-two/)
