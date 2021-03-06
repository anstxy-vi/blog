---
title: Javascript - 按位取反运算符 ~
description: 通过转换为二进制原码再进行若干步骤（取反、反码、补码）得到目标值
toc: true
#authors:
#  - Hypocriticalr
tags:
  - 位
  - 计算
  - javascript
date: '2021-12-30'
lastmod: '2021-12-30'
draft: false
---
# 开始

> 阅读前，需了解二进制取反、反码、补码知识

## 正整数

> 因数字较小，统一转换为8位的二进制数据

### 处理步骤

1、转换为8位二进制

2、取反

3、反码

4、补码

5、将补码后的数据转换为十进制

如对 5 该数字进行 按位取反运算，即 ~5

- 转换为二进制
```javascript
0 0 0 0 0 1 0 1
```
- 取反
```javascript
1 1 1 1 1 0 1 0
```
- 反码
```javascript
1 0 0 0 0 1 0 1
```
- 补码
```javascript
1 0 0 0 0 1 1 0
```
结果: -6


## 负整数

> 因数字较小，统一转换为8位的二进制数据

### 处理步骤

1、转换为8位二进制

2、反码

3、补码

4、取反

5、将取反后的数据转换为十进制

如对 -8 该数字进行 按位取反运算，即 ~-8

- 转换为二进制
```javascript
1 0 0 0 1 0 0 0
```
- 反码
```javascript
1 1 1 1 0 1 1 1
```
- 补码
```javascript
1 1 1 1 1 0 0 0
```
- 取反
```javascript
0 0 0 0 0 1 1 1
```
结果: 7