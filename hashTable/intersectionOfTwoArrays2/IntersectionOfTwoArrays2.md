## 350. Intersection of Two Arrays II
计算数组的交集 每个数组中元素可重复 交集中也应重复
1. 哈希表
先迭代第一个数组，记录每一个元素的出现次数
迭代第二个数组，对于每一个元素，如果在哈希表中次数大于0，加入结果，并将
哈希表中映射-1.
时间复杂度O(N)
2. sort
两个数组排序，two pointers。
时间复杂度O(NlogN)

