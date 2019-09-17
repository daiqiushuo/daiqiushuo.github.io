---
title: echarts中option的title
date: 2019-09-17 18:00:15
tags: 
- echarts
---
# echarts中option的title
```html

<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>标题</title>
</head>
<body>
	<div id = "d1" style = "width: 400px;height:400px;"></div>
	<script type="text/javascript" src = "js/echarts.min.js"></script>
	<script type="text/javascript">
		var myChart = echarts.init(document.getElementById("d1"));//初始化画布
		var option = {
			title:{
				show:"true",//是否显示标题，默认显示，可以不设置
				text:"echarts实例",//图表标题文本内容
				link:"http://echarts.baidu.com/",//点击标题内容要跳转的链接
				target:"blank",//跳转链接打开方式，blank是新窗口打开，self是自身窗口打开，跟a标签一样
				textStyle:{//标题内容的样式
					color:'#e4393c',//京东红
					fontStyle:'normal',//主标题文字字体风格，默认normal，有italic(斜体),oblique(斜体)
					fontWeight:"lighter",//可选normal(正常)，bold(加粗)，bolder(加粗)，lighter(变细)，100|200|300|400|500...
					fontFamily:"san-serif",//主题文字字体，默认微软雅黑
					fontSize:18//主题文字字体大小，默认为18px
				},
				textAlign:'left',//标题文本水平对齐方式，建议不要设置，就让他默认，想居中显示的话，建议往下看
				textBaseline:"top",//默认就好,垂直对齐方式,不要设置
				subtext:"作者:前端林三哥",//主标题的副标题文本内容，如果需要副标题就配置这一项
				sublink:"http://blog.csdn.net/zhaoxiang66",//点击副标题内容要跳转的链接
				subtarget:"blank",//同主标题，blank是新窗口打开，self是自身窗口打开
				subtextStyle:{//副标题内容的样式
					color:'green',//绿色
					fontStyle:'normal',//主标题文字字体风格，默认normal，有italic(斜体),oblique(斜体)
					fontWeight:"lighter",//可选normal(正常)，bold(加粗)，bolder(加粗)，lighter(变细)，100|200|300|400|500...
					fontFamily:"san-serif",//主题文字字体，默认微软雅黑
					fontSize:12//主题文字字体大小，默认为12px
				},
				padding:5,//各个方向的内边距，默认是5，可以自行设置
				itemGap:10,//主标题和副标题之间的距离，可自行设置
				left:"center",//left 的值可以是像 20 这样的具体像素值，可以是像 '20%' 这样相对于容器高宽的百分比，也可以是 'left', 'center', 'right',如果 left 的值为'left', 'center', 'right'，组件会根据相应的位置自动对齐。
				top:"center",//left 的值可以是像 20 这样的具体像素值，可以是像 '20%' 这样相对于容器高宽的百分比，也可以是 'left', 'center', 'right',如果 left 的值为'left', 'center', 'right'，组件会根据相应的位置自动对齐。
				right:"auto",//right 的值可以是像 20 这样的具体像素值，可以是像 '20%' 这样相对于容器高宽的百分比。
				bottom:"auto",//bottom 的值可以是像 20 这样的具体像素值，可以是像 '20%' 这样相对于容器高宽的百分比。
				//left设置center标题会自动水平居中
				//top设置center标题会自动垂直居中
				backgroundColor:"#ccc",//标题背景色，默认透明，颜色可以使用 RGB 表示，比如 'rgb(128, 128, 128)' ，如果想要加上 alpha 通道，可以使用 RGBA，比如 'rgba(128, 128, 128, 0.5)'，也可以使用十六进制格式，比如 '#ccc'
				borderColor:"red",//标题的边框颜色，颜色格式支持同backgroundColor
				borderWidth:2,//标题边框线宽，默认为0，可自行设置
				shadowBlur: 10,//图形阴影的模糊大小。该属性配合 shadowColor,shadowOffsetX, shadowOffsetY 一起设置图形的阴影效果。
				shadowColor: "black",
				shadowOffsetX: 0,
				shadowOffsetY: 0,
			}
		}
		myChart.setOption(option);
	</script>
</body>
</html>


```