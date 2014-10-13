# The Orange Juice ACM-ICPC Cheat Sheet

## Basic

### C++ Solution Template

```c++
#include <iostream>
#include <string>
#include <cstring>
#include <algorithm>
#include <climits>
#include <stack>
#include <queue>
#include <vector>
#include <set>
#include <map>

/*
 * n: number
 * i: LSB starting from 1
 */
#define SET_BIT(n, i) ((n) | (1 << ((i)-1)))
#define CLR_BIT(n, i) ((n) & ~(1 << ((i)-1)))
#define GET_BIT(n, i) (((n) & (1 << ((i)-1))) >> ((i)-1))
#define SHOW(x) {cout << #x << " = " << x << endl;}
const double E = 1e-8;
const double PI = acos(-1);

using namespace std;

int main() {
    ios::sync_with_stdio(false);
    /*
     * Main program.
     */
    return 0;
}
```

### C++ String

#### Input string

* get one string with no space and new-line.

```c++
string a;
cin >> a;
cout << "[C++] You have input \"" << a << "\", "
     << ", whose length is " << a.length() << endl;
```

Input
```
hello world
new line
```

Output
```
[C++] You have input "hello", , whose length is 5
```

#### read one line

* get one line

```c++
string a;
getline(cin, a);
cout << a << endl;
```

Input
```
Hello World!!!
```

Output
```
Hello World!!!
```


#### Convert to char array

```c++
string cppstr = "this is a string";
char target[1024];
strcpy(target, cppstr.c_str());
```


### C String (Character Array)

#### Input C String

* gets

Reads characters from the standard input (stdin) and stores them as a C string into str until a newline character or the end-of-file is reached.

```c++
char b[10];
gets(b);
cout << "[C++] You have input \"" << b << "\", "
     << ", whose length is " << strlen(b) << endl;
```

Input
```
 world
new line
```

Output
```
[C] You have input " world", , whose length is 6
```

Note: There is a space in front of "world", which will be part of the string.

However, using gets() is "unsafe", but we are not to discuss the details here.

#### Convert to C++ string
char arrstr[] = "this is a string";
string target = string(arr);



### Standard Template Library

##### ``include <algorithm>``

####### ``next_permutation / pre_permutation``

####### ``binary_search``

####### ``swap / iter_swap``

####### ``make_heap / pop heap / push heap / sort_heap``

####### ``sort / stable_sort``



##### ``include <map>``

##### ``include <priority_queue>``

##### ``include <queue>``

##### ``include <stack>``

##### ``string``

##### ``T::iterator``

##### ``include <vector>``

##### ``pair<, >``



### Java BigInteger & BigDecimal




### String Related

##### KMP




### Tree Related

##### Tree Traversal

##### Trie

##### Segment Tree

##### Union-find Set 冰茶鸡

##### 。。。




### Graph Theory

##### Minimium Spanning Tree

####### Prime

####### Kruskal


##### Shortest Path

####### 任意两点

####### SPFA

####### Dijkstra


##### 二分图

##### 最大流
 
##### 最小费用最大流 ?

##### 强连通分量 图的 割点, 桥, 双连通分支

##### 拓扑排序

##### Euler Cycle/Path, Hamilton Cycle/Path

##### 。。。




### Math

##### 。。。




### 计算几何

##### 向量点乘 叉乘

##### 直线公式

##### Convex Hull



### Tricks / 分析方法

##### Dynamic Programming

##### Divide and Conquer

##### 双向 BFS

##### Brute Force

####### 子集生成