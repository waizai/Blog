## ES5

### Object

1. [Object.keys(object)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/keys)   // 以数组返回所有可枚举的属性
2. [Object.defineProperty(object, property, descriptor)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/defineProperty)  // 添加或更改对象属性
3. Object.defineProperties(object, descriptors) // 添加或更改多个对象属性
4. Object.getOwnPropertyDescriptor(object, property) // 访问属性
5. Object.getOwnPropertyNames(object) // 以数组返回所有属性

7. Object.getPrototypeOf(object)  // 访问原型

8. Object.preventExtensions(object)  // 阻止向对象添加属性

9. Object.isExtensible(object)  // 如果可将属性添加到对象，则返回 true

10. Object.seal(object) // 防止更改对象属性（而不是值）

11. Object.isSealed(object) // 如果对象被密封，则返回 true

12. Object.freeze(object)   // 防止对对象进行任何更改

13. Object.isFrozen(object)  // 如果对象被冻结，则返回 true

14. Object.create ( O [, Properties] )   // 创建一个新对象，使用现有的对象来提供新创建的对象的__proto__。
15. Object.prototype.constructor
16. Object.prototype.toString ( )
17. Object.prototype.toLocaleString ( )
18. Object.prototype.valueOf ( )
19. [Object.prototype.hasOwnProperty (V)](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Object/hasOwnProperty)   // 返回一个布尔值，指示对象自身属性中是否具有指定的属性（也就是，是否有指定的键）。
20. Object.prototype.isPrototypeOf (V)
21. Object.prototype.propertyIsEnumerable (V)


### Array

1. Array.isArray()    // 用于确定传递的值是否是一个 Array
2. Array.forEach()    // 方法对数组的每个元素执行一次提供的函数。返回值undefined
3. Array.map()      // 创建一个新数组，其结果是该数组中的每个元素都调用一个提供的函数后返回的结果。
4. Array.filter()   // 创建一个新数组, 其包含通过所提供函数实现的测试的所有元素。
5. Array.reduce()    // 对数组中的每个元素执行一个由您提供的reducer函数(升序执行)，将其结果汇总为单个返回值。
6. Array.reduceRight()   // 接受一个函数作为累加器（accumulator）和数组的每个值（从右到左）将其减少为单个值。
7. Array.every()   // 测试一个数组内的所有元素是否都能通过某个指定函数的测试。它返回一个布尔值。
8. Array.some()   // 测试数组中是不是至少有1个元素通过了被提供的函数测试。它返回的是一个Boolean类型的值。
9. Array.indexOf()   // 返回在数组中可以找到一个给定元素的第一个索引，如果不存在，则返回-1。
10. Array.lastIndexOf()   // 返回指定元素（也即有效的 JavaScript 值或变量）在数组中的最后一个的索引，如果不存在则返回 -1。从数组的后面向前查找，从 fromIndex 处开始


###指令
"use strict" 指令

###String
1. String.trim()    // 从一个字符串的两端删除空白字符
2. String.prototype.charAt()   // 从一个字符串中返回指定的字符。



### JSON
1. JSON.parse()    
2. JSON.stringify()   // 将一个 JavaScript 值（对象或者数组）转换为一个 JSON 字符串



### Date
1. Date.now()    // 返回自1970年1月1日 00:00:00 UTC到当前时间的毫秒数。


###函数
1. [属性 Getter ](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Functions/get)   // get语法将对象属性绑定到查询该属性时将被调用的函数。

2. [Setter](https://developer.mozilla.org/zh-CN/docs/Web/JavaScript/Reference/Functions/set)