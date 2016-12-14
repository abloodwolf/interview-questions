#border-color

##语法

- border-color：&lt;color&gt;{1,4}
- 默认值：看每个独立属性
- 适用于：所有元素
- 继承性：无
- 动画性：是
- 计算值：看每个独立属性
- 相关属性：[ border-top-color ] || [ border-right-color ] || [ border-bottom-color ] || [ border-left-color ]


##取值

- &lt;color&gt;：指定颜色。


##说明

设置或检索对象的边框颜色。

- 如果提供全部四个参数值，将按上、右、下、左的顺序作用于四边。
- 如果只提供一个，将用于全部的四边。
- 如果提供两个，第一个用于上、下，第二个用于左、右。
- 如果提供三个，第一个用于上，第二个用于左、右，第三个用于下。
- 如果border-width等于0或border-style设置为none，本属性将被忽略。
- 对应的脚本特性为borderColor。


##兼容性


<table class="compatible">
<thead>
	<tr>
		<th>Values</th>
		<th>IE</th>
		<th>Firefox</th>
		<th>Chrome</th>
		<th>Safari</th>
		<th>Opera</th>
		<th>iOS Safari</th>
		<th>Android Browser</th>
		<th>Android Chrome</th>
	</tr>
</thead>
<tbody>
	<tr>
		<td><strong>Basic Support</strong></td>
		<td class="support">6.0+</td>
		<td class="support" rowspan="5">2.0+</td>
		<td class="support" rowspan="5">4.0+</td>
		<td class="support" rowspan="5">3.1+</td>
		<td class="support" rowspan="5">3.5+</td>
		<td class="support" rowspan="5">3.2+</td>
		<td class="support" rowspan="5">2.1+</td>
		<td class="support" rowspan="5">18.0+</td>
	</tr>
	<tr>
		<td rowspan="2"><a href="../../values/color/transparent.htm">transparent</a></td>
		<td class="unsupport">6.0 <sup><a href="#support1">#1</a></sup></td>
	</tr>
	<tr>
		<td class="support">7.0+</td>
	</tr>
	<tr>
		<td rowspan="2"><a href="../../values/color/rgba.htm">RGBA</a>, <a href="../../values/color/hsl.htm">HSL</a>, <a href="../../values/color/hsla.htm">HSLA</a></td>
		<td class="unsupport">6.0-8.0 <sup><a href="#support1">#1</a></sup></td>
	</tr>
	<tr>
		<td class="support">9.0+</td>
	</tr>
</tbody>
</table>


- 需要注意的是，边框颜色如果设置了不支持的值，则效果等同于默认值 currentColor。


##示例

```html

<!DOCTYPE html>
<html lang="zh-cmn-Hans">
<head>
<style>
.test{padding:10px;border-width:1px;border-style:solid;border-color:#000;}
.test2{margin-top:10px;padding:10px;border-width:1px;border-style:solid;border-color:#000 #f00;}
.test3{margin-top:10px;padding:10px;border-width:1px;border-style:solid;border-color:#000 #f00 #090;}
.test4{margin-top:10px;padding:10px;border-width:1px;border-style:solid;border-color:#000 #f00 #090 #0ff;}
</style>
</head>
<body>
<div class="test">提供1个参数</div>
<div class="test2">提供2个参数</div>
<div class="test3">提供3个参数</div>
<div class="test4">提供4个参数</div>
</body>
</html>

```
