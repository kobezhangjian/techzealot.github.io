---
title: (11) go面向对象-包和封装
date: 2020-05-10 23:19:01
tags: [go]
---

本章主要介绍go语言的包和封装

<!--more-->

### 封装

1. 名字一般使用CamelCase
2. 首字母大写表示public（包外可见）
3. 首字母小写表示private（包内可见）

### 包

1. 每个目录下只能有一个包（一个包可分散在多个文件），包名不必与目录名相关
2. main包包含可执行入口，main函数不在main包不能运行,不同目录下的main包成员不能互相访问
3. 为结构定义的方法必须放在同一个包内，但可以是不同的文件（方便协作开发）

### 工程化组织

将每个含有main函数的文件分散在不同的目录中，通常包名与文件名相同

> 可参考golang.org/x/tools/cmd