## 27. Remove Element

1. 两个指针，都初始化为0.快的指针遍历数组，发现不等于val的元素就复制到慢指针处，慢指针+1
缺点：每个元素都要复制一次
2. 碰到等于val的元素，就把数组最后一个元素赋值到这个位置，不用担心最后一个元素是val,我们会再检查。
如果val元素比较少，这种方法需要赋值的次数很少，可以。