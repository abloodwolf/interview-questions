#相邻选择符(E+F)

##语法

- E+F { sRules }


##说明

选择紧贴在E元素之后F元素。

- 与兄弟选择符不同的是，相邻选择符只会命中符合条件的相邻的兄弟元素。

**E~F VS. E+F：**

```html
<style>
	/* 相邻选择符(E+F) */
	p+p{color:#f00;}
	/* 兄弟选择符(E~F) */
	p~p{color:#f00;}
</style>
<p>p1</p>
<p>p2</p>
<h3>这是一个标题</h3>
<p>p3</p>
<h3>这是一个标题</h3>
<p>p4</p>
<p>p5</p>
```

>此例，如果使用p + p{color:#f00;}，那么p2, p5将会变成红色；如果使用p ~ p{color:#f00;}，那么p2,p3,p4,p5将会变成红色；




##兼容性


<table class="compatible">
<thead>
	<tr>
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
		<td class="unsupport">6.0</td>
		<td class="support" rowspan="2">2.0+</td>
		<td class="support" rowspan="2">4.0+</td>
		<td class="support" rowspan="2">3.1+</td>
		<td class="support" rowspan="2">3.5+</td>
		<td class="support" rowspan="2">3.2+</td>
		<td class="support" rowspan="2">2.1+</td>
		<td class="support" rowspan="2">18.0+</td>
	</tr>
	<tr>
		<td class="support">7.0+</td>
	</tr>
</tbody>
</table>




##示例

```html

<!DOCTYPE html>
<html lang="zh-cmn-Hans">
<head>
<style>
p + p {
	color: #f00;
}
</style>
</head>
<body>
<div class="test">
	<h3>这是一个标题</h3>
	<p>这是一个文字段落</p>
	<p>这是一个文字段落</p>
	<h3>这是一个标题</h3>
	<p>这是一个文字段落</p>
	<h3>这是一个标题</h3>
	<p>这是一个文字段落</p>
	<p>这是一个文字段落</p>
</div>
</body>
</html>

```
