---
title: "博客主题-蜘蛛"
date: 2023-03-20T08:00:00+08:00
draft: true
---

## 二级标题
### 三级标题
#### 四级标题
##### 五级标题


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

> “这一路上走走停停 顺着少年漂流的痕迹”

**加粗文本**

*斜体文本*

~~删除文本~~

这是行内式链接：[Azir's Articles](https://example.com/)

这是行内代码`onCreate(Bundle savedInstanceState)`的例子。

这是一行后面加两个空格  换行

使用 Markdown[^1]可以效率的书写文档, 直接转换成 HTML[^2], 你可以使用 Typora[^3] 编辑器进行书写。
[^1]:[Markdown - 维基百科，自由的百科全书](https://zh.wikipedia.org/wiki/Markdown)
[^2]:[HTML - 维基百科，自由的百科全书](https://zh.wikipedia.org/wiki/HTML)
[^3]:[Typora - 维基百科，自由的百科全书](https://zh.wikipedia.org/wiki/Typora)

以下是图片的显示效果

![大图片](5k.heic)

以上就是全部的显示效果了,以上就是全部的显示效果了,以上就是全部的显示效果了.以上就是全部的显示效果了,以上就是全部的显示效果了,以上就是全部的显示效果了.

