## 448. Find All Numbers Disappeared in an Array

这题跟之前哪一题是一样的

1. 可以用set判断已经有的元素 空间O(N) 时间O(N)

2. 不停地去替换 将值与下标对比 将元素替换到正确的位置 最后再扫描一遍即可 空间O(1) 时间O(N)
就是利用元素的值是从1到N的特性

评论区有个标记为负的 实际原理和效率是一样的 个人觉得不是很好 过度了