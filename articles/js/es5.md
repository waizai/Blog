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