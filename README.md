# easy_New-boom

## 提交链接 / Submit 
http://www.atomagic.cn:8080/problem/8

(You need register/login first before submit.)

（在提交前你需要先注册或登录）

## 题目描述 / Description

按顺序给你 N 个盒子,每个盒子包括两个球,每个球有颜色,颜色相同的算同一种球.

把盒子按顺序装到时钟塔里,如果这个地方里的盒子存在这样一种组合,盒子数等于这些盒子含有的球的种类数, 时钟塔就会爆炸.

## 输入 / Input

The first line is an integer N.

第一行只有一个整数 N

The next N lines include two integers a_i, b_i (1 ≤ i ≤ N) which represent the balls' colors in i_th box. 

接下来 N 行各包括两个整数 a_i,b_i 分别代表第 i 个盒子里两个球的颜色

数据保证

N ≤ 10^5

a_i, b_i < 10^5

## 输出 / Output

If the Clock Tower will boom, Output an integer Output "no" in otherwise

如果时钟塔会爆炸,输出爆炸时的箱子编号,否则输出" no "

## 样例 / Example

### input1

4

2 1

2 3

2 1

2 1

### output1

3

### 样例解释

4 

2 1  (A)

2 3  (B)

2 1  (C)

2 1  (D)

装入第一个盒子A后 存在盒子的组合只有{A}  盒子数和种类数 只可能是 1 2

装入第二个盒子B后 存在的盒子组合可以是{A},{B},{A,B}  盒子数和种类数 只可能是 2 3 ({A,B})  和 1 2 ({A}或{B})

装入第三个盒子C后 盒子数和种类数 可能是 3 3 ({A,B,C})    和 2 2  ({A,C}) 和 2 3 ({A,B} 或 {B,C}) 和 1 2   ({A}或{B}或{C})

本题所说的组合是指 已经在塔内的盒子的子集,显然有(2^n)-1种

## 答案 / Solutions


[Cpp](https://github.com/SIST-Manual/easy_New-boom/blob/master/solve.cpp)
