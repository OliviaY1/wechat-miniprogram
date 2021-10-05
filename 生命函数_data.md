## Intro
在xtml中绑定一个生命函数, 用`bindxxx= "handleUserInfo"`回调中获取到用户信息

在js文件中保存用户信息

```js
data: {
    var_name: {} //data中初始化一个值
}
handleUserInfo(res){
    if (res.detail.userInfo){ // 如果用户点击了授权
        this.setData({
            var_name: res.detail.userInfo 
        })
    }
}
```

## 语句
JS内
1. if(){}
2. if(){} else{}
3. if(){} else if(){} else{}
4. for (var i=0; i<5; i++){}  
    初始化变量；条件表达式；操作表  

`&&` -> and `||` -> or `!` -> not

xwml内
1. wx: if="{{ }}"
2. wx: elif = "{{ }}"
3. wx: else

### types
number 可以做基本的 `+ - * / %`

string
- 18 == '18' 判断值
- 18 === '18' 判断值+类型
- string1.length

var name = null
判断变量的类型 `typeof variable`

转换为string： `var1.toString` `" "+ var1` `string(var1)`  
转换为int: `Number(var1)` `parseFloat(var1)` `parseInt(var1)`: return an int
- Number(" ") -> 0
- Number(true) -> 1
- Number(false) -> 0
- Number("str") -> NaN

Array 数组
1. var name = [..,..,..]
2. var name = new Array()  
    name[0] = '...' 先新建一个数组，之后再赋值

对象
1. var name = {xx:value, xx2:value2, 方法名: function(){}}

Date 日期
1. var date = new Date()
2. var date = new Date(年，月，日)

---
cite data base  `const name = wx.cloud.database()`  
get data `name.collection("demo_name").doc("data id").get({})`
