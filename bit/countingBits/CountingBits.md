## 338. Counting Bits
直接求解很容易

要求用O(N)的复杂度one pass
找规律
比如8|1000 = 4|100 + 8&1(看最后一位是不是1)

19|10011 = 9|1001 + 19&1

可知 F[i] = F[i/2] + F[i]&1;
