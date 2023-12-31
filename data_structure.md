# 基本概念
> 数据

> 数据类型

> 数据元素

> 数据对象

> 数据项

> 数据结构

> 数据结构三要素：逻辑结构，存储结构，数据的运算




# 线性表

## 线性表的类型定义
> 定义：具有相同数据类型的n个数据元素的**有限**序列

> 基本操作：

## 线性表的顺序表示
> 用一组地址**连续**的存储单元依次存储线性表的数据结构（逻辑上相邻，物理上也相邻）

> 静态分配&动态分配：静态分配空间固定；动态分配允许申请更大的空间，拷贝原来的数据到新的空间

> 特点：随机访问、存储密度高、逻辑上相邻物理上也相邻，插入删除移动大量数据元素

### 时间复杂度
1. 插入 O(n)
1. 删除 O(n)
1. LocateElem 按值查找(顺序查找) O(n)
1. GetElem O(1)

## 线性表的链式表示
> 实现方式：不带头结点（空表判断L == NULL），代码书写不方便、带头结点（L->next == NULL），代码书写方便（相当于链表至少有一个元素，删除结点、插入结点时不用考虑首元结）

> 特点：插入删除不需要移动数据元素，只需要修改指针；不能随机存取，只能从表头遍历；浪费了一定空间；

### 线性链表（单链表）
> 用一组**任意的**（可以连续也可以不连续）存储单元存储线性表的数据元素（逻辑上相邻，物理上不一定相邻）

> 结点 数据域+指针域

> 头指针：指示链表中第一个结点（第一个数据元素的存储映像）的存储位置。链表的存取从**头指针**开始

> 头结点：单链表第一个结点之前附设的结点，好处：简化代码TODO

> 首元结点：第一个数据元素，单链表第一个结点

#### 基本操作
1. 建立操作：头插法、尾插法
1. LocateElem 按值查找(顺序查找) O(n)
1. GetElem O(n)
1. 插入 若给定了结点指针，O(1)；若给定的是index，由于需要用GetElem获得指针，则为o(n)
1. 删除 同插入（还需要free）


### 静态链表
TODO

### 循环链表
> 特点：表中最后一个结点的指针域指向头结点，整个链表形成一个环
> 仅设置尾指针，不设置头指针能使两个线性表合并时间为O(1)

### 双向链表
> 克服了寻找PriorElem结点为O(n)的缺点

#### 基本操作
1. 插入
1. 删除

## 从时间、空间复杂度的角度比较线性表两种存储结构的不同特点及其适用场合 TODO
1. 时间：顺序表随机访问，
1. 空间：

---
1. 存取（读写）方式：顺序表可以顺序存取&随机存取
1. 逻辑结构&物理结构：顺序表逻辑上连续物理上也连续
1. 插入、删除：顺序表移动元素O(n);链表只需修改指针（给定指针的情况）
1. 按值查找：顺序表有序时可以折半查找O(logn)，无序时O(n)
1. 按序号查找：顺序表可以随机访问O(1)
1. 存储结构：顺序表连续分配，静态分配&动态分配（拷贝）；

##  一元多项式的表示及相加


# 栈和队列

## 栈
> 定义：栈是限定仅在表尾进行插入或者删操作的线性表。
> 栈顶：表尾端；栈底：表头端
> 特点：后进先出（LIFO）

## 栈与递归实现（递归算法中栈的作用）

## 栈的应用举例
1. 数制转换
1. 括号匹配的检验
1. 行编辑程序
1. 迷宫求解
1. 表达式求值




