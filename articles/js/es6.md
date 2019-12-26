## ES6


### 类
### 模块化

1. ES6模块化和CommonJS 和 AMD 模块的区别    
    - ES6模块化: 
        1. 设计思想静态化，__编译时确定依赖关系__；输入输出变量。import的是n个方法。
        2. export语句输出的接口，与其对应的值是动态绑定关系，即通过该接口，可以取到模块内部实时的值。
        3. import命令输入的变量都是 __只读__ 的，因为它的本质是输入接口。也就是说，不允许在加载模块的脚本里面，改写接口。
        4. import命令具有提升效果，会提升到整个模块的头部，首先执行。
    - CommonJS 和 AMD: 
        1. require的是个对象，再从对象上读取方法，属于 __运行时加载__。
        2. CommonJS 模块输出的是值的缓存，不存在动态更新
2. ES6主要功能
    - export命令规定的是对外的接口，必须与模块内部的变量建立一一对应关系。
    ```javascript
        // 一组变量
        export { firstName, lastName, year };
        // 函数或者类
        export function multiply(x, y) {
            return x * y;
        };
        // 可以使用as关键字重命名
        export {
            v1 as streamV1,
            v2 as streamV2,
            v2 as streamLatestVersion
        };
        
        // 为模块指定默认输出
        // 本质上，export default就是输出一个叫做default的变量或方法，然后系统允许你为它取任意名字
        export default function () {
            console.log('foo');
        }
        export default 42;
        // import命令可以为该匿名函数指定任意名字。
        // 下面2种写法都可以
        import customName from './export-default';
        import { default as foo } from './export-default';

        
        
        import { firstName, lastName, year } from './profile.js';
        // 可以使用as关键字重命名
        import { lastName as surname } from './profile.js';
        import * as circle from './circle';
        // 仅仅执行lodash模块，但是不输入任何值。
        import 'lodash';```
3. ES2020提案 引入import()函数，支持动态加载模块。



### 箭头函数
### 函数参数默认值
### 模板字符串
### 解构赋值
### 延展操作符
### 对象属性简写
### Promise
### Let与Const
### Object



### Array