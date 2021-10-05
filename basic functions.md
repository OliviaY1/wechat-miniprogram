`<view class=""> </view>` 小组件
	`padding: #px` `text-align: center`

`<image src = '/images/xxx.jpg'>` "/"代表此根目录文件下

## 表单

```xml
<form>
    <input class='' placeholder='' placeholder-style=''> </input>
</form>

属性：autofocus
```



## 滑动：

```xml
<swiper>
    <swiper-item> <image src="/"> </swiper-item>
    <swiper-item> </swiper-item>
</swiper>
```
一些属性：`indicator-dot` `indicator-color` `indicator-active-color` `circular` `next-margin / previous-margin`
<https://developers.weixin.qq.com/miniprogram/dev/component/swiper.html>

## 按钮：
`<button> </button>`
属性：
`size='mini'` `type`
<https://developers.weixin.qq.com/miniprogram/dev/component/button.html>

## icon

`<icon type=" " size=" "> </icon>`

## 进度条 

`<progress percent= '' activeColor= ''> </progress> `
<https://developers.weixin.qq.com/miniprogram/dev/component/progress.html>



# 结构

app.json 中page创建一个页面
app.json中window调整导航，背景等变化
	`"enablePullDownRefresh": true` 开启下拉刷新
	`"backgroundColor":` 下拉刷新的背景色
	`"navigationBarTitleText": ""`

app.json中tabbar: list中至少两个参数
<https://developers.weixin.qq.com/miniprogram/dev/reference/configuration/app.html#tabBar>

```xml
"tabBar" : {
	"list":[
		{
			"pagePath": " ",
			"text": " ",
			"iconPath": " ",
			"selectedIconPath": " "
		},{
			"pagePath": " ",
			"text": " "
		}
	]
}
```

page json中设置单个配置

js：

​	data can store list, set, string; use {{ }} in wxml

`wx:if="{{判断内容}}"`





