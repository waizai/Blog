# JSONP原理
## 问题
1. 前端是如何拿到后端的回调的？    正常get请求
2. 拿到回调后如何调起回调函数？   js注入
3. 这中间前端需要做什么？    声明callback
4. 后端又需要做些什么来支持？   跟前端统一callbackName
5. 超时场景又该如何处理？    监听script元素on error事件回调逻辑
6. 整个生命周期会有多个钩子可以被触发，而我们可以监听哪些钩子来得知请求的状况?
ajaxComplete钩子
ajaxError钩子
ajaxStop钩子





[demo](../../demos/jsonp/jquery.html)