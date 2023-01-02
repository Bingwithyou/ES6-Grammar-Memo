### 1. 一定要赋初始值
```js
// 报错：Uncaught SyntaxError: Missing initializer in const declaration
const A;
```
### 2. 一般常量使用大写（潜规则）
### 3. 常量的值（所指向的地址）不能修改
```js
// 报错：Uncaught TypeError: Assignment to constant variable. at xxx:xx
const SCHOOL = "NYC";
SCHOOL = "NYA";
```
### 4. 块级作用域
```js
// 报错：Uncaught ReferenceError: Player is not defined at xxx:xx
{
  const PLAYER = "Arthur";
}
console.log(PLAYER);
```
### 5. 对于数组和对象的元素修改不会报错
```js
// 不会报错，因为并没有修改 TEAM 数据指向的内存位置
const TEAM = ['S1mple','Perfecto','b1t','electronic','Boombl4'];
TEAM.pop()
```
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTcxMTY4OTAyOF19
-->