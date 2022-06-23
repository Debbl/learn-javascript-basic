# 原始类型的包装类

- JavaScript的原始类型并非对象类型，所以从理论上来说，它们是没有办法获取属性或者调用方法的。

- 那么，为什么会出现这样奇怪的现象呢？（悖论）
    - 原始类型是简单的值，默认并不能调用属性和方法；
    - 这是因为JavaScript为了可以使其可以获取属性和调用方法，对其封装了对应的包装类型；

- 常见的包装类型有：String、Number、Boolean、Symbol、BigInt类型；

# 包装类型的使用过程

- 默认情况，当我们调用一个原始类型的属性或者方法时，会进行如下操作：
    - 根据原始值，**创建一个原始类型对应的包装类型对象**；
    - 调用对应的属性或者方法，返回一个新的值；
    - **创建的包装类对象被销毁**；
    - 通常JavaScript引擎会进行很多的优化，它可以跳过创建包装类的过程在内部直接完成属性的获取或者方法的调用

# Number
- 类属性
    - .length
    - .MAX_VALUE
    - .MIN_VALUE
    - .MAX_SAFE_VALUE
- 实例方法
     - toSting()
     - toFixed()
- 类方法
- Number.parseInt()
- Number.parseFloat()

# Math 对象
- https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Math
- 属性
    - Math.PI
- 方法
    - floor()
    - ceil()
    - round()
    - random()
    - pow()

# String
- 属性
    - length
- 实例方法
    - toUpperCase()
    - toLowerCase()
    - slice() 截取字符串
    - substr() 截取字符串
    - concat() 连接字符串

## 字符串的不可变性

# Array
- 实例方法
    - push()
    - pop()
    - unshift()
    - shift()
    - splice() **重要** 修改原数组
    - slice() 截取数组，返回一个新的数组
    - concat()
    - join()

## 数组的 length 属性

- length 属性是可写的，可赋值
- 大于用 `empty` 填充
- 小于截取
- `.length = 0` 清空数组

## 数组的三种遍历方式

- for 普通
- for...in...
- for...of...

## 查找数组的元素

- indexOf() / lastIndexOf()
- includes()
- find((item) => )
- findIndex((item) => )

## 数组排序/反转

- sort()
- reverse()

# 时间 Date

## 两种标准

- RFC 2822
- ISO 8601

## 对象方法

- getFullYear()
- getMonth()
- getDate()
- getHours()
- getMinutes()
- getSeconds()
- getDay()

## 获取时间戳

- getTime()
- valueOf()

## parse() 方法

- 解析字符串为时间戳
