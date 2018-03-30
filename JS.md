# Java Script
***
## JS对大小写敏感
- **查找 HTML 元素**
    - 通过 id 找到 HTML 元素
    - 通过 id 找到 HTML 元素
    - 通过类名找到 HTML 元素

* **变量: 用var**
```javascript
var a=12,b=11;
//只有一种数字类型
var s='ss',v="sad";

```
- **数组:**
```javascript
var a = new Array("a","s");
//or
var a = new Array();
a[0]="aa";
a[1]="ww";
...
```
- **对象:**
*对象由花括号分隔。在括号内部，对象的属性以名称和值对的形式 (name : value) 来定义。属性由逗号分隔*
```javascript
var person={firstname:"Bill", lastname:"Gates", id:5566};
//在 JavaScript 中，对象是数据（变量），拥有属性和方法。
```
- **添加对象属性:**
```javascript
person=new Object();
person.firstname="Bill";
person.lastname="Gates";
person.age=56;
person.eyecolor="blue";
```
- **函数:**
*可以发送任意多的参数，由逗号分隔；当您声明函数时，请把参数作为变量来声明；变量和参数出现顺序需一致.*
*函数内为局部变量，函数外为全局变量*
- **生命周期：**
    - JavaScript 变量的生命期从它们被声明的时间开始。
    - 局部变量会在函数运行以后被删除。
    - 全局变量会在页面关闭后被删除。

```
<button onclick="myFunction('Bill Gates','CEO')">点击这里</button>

<script>
function myFunction(name,job)
{
alert("Welcome " + name + ", the " + job);
}
</script>
```
- **运算：**
数字与字符串相加，结果将成为字符串。
- **错误处理:**
    - **try** 语句测试代码块的错误。
    - **catch** 语句处理错误。
    - **throw** 语句创建自定义错误。

**实例：**
```javascript
<!DOCTYPE html>
<html>
<head>
<script>
var txt="";
function message()
{
try
  {
  adddlert("Welcome guest!");
  }
catch(err)
  {
  txt="There was an error on this page.\n\n";
  txt+="Error description: " + err.message + "\n\n";
  txt+="Click OK to continue.\n\n";
  alert(txt);
  }
}
</script>
</head>

<body>
<input type="button" value="View message" onclick="message()">
</body>

</html>
```