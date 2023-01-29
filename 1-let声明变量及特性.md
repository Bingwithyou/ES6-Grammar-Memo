### 1. 变量不能重复声明
```js
let star = "Altair";
let star = "Altair";
// 报错：Uncaught SyntaxError: Identifier 'Altair' has already been declared
```
### 2. 块级作用域
```js
{
  let girl = "Sadie";
}
console.log(girl);
// 报错：Uncaught ReferenceError: girl is not defined at xxx:xx
```
### 3. 不存在变量提升
> 一般 var 声明的变量会存在变量提升，即在解析代码时会将所有声明语句提到最上边，之后再按顺序依次执行
```js
 // 不会报错，但输出结果为 undefined，因为存在变量提升
 console.log(song)
 var song = "Wintering"
 
 // 报错：Uncaught ReferenceError: cannot access 'song' before initialization at xxx:xx
 console.log(song)
 let song = "Wintering"
```
### 4. 不影响作用域链
```js
{
  // 函数作用域内找不到 school ，会向上一级作用域传递
  let school = 'NYA'
  function fn(){
	console.log(school)
  }
}
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE5ODI4NTk0NzYsLTExNzgwNzM2NzFdfQ
==
-->