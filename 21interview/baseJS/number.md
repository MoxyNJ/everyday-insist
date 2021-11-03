## number能表示的整数的最大范围
1. 安全的整数范围：15位数以下

2. JavaScript 并不能表示任意位的整数，最大的整数是Number.MAX_SAFE_INTEGER(9007199254740991)，最小的整数是Number.MIN_SAFE_INTEGER(-9007199254740991)

3. 特别注意，很多ID是超出这个范围的，所以ID最好是用string，当ID超出**15**位数的话，就肯定要用字符串类型了。

4. 超出会失准
```js
var a = 9007199254740995
a; // 9007199254740996
```
