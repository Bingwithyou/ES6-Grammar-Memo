### ES6 引入 rest 参数，用于获取函数的实参，用来代替 arguments
#### 1. ES5 获取实参的方式
```js
function date(){
  // 输出结果的原型是 object
  console.log(arguments);
}
date('Monday', 'Tuesday','Wednesday');
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTEzNzc3OTM0MDksLTIwODg3NDY2MTJdfQ
==
-->