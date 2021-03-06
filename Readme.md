# **Specifying Systems**

**The TLA+ Language and Tools for**
**Hardware and Software Engineers**
**Leslie Lamport**
**Microsoft Research**

# 目录

## 第一部分 如何开始

### 简单的数学

1. 定理逻辑
2. 集合
3. 谓词逻辑
4. 公式与语言

### 定义一个简单的时钟

1. 行为
2. 钟表
3. 仔细看看说明书
4. 在TLA+中的规范
5. 另一种规范

### 异步接口

1. 第一次的规范
2. 另一个规范
3. 类型提示
4. 定义
5. 评论

### 先入先出队列

1. 内部规范
2. 实例化检查
3. 可替代的实例化
4. 参数实例化
5. 隐式替换
6. 实例化,不重命名
7. 隐藏队列
8. 有界的先入先出队列
9. 我们指定的是什么?

### 缓存内存

1. 内存接口
2. 函数
3. 线性内存
4. 元组作为函数
5. 递归函数
6. 连续写入缓存
7. 不可变性
8. 证明实现

### 更多一点数学

1. 集合
2. 简单的表达式
3. 重新审视递归
4. 函数与操作符
5. 使用函数
6. 选择

### 关于写一份规范的一些建议

1. 为什么需要规范
2. 什么是规范
3. 原子的粒度
4. 数据结构
5. 编写规范
6. 一些进一步的提示
7. 什么时候和怎样规范?

## 第二部分 更多高级主题

### 活性与公平

1. 时序公式
2. 时序等式
3. 时态证明规则
4. 弱公平
5. 内存规范
6. 活性的要求
7. 另一种写法
8. 推广
9. 强公平
10. 连续写入缓存
11. 定量
12. 时态逻辑检验
13. 回顾
14. 机器闭包和可能性
15. 重新映射和公平
16. 不重要的活性
17. 时序逻辑被认为是混乱的

### 实时

1. 重新审视时钟
2. 一般的实时规范
3. 实时缓存内存
4. Zeno规范
5. 混合系统规范
6. 实时系统上的备注

### 组合规范

1. #### 组合两种规范

2. #### 组合多种规范

3. #### 先进先出队列

4. #### 与共享状态组合

   4.1精确的状态变化

   4.2与Joint Actions组合

5. #### 简要回顾

   5.1结构的构造

   5.2来回再考虑

   5.3再考虑Joint Actions

6. #### 活性与隐藏

   6.1活性与机器闭包

   6.2隐藏

7. #### 开发系统规范

8. #### 接口提取

   8.1二进制时钟

   8.2提取通道

   8.3一般地接口提取

   8.4开放接口规范

9. #### 你应该怎么组合?



### 高级例子

1. 规范数据结构
2. 本地定义
3. 图
4. BNF语法
5. 其他内存规范
6. 接口
7. 关于正确条件
8. 顺序一致的内存
9. 考虑内存问题



## 第三部分 工具

## 12.语义分析器

### 13 TLATEX  排版助手

1. 介绍

2. 屏蔽注释

3. 怎样排版规范

4. 怎样排版注释

5. 调整输出格式

6. 输出文件

7. 故障排除

8. 使用 LATEX 命令


### TLC模型检查器

#### 介绍TLC

#### 可以使用TCL处理什么

1. TLC的值

2. TLC怎么执行表达式

3. 赋值和代换

4. 执行时序公式

5. 重写模块

6. TLC怎样计算状态


#### TLC怎样检查属性

1. 模型检查模式

2. 仿真模式

3. 视图与指纹

4. 利用对称性的优势

5. 活性检查的局限性


#### TLC模块

#### 怎样使用TLC运行

1. 运行TLC
2. TLC调试规范

3. 有效地使用TLC的注解


#### TLC不能做什么

#### 良好的打印

1. 配置文件的语法

2. 可比较的TLC的值




## 第四部分 TLA+语言

迷你手册

### TLA+语法

#### 简单的语法

#### 完备的语法

1. 优先级与结合律

2. 对齐

3. 注释

4. 时序公式

5. 两个异常


#### TLA+的Lexemes

### TLA+的操作符

#### 常量操作符

1. 布尔操作符

2. 选择操作符

3. 布尔操作符的解释

4. 条件的构造

5. Let/In 的构造

6. 集合论的操作符

7. 函数

8. 记录

9. 元组

10. 字符串

11. 数字


### 非常量表达式

1. 基本常量表达式

2. 状态函数的意义

3. action操作符

4. 时序操作符


#### 模块的意义

#### 操作符与表达式

1. 数量与操作符的顺序
2. lamdba表达式
3. 简化操作符应用
4. 表达式

#### 等级

#### 上下文

#### lamdba表达式的意义

#### 模块的意义

1. 继承
2. 生命
3. 操作符的定义
4. 函数的定义
5. 实例化
6. 定理和假设
7. 子模块

#### 模块的正确性

#### 发现模块

#### 实例化的意义

### 标准模块

#### Sequences模块

#### FiniteSets模块

#### Bags模块

#### Numbers模块



## 问题的列表和表格

### 问题

1. 时钟的标准--类型集合和ASCII的版本
2. 我们第一个异步接口的规范
3. 我们第二个异步接口的规范
4. 带有注释的时钟规范
5. 带有内部可见变量q的FIFO的规范
6. 长度为N的FIFO缓冲区的规范
7. 内存接口的规范
8. 内部内存规范
9. 内存规范
10. 直写模式缓存
11. 直写模式缓存的规范
12. 时钟的实时规范
13. 针对写入的实时规范的实时模块
14. 线性内存规范的实时版本
15. 直写模式缓存的实时版本
16. 一种非交错组合的FIFO组合
17. 一种joint-action规范的线性内存
18. 一种二进制时钟的规范
19. 关注一个通道
20. 针对定制图操作的模块
21. 针对解决等价公式的模块
22. BNF语法的模块
23. 对内存定制一个寄存器接口的模块
24. InnerSerial模块
25. InnerSequential模块
26. 交换位协议
27. MCAlternatingBit模块
28. MCAlternatingBit模块的配置文件
29. 比特交换协议的正确性规范
30. TLC模块的规范
31. BNF语法的配置文件
32. Sequences模块的配置文件
33. standard Sequences模块
34. standard FiniteSets模块
35. standard Bags模块
36. Peano模块
37. ProtoReals模块
38. standard Naturals 模块
39. standard Integers 模块
40. standard Reals 模块
41. Peano模块
42. standard Reals模块



### 表格:

表格1 常量运算符

表格2 混杂的构造

表格3 Action操作符

表格4 时序操作符

表格5 用户定义操作符

表格6操作符的优先级范围

表格7在标准模块中操作符的定义

表格8类型集合符号的Ascii码的表示











