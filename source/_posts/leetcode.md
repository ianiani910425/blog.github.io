title: leetcode
author: John Doe
date: 2024-01-17 18:54:59
tags:
---
#### 基本C++語法

1. 動態陣列 vector 
```
n = 7,m=8 	//int
nums 		//陣列
```

```cpp
  #include<vector>

  vector<int> nums(n);       
  vector<int> nums(m, 2); 

  vector<int> nums{ 1,3,5 };

  vector<vector<int>> dp;		//二維陣列

  vector<vector<bool>> dp(m, vector<bool>(n, true));

  nums.empty()		//是否空值
  nums.size()		//大小


  nums.push_back(n)		//加入
  nums.back();			//查看最後一個
  nums.pop_back(m)		//刪除
```
<mark>從中間或頭部增刪元素會涉及搬移資料，效率會較低，使用演算法以避免此類操作</mark>

2.字串 string
```
s 		//字串
```

```cpp
#include<string>

s.push_back('n')
s += "abc"

s.substr(<mark>誰開始</mark>,<mark>後面要幾個</mark>)
```
		




