## 172. Factorial Trailing Zeroes
要求是LogN的复杂度，自然就不能用常规做法，并且阶乘也是很容易溢出的。

思考过后，我们发现因为是连乘，所以其实2*5=10就会给结果添加一个0。
再然后发现其实2是远远多于5的，绝对够用。
所以我们只需要count 5的乘数的个数。

首先
101 = 101*100...*11*10*9*8*7*6*5*4*3*2*1

101/5其实就可以得到有多少个5，每隔5个数会产生一个5的倍数
比如11/5可以得到2个5的倍数，10和5

但是考虑25，会有两个5，所以我们要计算n/5 + n/25 + n/125 + ....才是最后5的个数
