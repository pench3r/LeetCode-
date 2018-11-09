#### 题目描述 ####

写出一个程序，接受一个十六进制的数值字符串，输出该数值的十进制字符串。（多组同时输入 ）

input:
> 0xa

output:
> 10

#### 思路 ####

个人思路: 直接使用`cin>>hex>>`接收十六进制的数据,然后输出

优化思路: 手写十六进制的转换,主要通过从个位数开始遍历,解析`0-9,A-F`字符为数字乘以对应的pow16,并将其结果进行累加

#### 知识点 ####

- 对于字符数字的转换可以直接`-48`转换,也可以通过`-'0'`进行转换
- 对于`A-F`的转换可以直接`-55`进行转换对应的`10-15`