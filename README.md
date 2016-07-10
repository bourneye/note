# note
参考手册
    语法 核心语义
标准类库
    内置对象 内置函数 模板

高级数据结构 面向对象
interpreter 解释器
concepts 概念
glossary 术语
semantics 语义
Tk 图形接口工具集
解释型语言开发速度快

语法
数据结构
表达式
数据类型
    数值
        + - * / ** %
        // 除，去小数点后值
        _ 上一命令的输出结果
        输入类型转换  int(raw_input('birth: '))

    字符串
        原始字符串   r'string'
        输出多行 """...""" or '''...'''
        串联  'string1'+'string2'  ('string1'
                                    'string2')
        重复次数    num'string'
        空格自动串联  'string1' 'sting2'
        字符串索引   a='string1' a[1] a[-1]
        统一编码字符串 unicode string
            >>> u'Hello\u0020World !'
            u'Hello World !'
        转换为list
            listname.split('')

    列表 list [ ] 链表
        有序集合
        insert append pop
        元素为string，转换string
            ','.join(listname)
        元素为int，转换string
            while n < len(l):
        列表生成式List Comprehensions
             [i for i in range(1,11)  if i % 2 == 0]


    元组 tuple ( )
        速度快，指向不变（写保护）
        只有1个元素的tuple定义时必须加一个逗号,，来消除歧义
    字典 dict { } 数组
        HashMap，Key-Value键值对
        查找速度快 无序  内存占用大
    集合 set [ ]
        不可重复

语句
    流程控制
        if
        for
        break continue pass
        function def

面向对象
    类
        实例化
    函数
        递归函数   一个函数在内部调用自身本身
        尾递归函数 解决递归调用栈溢出
        函数名可以为变量    f=abs; f(-10)
        高阶函数 把函数作为参数传入，函数式编程就是指这种高度抽象的编程范式。
            def add(x, y, f): return f(x) + f(y)
            add(-5, 6, abs)
    模块
        每一个py文件
异常处理
自定义类

        切片（Slice）操作符 range(100) [1::2]奇数
        迭代（Iteration） for循环
            判断是否为可迭代对象
                from collections import Iterable
                isinstance(something,, Iterable)
            字符串str  for i in 'abc'
            列表list   实现下标循环，形成索引-元素对，迭代索引和元素本身
            字典dict   无序排列，迭代出的结果顺序不一样。
                        迭代key       默认
                        迭代value     for value in d.itervalues()
                        迭代key-value for k, v in d.iteritems()
            多变量     for x, y in [(1, 1), (2, 4), (3, 9)]:





