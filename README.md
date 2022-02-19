# 目标
用于记录做动态规划这部分的算法题的心得。
什么是动态规划
动态规划，英⽂：Dynamic Programming，简称DP，如果某⼀问题有很多重叠⼦问题，使⽤动态规划
是最有效的。
所以动态规划中每⼀个状态⼀定是由上⼀个状态推导出来的，这⼀点就区分于贪⼼，贪⼼没有状态推
导，⽽是从局部直接选最优的，例如：有N件物品和⼀个最多能背重量为W 的背包。第i件物品的重量是weight[i]，得到的价值是value[i]
。每件物品只能⽤⼀次，求解将哪些物品装⼊背包⾥物品价值总和最⼤。
动态规划中dp[j]是由dp[j-weight[i]]推导出来的，然后取max(dp[j], dp[j - weight[i]] + value[i])。
但如果是贪⼼呢，每次拿物品选⼀个最⼤的或者最⼩的就完事了，和上⼀个状态没有关系。
所以贪⼼解决不了动态规划的问题。

## 动态规划的解题步骤：
状态转移公式（递推公式）是很重要，但动规不仅仅只有递推公式。
对于动态规划问题，我将拆解为如下五步曲，这五步都搞清楚了，才能说把动态规划真的掌握了！
1. 确定dp数组（dp table）以及下标的含义
2. 确定递推公式
3. dp数组如何初始化
4. 确定遍历顺序
5. 举例推导dp数组

## 动态规划应该如何debug：
找问题的最好⽅式就是把dp数组打印出来，看看究竟是不是按照⾃⼰思路推导的！


