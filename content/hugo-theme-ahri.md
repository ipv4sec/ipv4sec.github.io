---
title: "本站博客主题-阿璃"
date: 2023-03-10T08:00:00+08:00
draft: false
---

# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题

* Red
* Green
* Blue

1. Red
2. Green
3. Blue

| 表头  | 表头  |
|-----|-----|
| 单元格 | 单元格 |
| 单元格 | 单元格 |

```
func Init(dsn string) (err error) {
	db, err := gorm.Open(mysql.New(mysql.Config{
		DSN: fmt.Sprintf("gorm:gorm@tcp(localhost:3306)/example??charset=utf8mb4&parseTime=True&loc=%s", "Asia%2FShanghai"),
	}), &gorm.Config{})
}
```

> “We live in a networked world in which each company partners with a set of other companies.”

**加粗文本** 

*斜体文本* 

~~删除文本~~

这是行内式链接：[Azir's Articles](https://opensource.moejs.com/)

这是行内代码`onCreate(Bundle savedInstanceState)`的例子。

这是一行后面加两个空格  换行

使用 Markdown[^1]可以效率的书写文档, 直接转换成 HTML[^2], 你可以使用 Typora[^T] 编辑器进行书写。
[^1]:Markdown是一种纯文本标记语言
[^2]:HyperText Markup Language 超文本标记语言
[^T]:NEW WAY TO READ & WRITE MARKDOWN.


以下是图片的显示效果

![](assets/favicon.png)

以上就是全部的显示效果了,以上就是全部的显示效果了,以上就是全部的显示效果了.以上就是全部的显示效果了,以上就是全部的显示效果了,以上就是全部的显示效果了.

