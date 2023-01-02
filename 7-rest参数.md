### ES6 引入 rest 参数，用于获取函数的实参，用来代替 arguments
#### 1. ES5 获取实参的方式（arguments）
```js
function date(){
  // 输出结果的原型是 object，不是一个真正的数组
  console.log(arguments);
}
date('Monday', 'Tuesday','Wednesday');
```
#### 2. rest 参数
```js
function date(...args){
  // 输出结果为数组，可以使用数组身上的方法：filter,some,every,map等
  console.log(args);
}
date('Monday', 'Tuesday','Wednesday');
```
> rest 参数必须要放到参数最后，否则报错：Rest parameter must be last formal parameter
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzc1MTE5NzA3XX0=
-->