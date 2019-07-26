## 458. Poor Pigs
这题很有意思 主要考察进制 和信息量的承载
有n个buckets，只有一个有毒药。
每只猪喝完冷却时间为t, 喝完死的时间也为t
求给定一段时间t1, 在这段时间内测出毒药所需要的猪的数量

我们首先看一头猪能够测几瓶，一头猪能够喝t1/t瓶，剩下一瓶自然就检测出了。
所以一头猪可以检测t1/t瓶。
那么两头猪其实可以检测t1/t的二次方瓶，这里用二维阵列不难看出。
然后推广到高维空间也成立。
所以我们的公式是pow(t1/t+1, pigNum) >= n即可
