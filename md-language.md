# 目录
<link rel="stylesheet" href="http://yandex.st/highlightjs/6.2/styles/googlecode.min.css">

<script src="http://code.jquery.com/jquery-1.7.2.min.js"></script>

<script src="http://yandex.st/highlightjs/6.2/highlight.min.js"></script>

<script>hljs.initHighlightingOnLoad();</script>

<script type="text/javascript">

	$(document).ready(function(){

 		$("h2,h3,h4,h5,h6").each(function(i,item){

 			var tag = $(item).get(0).localName;

 			$(item).attr("id","wow"+i);

 			$("#category").append('<a class="new'+tag+'" href="#wow'+i+'">'+$(this).text()+'</a></br>');

			$(".newh1").css("margin-left",0);
 			$(".newh2").css("margin-left",10);
 			$(".newh3").css("margin-left",20);
 			$(".newh4").css("margin-left",40);
 			$(".newh5").css("margin-left",60);
 			$(".newh6").css("margin-left",80);
		});
		$("#category").css("font-size",16);
	});

</script>

<div id="category"></div>


##  标题
	# 一级 
	## 二级  有下划线
	### 三级
	#### 四级
	##### 五级
	###### 六级

  `##### cmd+#号数  立即打标题`

##  列表
* 无序列表11
* 无序列表12

- 无序列表21
- 无序列表22

+ 无序列表31
+ 无序列表32

1. 有序列表1
2. 有序列表2

## 做笔记

1. 第一节
* 第二节
	* 第一小节
		* 小小节1
		* 小小节2
	* 第二小节


## 单行代码块
`tab 键即可缩进`

## 多行代码块
```
tab 键即可缩进

```
```python
@requires_authorization
def somefunc(param1='', param2=0):
    '''A docstring'''
    if param1 > param2: # interesting
        print 'Greater'
    return (param2 - param1 + 1) or None
class SomeClass:
    pass
>>> message = '''interpreter
... prompt'''
```

## 注释
<!--我是注释，你看不见我-->

## 引用


在引用的段落前面加一个>，即表示你引用的段落，背景也会不一样
> 引用的表人的话，如果想换行，就再加一个>
> 衣带渐宽终不悔，为伊消得人憔悴
>> 二级引用 
>>> 三级引用

>> 回到二级引用

> 回到一级引用__

## 图片
![春花秋月图](http://dizhiya/dizhi)

## 后面指定图片链接
[![指定图片的多个链接]][link1][link2]
[link1]: http://img3.douban.com/mpic/s1108264.jpg
[link2]: http://book.douban.com/subject/1141406/

## 链接
[Baidu](http://www.baidu.com)

## 后面指定链接
[**我暂时是一个空链接**][null-link]
[null-link]: https://www.baidu.com

## 链接加hover
P.S. [我是一个有**hover效果**的链接哦 ~][hover]
[hover]: http://www.baidu.com 
## 粗体
**这就是粗体**

## 斜体
*这就是斜体*

## 文字底纹
这几个文字就是`有底纹的文字`,用俩引号就是重点字了哦

## 删除线

~~文字删除线~~  需要设置 preferences->MarkDown-> Strikethrough

## 高亮文字

==高亮文字== 需要设置 preferences->MarkDown->highlight

## 下划线
我是一个可爱的_下划线呀下划线_

## 小文本
<small>文本内容</small>

## 分割线
我就是一条可爱的分割线，哈哈哈哈
***
我也是哦

---

## 水平线

--
两个减号表示实线

--- 
三个减号表示虚线

## 换行
1. 使用标签，间距小一点
第一行</br>第二行

2. 在末尾敲击两个以上空白，然后回车，间距较大
第一行  
第二行

## 空格
在这一行里面添加空格吧，来一个&nbsp;呀，来两个&nbsp;&nbsp;呀


## 首行缩进
1. 敲空格，不管用
2. 使用占位符  &ensp;或&#8194; //半角   &emsp;或&#8195; //全角  &nbsp; //空格

&ensp;&ensp;&ensp;&ensp;首行缩进
第二行没有缩进

## 表格
| 左对齐     | 居中对齐    |   右对齐  |
|-----------|:----------:|----------:|
| row1 col1 | row1 col2  | row1 col3 |
|      row2 | row2       | row2      |
| row3 col3 | row3 col2  | row3 col3 |


## 公式
`行内公式`
		
$\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$

`块级公式`
$$	x = \dfrac{-b \pm \sqrt{b^2 - 4ac}}{2a} $$

## 复选框
使用 `- [ ]` 和 `- [x]` 语法可以创建复选框，实现 todo-list 等功能。例如：

- [x] 已完成事项
- [ ] 待办事项1
- [ ] 待办事项2

## 流程图

```flow
st=>start: Start
e=>end
op=>operation: My Operation
cond=>condition: Yes or No?

st->op->cond
cond(yes)->e
cond(no)->op
```

## 时序图
```sequence
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob-->Alice: I am good thanks!
```

## 脚注
我是一个脚注[^demo]哦。点它就能回到我这里哦~~

[^demo]: 这是一个示例脚注。

## 锚点
[第一章](#first_page)
<A NAME="first_page">第一章引子</A>

## 其他
* 段落   段落与 段落之间一定要空一行


